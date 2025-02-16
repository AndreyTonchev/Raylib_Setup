cmake_minimum_required(VERSION 3.10)

project(MyProject)

set(CMAKE_BUILD_TYPE Debug)

set(CMAKE_TOOLCHAIN_FILE "C:/vcpkg/scripts/buildsystems/vcpkg.cmake" CACHE STRING "")

find_package(raylib CONFIG REQUIRED) 

add_executable(MyProject main.cpp)

target_link_libraries(MyProject PRIVATE raylib)