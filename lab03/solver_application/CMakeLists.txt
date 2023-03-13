cmake_minimum_required(VERSION 3.2)

project (equation)

include_directories(solver_lib formatter_ex_lib)
add_subdirectory(solver_lib)
add_subdirectory(formatter_ex_lib)

add_executable(equation equation.cpp)
target_link_libraries(equation solver_lib formatter_ex_lib)