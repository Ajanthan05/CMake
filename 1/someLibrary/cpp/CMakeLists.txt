cmake_minimum_required(VERSION 3.22.1)

project(ajmath)
add_library(ajmath cal.cpp)

set_target_properties(ajmath PROPERTIES PUBLIC_HEADER cal.h)
install(TARGETS ajmath LIBRARY DESTINATION lib
        PUBLIC_HEADER DESTINATION include/aj)