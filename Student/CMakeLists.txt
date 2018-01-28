cmake_minimum_required(VERSION 2.8.9)
project(directory_test)

#Include headers such as Student.h into the project
include_directories(include)

# Configure sources
set(SOURCES src/main.cpp src/Student.cpp)

add_executable(student ${SOURCES})
