# Minimum CMake version
cmake_minimum_required(VERSION 3.10)

# Project name
project(two)

# Specify the C++ standard
set(CMAKE_CXX_STANDARD 14)

# Add the source files for the library
add_library(two STATIC src/libtwo.cpp)

# Specify the include directories
target_include_directories(two PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/src)
