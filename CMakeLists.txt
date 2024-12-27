cmake_minimum_required(VERSION 3.31)

project(another-pong 
VERSION 1.0 
DESCRIPTION "A clone of pong made using SDL2"
LANGUAGES CXX)

add_executable(another-pong 
src/main.cpp)

find_package(SDL2 REQUIRED)
target_link_libraries(another-pong ${SDL2_LIBRARIES})


