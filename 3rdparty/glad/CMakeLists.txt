cmake_minimum_required (VERSION 3.5)
project (glad C)

file(GLOB HEADERS "include/glad.h")
set(SRC "src/glad.c")

add_library(glad STATIC ${HEADERS} ${SRC})
target_include_directories(glad PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}/include")
