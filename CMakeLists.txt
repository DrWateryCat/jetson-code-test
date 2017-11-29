cmake_minimum_required(VERSION 2.6)

project(jetson-code-test CXX)

set( PROJECT "jetson-code-test" )

include_directories("${PROJECT_SOURCE_DIR}")
include_directories("${PROJECT_SOURCE_DIR}/include")

set( CMAKE_CPP_FLAGS "-Wall" )

file( GLOB MAIN_SOURCES src/*.cpp )

add_executable( ${PROJECT} ${MAIN_SOURCES} )

set( CMAKE_COMPILE_FLAGS ${CMAKE_C_FLAGS})
