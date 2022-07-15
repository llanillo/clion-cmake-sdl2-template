cmake_minimum_required(VERSION 3.22)
project(PROJECT_NAME)

set(CMAKE_CXX_STANDARD 14)

add_executable(${PROJECT_NAME} main.cpp)

# --- SDL2 SETUP ---
find_package(${PROJECT_NAME} REQUIRED)
include_directories( ${SDL2_INCLUDE_DIR} )
target_link_libraries(${PROJECT_NAME} ROJECT ${SDL2_LIBRARY})
