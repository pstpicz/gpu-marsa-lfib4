cmake_minimum_required(VERSION 3.7)
find_package(CUDA  REQUIRED)


# Pass options to NVCC
set(
    CUDA_NVCC_FLAGS
    ${CUDA_NVCC_FLAGS};
    -O3 -Xcompiler -fopenmp
    )

include_directories(
    src
    )

cuda_add_executable(
    lfib4
    src/lfib4.cu
    )

target_link_libraries(
    lfib4
    -lgomp
    )