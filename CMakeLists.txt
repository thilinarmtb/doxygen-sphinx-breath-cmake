cmake_minimum_required (VERSION 3.8)
project("cc")

set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} "${PROJECT_SOURCE_DIR}/cmake")

add_library(cc "cc/cc.cpp" "cc/cc.h")
target_include_directories(cc PUBLIC cc)
add_subdirectory("docs")
