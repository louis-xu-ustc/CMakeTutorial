cmake_minimum_required(VERSION 2.8)
project(Part4Project)

set(CMAKE_CXX_FLAGS "-std=c++0x -Wall")
message("CMAKE_BUILD_TYPE is $(CMAKE_BUILD_TYPE)")

if (CMAKE_BUILD_TYPE STREQUAL Debug)
    set(BUILD_POSTFIX "_d")
else(CMAKE_BUILD_TYPE STREQUAL Debug)
    set(BUILD_POSTFIX "")
endif(CMAKE_BUILD_TYPE STREQUAL Debug)

include_directories(src/include)
add_subdirectory(src)
add_subdirectory(test)
