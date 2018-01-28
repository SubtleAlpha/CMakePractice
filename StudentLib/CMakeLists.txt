cmake_minimum_required(VERSION 2.8.9)
project(directory_test)
set(CMAKE_BUILD_TYPE Release)

#Include headers such as Student.h into the project
include_directories(include)

set(SOURCES src/Student.cpp)

#Generate the shared library from the sources
add_library(student SHARED ${SOURCES})

#Set the location for the library installation.
#Requires calling "sudo make install"
install(TARGETS student DESTINATION /usr/lib)
