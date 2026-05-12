cmake_minimum_required(VERSION 3.22.1)

project(cpp)
add_library(cpp cal.cpp)

set_target_properties(cpp PROPERTIES PUBLIC_HEADER cal.h)
install(TARGETS cpp LIBRARY DESTINATION cpp
        PUBLIC_HEADER DESTINATION include)