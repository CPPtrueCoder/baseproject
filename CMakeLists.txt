cmake_minimum_required(VERSION 2.8)

project(app)
set(DOCTEST_INCLUDE_DIR ${CMAKE_CURRENT_SOURCE_DIR}3rdparty/doctest)
add_subdirectory(3rdparty/doctest)
include_directories(${DOCTEST_INCLUDE_DIR})
add_executable(tester main.cpp)
target_link_libraries(tester doctest)
add_dependencies(tester doctest)
