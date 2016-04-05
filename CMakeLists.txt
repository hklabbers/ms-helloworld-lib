cmake_minimum_required (VERSION 3.0)
project(ms-helloworld)

set (CMAKE_VERBOSE_MAKEFILE ON)
set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11 -O0 -g3 -Wall -fmessage-length=0")

# Poco libraries used by this project
set(POCO PocoFoundation PocoNet)

# Build gtest and googlemock
add_subdirectory(test)

# Build the microserver hello world library
add_subdirectory(ms-helloworld-lib)

