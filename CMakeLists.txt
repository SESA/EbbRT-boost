cmake_minimum_required(VERSION 2.6)

# This must be before the project() command so cmake finds our platform
# definition
list(APPEND CMAKE_MODULE_PATH "${CMAKE_CURRENT_LIST_DIR}/../../cmake")

project(Boost NONE)

install(DIRECTORY ${CMAKE_SOURCE_DIR}/include/boost DESTINATION include
  FILES_MATCHING PATTERN "*.hpp")
