##
## Author(s):
##  - Samuel MARTIN <smartin@aldebaran-robotics.com>
##
## Copyright (C) 2012 Aldebaran Robotics

# CMake file for OpenNI
cmake_minimum_required(VERSION 2.8)
project(Primesense-Sensor)
find_package(qibuild)

include_directories(Include)
include_directories(Source)
include_directories(Source/XnCommon)
include_directories(Source/XnCore)
include_directories(Source/XnDDK)
include_directories(Source/XnDeviceFile)
include_directories(Source/XnDeviceSensorV2)
include_directories(Source/XnFormats)

set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -fvisibility=hidden")
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -fvisibility=hidden")

add_subdirectory(Source)
add_subdirectory(Data)
