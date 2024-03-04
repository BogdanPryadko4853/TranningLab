cmake_minimum_required(VERSION 3.26)
project(untitled C)

set(CMAKE_C_STANDARD 11)

add_executable(untitled main.c
        libs/data_structure/vector/vector.h
        libs/data_structure/vector/vector_void.h
        libs/data_structure/vector/vector.c
        libs/data_structure/vector/vector_void.c
)

add_subdirectory(libs)
target_link_libraries(data_structure)