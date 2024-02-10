cmake_minimum_required(VERSION 3.25)

project(
    "stb"
    VERSION 1.0.0
    DESCRIPTION "Contains a set of files from the stb library: https://github.com/nothings/stb"
    LANGUAGES C CXX
)

add_library("stb" INTERFACE
    "${CMAKE_CURRENT_SOURCE_DIR}/include/stb/stbImageLoad.h"
    "${CMAKE_CURRENT_SOURCE_DIR}/include/stb/stbImageWrite.h"
    "${CMAKE_CURRENT_SOURCE_DIR}/include/stb/stbImageResize.h"
)

target_include_directories("stb" INTERFACE
    "${CMAKE_CURRENT_SOURCE_DIR}/include/"
)