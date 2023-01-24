cmake_minimum_required(VERSION 3.10)
project(SecondOrder)

set(HEADER_FILES    
    secondorder.h
)
set(SOURCES_FILES    
    secondorder.cpp
)

add_library(SecondOrder
    STATIC
    ${HEADER_FILES}
    ${SOURCES_FILES}
)
target_include_directories(SecondOrder 
    PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR} 
)