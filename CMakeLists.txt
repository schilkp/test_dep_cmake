cmake_minimum_required(VERSION 3.20)
project(RandomProject VERSION 0.1.0 LANGUAGES CXX)

# Set C++23 standard
set(CMAKE_CXX_STANDARD 23)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

# Add the library
add_library(RandomLib
    src/random_lib.cpp
)

target_include_directories(RandomLib
    PUBLIC
        ${CMAKE_CURRENT_SOURCE_DIR}/include
)
