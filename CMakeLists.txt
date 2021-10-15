cmake_minimum_required(VERSION 3.20)
project(cuda_executable CUDA)

set(CMAKE_CUDA_STANDARD 14)

add_executable(cuda_executable main.cu)

set_target_properties(cuda_executable PROPERTIES
        CUDA_SEPARABLE_COMPILATION ON)
