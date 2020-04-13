cmake_minimum_required(VERSION 3.15)
project(FullScreenModes)

set(CMAKE_CXX_STANDARD 17)

list(APPEND CMAKE_MODULE_PATH ${CMAKE_CURRENT_SOURCE_DIR}/cmake)

find_package(SDL2 REQUIRED)

add_executable(FullScreenModes src/FullScreenModes/main.cpp)

target_link_libraries(FullScreenModes
    SDL2::SDL2
    )
