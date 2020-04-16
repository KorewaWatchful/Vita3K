cmake_minimum_required (VERSION 3.6.0)

set (PROJECT libzRIF)
project (${PROJECT})

add_library(${PROJECT} STATIC include/zRIF/keyflate.h
                              include/zRIF/licdec.h
                              include/zRIF/rif.h
                              src/keyflate.c
                              src/licdec.cpp)

include_directories(${ZLIB_INCLUDE_DIR})
include_directories(include)
