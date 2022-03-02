cmake_minimum_required(VERSION 3.5)
project(Motor)

add_subdirectory(dynamixel)
add_subdirectory(motor)

add_library(Motor SHARED Dmotor.cpp DmotorMx.cpp DmotorPro.cpp DmotorProPlus.cpp DmotorXm.cpp)
target_link_libraries(Motor DynamixelSdk motor)