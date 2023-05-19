cmake_minimum_required(VERSION 3.24)
project(PosixThreadsLab)

set(CMAKE_CXX_STANDARD 17)
include_directories(/opt/homebrew/Cellar/mpich/4.1/include)
set(CMAKE_C_COMPILER "/opt/homebrew/bin/mpicc")
set(CMAKE_CXX_COMPILER "/opt/homebrew/bin/mpic++")

add_executable(PosixThreadsLab main.cpp)
target_link_libraries(PosixThreadsLab m)