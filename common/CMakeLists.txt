# CMake version string
cmake_minimum_required(VERSION 2.8.11)

# Includes
HEADER_DIRECTORIES(COMMON_INCLUDES ${CMAKE_CURRENT_SOURCE_DIR})
set(INCLUDES
    ${INCLUDES}
    ${COMMON_INCLUDES}
PARENT_SCOPE)

# Sources
file(GLOB_RECURSE COMMON_SOURCES "*.cpp" "*.h")
set(SOURCES
    ${SOURCES}
    ${COMMON_SOURCES}
PARENT_SCOPE)
