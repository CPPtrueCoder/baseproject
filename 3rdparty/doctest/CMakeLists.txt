cmake_minimum_required(VERSION 2.8)

set(DOCTEST_SRCS testclass.h testclass.cpp main.cpp)
SET(LIB_TYPE STATIC)
add_library(doctest${LIB_TYPE}${DOCTEST_SRCS})
