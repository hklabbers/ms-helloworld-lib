cmake_minimum_required (VERSION 3.0)
project(google-test)

set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11 -O0 -g3 -Wall -fmessage-length=0")

add_subdirectory(googlemock)
