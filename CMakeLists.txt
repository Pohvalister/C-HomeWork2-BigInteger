cmake_minimum_required(VERSION 3.5)

project(My_big_int_v1.1)



add_executable(big_integer_testing
               big_integer_testing.cpp
               big_integer.h
               big_integer.cpp
               gtest/gtest-all.cc
               gtest/gtest.h
               gtest/gtest_main.cc
        )


set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall -Wextra -std=c++11 -pedantic -O3 -fstrength-reduce -fthread-jumps")

target_link_libraries(big_integer_testing -lpthread)
