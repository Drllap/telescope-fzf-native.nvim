cmake_minimum_required(VERSION 3.16 FATAL_ERROR)
project(TelescopeFzfNative C)

add_library(fzf SHARED)

target_sources(fzf
  PRIVATE
    src/fzf.h
    src/fzf.c
)

install(TARGETS fzf DESTINATION ${PROJECT_BINARY_DIR})

