cmake_minimum_required(VERSION 2.8)

project(gtest_cmake)

set(CMAKE_CXX_FLAGSS "${CMAKE_CXX_FLAGS} -std=c++11 -g -pthread -Wfatal-errors -O2")

include_directories("${CMAKE_CURRENT_SOURCE_DIR}/third_party/googletest/googletest")
include_directories("${CMAKE_CURRENT_SOURCE_DIR}/third_party/googletest/googletest/include")

file(GLOB SRC_DIR "${CMAKE_CURRENT_SOURCE_DIR}/third_party/googletest/googletest/src/*.cc")
add_library(gtest_shared SHARED ${SRC_DIR})


















