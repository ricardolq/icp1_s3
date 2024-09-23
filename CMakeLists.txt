cmake_minimum_required(VERSION 3.28)
project(MyProject LANGUAGES C CXX)

if (CMAKE_BUILD_TYPE MATCHES "Debug")
    enable_testing()
    #SET(CMAKE_CXX_FLAGS "-g -O0 -Wall -fprofile-arcs -ftest-coverage")
    #SET(CMAKE_C_FLAGS "-g -O0 -Wall -W -fprofile-arcs -ftest-coverage")
endif()

add_subdirectory(include/sample_gtest)
add_subdirectory(tests)