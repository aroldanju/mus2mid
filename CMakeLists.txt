cmake_minimum_required(VERSION 3.14.3)
project(mus2mid)

set(CMAKE_CXX_STANDARD 14)

file(GLOB MUS2MID_SOURCES libmus2mid/*.h libmus2mid/*.cpp)

add_library(${PROJECT_NAME} ${MUS2MID_SOURCES})
add_library(dependencies::mus2mid ALIAS ${PROJECT_NAME})

