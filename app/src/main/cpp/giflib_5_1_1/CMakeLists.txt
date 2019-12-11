cmake_minimum_required(VERSION 3.4.1)
#project(giflib_5_2_1 C)

set(CMAKE_C_STANDARD 11)

#include_directories(.)

# 解决 NO_SONAME 问题
#set_property(TARGET your_imported_lib PROPERTY IMPORTED_NO_SONAME 1)

add_library(giflib_5.1.1

        SHARED

        config.h
        dgif_lib.c
        egif_lib.c
        gif_err.c
        gif_font.c
        gif_hash.c
        gif_hash.h
        gif_lib.h
        gif_lib_private.h
        gifalloc.c
        openbsd-reallocarray.c
        quantize.c)
