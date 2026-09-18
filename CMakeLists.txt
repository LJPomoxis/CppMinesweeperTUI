cmake_minimum_required(VERSION 3.21)
project(my_project LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_subdirectory(core-engine)

add_executable(minesweeperTUI
    main.cpp
)

target_link_libraries(minesweeperTUI PRIVATE core_engine)