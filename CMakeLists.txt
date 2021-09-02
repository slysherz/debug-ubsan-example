project(test)
cmake_minimum_required(VERSION 3.19)

add_executable(test test.cpp)
target_compile_options(test PRIVATE -fsanitize=undefined)
target_link_options(test PRIVATE -fsanitize=undefined)
