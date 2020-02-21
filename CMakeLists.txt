cmake_minimum_required(VERSION 3.10 FATAL_ERROR)

project(MyProject VERSION 0.1.0 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17 CACHE STRING "")
set(CMAKE_CXX_STANDARD_REQUIRED yes CACHE STRING "")
set(CMAKE_CXX_EXTENSIONS no CACHE STRING "")
set(MY_PROJECT_GENERATED_INCLUDEDIR "${PROJECT_BINARY_DIR}/generated/include" CACHE STRING "Where to place the header files configured by CMake.")

add_subdirectory(src)
