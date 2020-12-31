cmake_minimum_required(VERSION 3.17)
project(cuda_practice CUDA)

set(CMAKE_CUDA_STANDARD 14)

add_executable(add add.cu)

set_target_properties(
        add
        PROPERTIES
        CUDA_SEPARABLE_COMPILATION ON)