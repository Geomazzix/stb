cmake_minimum_required(VERSION 3.25)

project(
    stb
    VERSION 1.0.0
    DESCRIPTION "stb"
    LANGUAGES C CXX
)

add_library(stb INTERFACE
    "${CMAKE_CURRENT_SOURCE_DIR}/stbImageLoad.h"
    "${CMAKE_CURRENT_SOURCE_DIR}/stbImageWrite.h"
    "${CMAKE_CURRENT_SOURCE_DIR}/stbImageResize.h"
)