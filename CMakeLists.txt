cmake_minimum_required(VERSION 3.24.0)

project(
  cuda_debug
  VERSION 0.1.0
  LANGUAGES CUDA CXX)
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CUDA_STANDARD 20)
set(CMAKE_CUDA_STANDARD_REQUIRED ON)
set(CMAKE_CUDA_ARCHITECTURES native)

find_package(CUDAToolkit REQUIRED)

add_executable(name_too_long name_too_long/name_too_long.cpp)
target_link_libraries(name_too_long PRIVATE CUDA::nvrtc)
