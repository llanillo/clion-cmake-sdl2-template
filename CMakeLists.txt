cmake_minimum_required(VERSION 3.22)
project(NAME_PROJECT)

set(CMAKE_CXX_STANDARD 14)

add_executable(NAME_PROJECT main.cpp)

# --- SDL2 SETUP ---
find_package(SDL2 REQUIRED)
include_directories( ${SDL2_INCLUDE_DIR} )
target_link_libraries(NAME_PROJECT ${SDL2_LIBRARY})
