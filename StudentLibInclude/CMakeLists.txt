cmake_minimum_required(VERSION 2.8.9)
project(TestLibrary)

#For the shared library:
set(PROJECT_LINK_LIBS libstudent.so)
link_directories(~/CMakePractice/StudentLib/build)

include_directories(~/CMakePractice/StudentLib/include)

add_executable(lib lib.cpp)
target_link_libraries(lib ${PROJECT_LINK_LIBS})
