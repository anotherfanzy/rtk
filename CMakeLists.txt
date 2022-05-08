cmake_minimum_required(VERSION 3.0)

project(POSDEMO)

aux_source_directory(${PROJECT_SOURCE_DIR}/src SRC)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/bin)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -g -Wall -o2")
set(CMAKE_BUILD_TYPE "Debug")

include_directories(${PROJECT_SOURCE_DIR}/include)

add_executable(main main.cpp ${SRC})