cmake_minimum_required(VERSION 2.8)
project(Part3Project)

set(CMAKE_CXX_FLAGS "-std=c++0x -Wall")
message("CMAKE_BUILD_TYPE is $(CMAKE_BUILD_TYPE)")
add_executable(part3 main.cc)
set_target_properties(part3 PROPERTIES DEBUG_POSTFIX "_d")
set_target_properties(part3 PROPERTIES RUNTIME_OUTPUT_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/bin)
