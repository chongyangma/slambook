cmake_minimum_required(VERSION 2.8)
project(slambook)

set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} "${CMAKE_CURRENT_SOURCE_DIR}/cmake/")
find_package(Eigen3 REQUIRED)
include_directories(${EIGEN3_INCLUDE_DIR})

ADD_SUBDIRECTORY(3rdparty)
ADD_SUBDIRECTORY(ch2)
ADD_SUBDIRECTORY(ch3)
