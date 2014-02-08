cmake_minimum_required(VERSION 2.8)
project(AntTweakBar)

set(LIBRARY_OUTPUT_PATH ${CMAKE_SOURCE_DIR}/lib)
set(EXECUTABLE_OUTPUT_PATH ${CMAKE_SOURCE_DIR}/bin)

include_directories(
	include
)

file(GLOB_RECURSE SOURCES src/*.cpp)

ADD_DEFINITIONS(-D_UNIX)
	 
add_library(AntTweakBar ${SOURCES})
target_link_libraries(AntTweakBar GL)

Option(AntTweakBar_BUILD_EXAMPLES "Build the AntTweakBarexample programs" ON)
if (AntTweakBar_BUILD_EXAMPLES)
    add_subdirectory(examples) 
endif()

