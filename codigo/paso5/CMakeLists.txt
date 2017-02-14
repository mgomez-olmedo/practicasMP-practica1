
cmake_minimum_required(VERSION 2.8.9)
project(principal)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "bin/")

#Bring the headers, such as Student.h into the project
include_directories(include)

#However, the file(GLOB...) allows for wildcard additions:
file(GLOB SOURCES "src/*.cpp")

add_executable(principal ${SOURCES})

