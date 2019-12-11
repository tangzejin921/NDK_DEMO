
cmake_minimum_required(VERSION 3.4.1)

add_library(
        bzip2

        SHARED

        blocksort.c
        bzip2.c
        bzip2recover.c
        bzlib.c
        compress.c
        crctable.c
        decompress.c
        huffman.c
        randtable.c
)


