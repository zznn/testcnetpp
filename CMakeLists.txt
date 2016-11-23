cmake_minimum_required(VERSION 3.3)
project(testcnetpp)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

#include_directories("${CMAKE_SOURCE_DIR}/src")
include_directories("/usr/local/include/cnetpp/")
#include_directories("/Users/zhulei/Desktop/cnetpp/cnetpp/src/")

set(SOURCE_FILES main.cpp)
add_executable(testcnetpp ${SOURCE_FILES})
target_link_libraries(testcnetpp cnetpp pthread)