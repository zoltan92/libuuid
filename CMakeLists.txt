cmake_minimum_required(VERSION 3.16.3)

Project(LibUUID)

file(GLOB LUUID_SRCS 
    "uuid.c"
)

add_library(libuuid ${LUUID_SRCS})
message("-- LIBUUID Include: ${CMAKE_CURRENT_SOURCE_DIR}")
target_include_directories(libuuid PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})