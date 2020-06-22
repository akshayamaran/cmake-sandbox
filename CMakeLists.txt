#cmake minimum version should be mentioned
cmake_minimum_required(VERSION 3.17)

# set the project name
project(sample)

#include directory
include_directories("dir")


add_executable(sample main.c main.h)