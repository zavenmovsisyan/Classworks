cmake_minimum_required(VERSION 3.20)

project(Hello_world)

add_executable(Hello_world main.cpp)

set_target_properties(
    Hello_world PROPERTIES
    CXX_STANDART 11
    CXX_STANDART_REQUIRED ON
    )

