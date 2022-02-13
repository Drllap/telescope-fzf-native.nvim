cmake_minimum_required(VERSION 3.22 FATAL_ERROR)
project(TelescopeFzfNative C)

add_library(libfzf SHARED)

target_sources(libfzf
  PRIVATE
    src/fzf.h
    src/fzf.c
)

install(TARGETS libfzf DESTINATION ${PROJECT_BINARY_DIR})

