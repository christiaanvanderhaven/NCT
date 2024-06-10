cmake_minimum_required(VERSION 3.0.0)
project(NCT VERSION 0.1.0 LANGUAGES C CXX)

add_executable(NCT main.cpp glad.c)

add_subdirectory(./include/glfw)
add_subdirectory(./include/imgui)

include_directories(./include)

target_link_libraries(NCT glfw imgui)
