cmake_minimum_required(VERSION 2.8)

project(Lazy)

set(OUTPUTNAME Lazy)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall -g -O2 -std=c++11")

include_directories($ENV{BOOST_INCLUDE_PATH})

link_directories($ENV{BOOST_LIB_PATH})

aux_source_directory(. DIR_SRCS)
add_executable(${OUTPUTNAME} ${DIR_SRCS})

