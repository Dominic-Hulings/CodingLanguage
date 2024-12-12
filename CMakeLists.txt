cmake_minimum_required(VERSION 3.10)
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

file(GLOB_RECURSE SRC_FILES src/*.cpp)
file(GLOB_RECURSE INCLUDE_FILES includes/*.h)

include_directories(includes)

project(compiler VERSION 1.0)

add_executable(compiler.o ${SRC_FILES} ${INCLUDE_FILES})