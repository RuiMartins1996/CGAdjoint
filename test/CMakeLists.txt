cmake_minimum_required(VERSION 3.10)
project(CGAdjoint)

# Define a variable for the executable name
set(EXECUTABLE_NAME test)

# Define variables for the source and include directories
set(SRC_DIR "${CMAKE_SOURCE_DIR}/src")
set(INCLUDE_DIR "${CMAKE_SOURCE_DIR}/include")


add_subdirectory(lib/Catch2)
# These tests can use the Catch2-provided main
add_executable(${EXECUTABLE_NAME} test.cpp)
target_link_libraries(${EXECUTABLE_NAME} PRIVATE Catch2::Catch2WithMain)
