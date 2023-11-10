cmake_minimum_required (VERSION 3.17)

project(dyn_b_suitor_comp CXX)

set(CMAKE_CXX_STANDARD 17)

link_directories(/usr/local/lib)

add_executable(dyn_b_suitor_comp
    main.cpp
)

# Link against the installed Networkit library
target_link_libraries(dyn_b_suitor_comp
    PRIVATE networkit
)

