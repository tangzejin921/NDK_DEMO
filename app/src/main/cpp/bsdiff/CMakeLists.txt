cmake_minimum_required(VERSION 3.4.1)

ADD_SUBDIRECTORY(bzip2)

#==============================
add_library(
        bsdiff

        SHARED

        bsdiff.c
)
target_link_libraries(
        bsdiff

        bzip2)
#==============================
add_library(
        bspatch

        SHARED

        bspatch.c
)
target_link_libraries(
        bspatch

        bzip2)
#==============================


