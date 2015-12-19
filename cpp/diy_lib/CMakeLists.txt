cmake_minimum_required(VERSION 3.4)      # Check cmake version. always a good practice

project(libhello)                        # Change this to reflect your project

set(CMAKE_BUILD_TYPE Debug)              # Set build debug/release

include_directories(/usr/local/include)  # Add any lib include to be added

add_library(libconfig MODULE libhello.cpp)  # Set source compile as library
                                         # 'MODULE' generates .so.1 file
                                         # 'SHARED' generates .dylib file OSX

add_subdirectory(test)                   # Add unit test dir
