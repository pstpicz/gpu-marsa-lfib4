# README #

gpu-marsa-lfib4 implements in CUDA (currently) and OpenACC (will be added soon)
our new parallel and fully vectorized version on Marsa-LFIB4. Details can be
found in (https://doi.org/10.1016/j.jpdc.2019.12.004).

### Requirements ###

Tested compilers and GPUs

* NVCC 10.1 for CUDA (with gcc 6.3.0) on GeForce RTX 2080 SUPER
* NVCC  9.0 for CUDA (with gcc 4.4.7) on Tesla K40m 
* NVCC  8.0 for CUDA (with gcc 4.8.5) on Tesla M2050 


### Compiling and running ###

* CUDA

````
cd cuda
mkdir build
cd build
cmake ..
make
````

* OpenACC (will be added soon)

````
cd acc
mkdir build
cd build
cmake ..
make
````



### Citing gpu-marsa-lfib4 ###

If you publish work that mentions gpu-marsa-lfib4, please cite the following paper:

````
@article{Stpiczynski19c,
  author = {Przemyslaw Stpiczynski},
  title = {Algorithmic and language-based optimization of {Marsa-LFIB4} 
            pseudorandom number generator using {OpenMP}, {OpenACC} and {CUDA}},
  journal = {Journal of Parallel and Distributed Computing},
  year = {2020},
  volume = {137},
  pages = {238--245},
  doi = {10.1016/j.jpdc.2019.12.004}
}
````

If you use this implementation in your software, please let me know.

Przemyslaw Stpiczynski
(http://stpiczynski.umcs.lublin.pl/)
