cmake_minimum_required(VERSION 3.5)

project(hello_world)

include_directories(hello_world /home/inspired/T_lb3/hello_world_application)

include_directories(hello_world /home/inspired/T_lb3/formatter_ex_lib)

include_directories(hello_world /home/inspired/T_lb3/formatter_lib)

add_library(hello_world STATIC hello_world.cpp)

target_link_libraries(hello_world PUBLIC /home/inspired/T_lb3/formatter_ex_lib/formatter_ex.cpp)

target_link_libraries(hello  PUBLIC /home/inspired/T_lb3/formatter_lib/formatter.cpp)

target_link_libraries(hello_world /home/inspired/T_lb3/formatter_ex_lib/_build/libformatter_ex.a)

target_link_libraries(hello /home/inspired/T_lb3/formatter_lib/_build/libformatter.a)

