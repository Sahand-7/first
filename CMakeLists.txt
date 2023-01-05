cmake_minimum_required(VERSION 3.10.2)

project(OLALA)

add_executable(${PROJECT_NAME} main.c)


add_subdirectory(Adder)

target_include_directories(${PROJECT_NAME} PUBLIC Adder)

link_directories(${PROJECT_NAME} PUBLIC Adder)

target_link_libraries(${PROJECT_NAME} adder)