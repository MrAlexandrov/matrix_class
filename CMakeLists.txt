cmake_minimum_required(VERSION 3.14)
project(matrix CXX)

set(CMAKE_CXX_STANDARD 20)

include_directories(${CMAKE_SOURCE_DIR}/include)

add_executable(${PROJECT_NAME} ${CMAKE_SOURCE_DIR}/main.cpp)

enable_testing()
add_subdirectory(${CMAKE_SOURCE_DIR}/tests)

set(CTEST_BINARY_DIRECTORY ${CMAKE_BINARY_DIR})