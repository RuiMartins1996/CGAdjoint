cmake_minimum_required(VERSION 3.10)
project(CGAdjoint)

# Set the C++ standard
set(CMAKE_CXX_STANDARD 11)

# Define a variable for the executable name
set(EXECUTABLE_NAME executable)

# Define variables for the source and include directories
set(SRC_DIR "${CMAKE_SOURCE_DIR}/src")
set(INCLUDE_DIR "${CMAKE_SOURCE_DIR}/include")

# Add the executable
add_executable(${EXECUTABLE_NAME} src/main.cpp)
