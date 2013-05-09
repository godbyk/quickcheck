
cmake_minimum_required(VERSION 2.8.2)

# Set package properties
project(quickcheck)

# Search CMakeModules/ subdir for cmake modules
list(APPEND CMAKE_MODULE_PATH ${CMAKE_SOURCE_DIR}/CMakeModules)

# Enable loads of warnings
include(EnableExtraCompilerWarnings)

# Compile with C++11
include(EnableCXX11)

###
# Build the project
###

include_directories(.)
add_executable(tests tests.cc)
add_executable(examples examples.cc)


###
# End project build
###

