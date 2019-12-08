cmake_minimum_required(VERSION 3.1)
project(HSVDetection)

find_package(OpenCV REQUIRED)
set(CMAKE_CXX_STANDARD 14)

INCLUDE_DIRECTORIES(${OpenCV_DIRS})



add_executable(HSVDetection main.cpp)

TARGET_LINK_LIBRARIES(HSVDetection ${OpenCV_LIBS})