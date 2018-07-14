cmake_minimum_required( VERSION 2.8 )
project( useEigen )

set( CMAKE_BUILD_TYPE "Release" )
set( CMAKE_CXX_FLAGS "-O3" )

set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} "${CMAKE_CURRENT_SOURCE_DIR}/cmake/")
find_package(Eigen3 REQUIRED)
include_directories(${EIGEN3_INCLUDE_DIR})

add_executable( eigenMatrix eigenMatrix.cpp )
