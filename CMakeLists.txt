cmake_minimum_required(VERSION 3.5)
project(MotorUnion)

add_subdirectory(Motor)

add_library(${PROJECT_NAME} SHARED MotorUnion.cpp)
target_link_libraries(${PROJECT_NAME} Motor)
