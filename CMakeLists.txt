cmake_minimum_required(VERSION 3.10)
set(CMAKE_CXX_COMPILER "C:/cmake-3.28.0-rc5-windows-x86_64/bin")
set(CMAKE_C_COMPILER "C:/cmake-3.28.0-rc5-windows-x86_64/bin")

project(tarea)

find_package(OpenCV REQUIRED)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

include_directories(${OpenCV_INCLUDE_DIRS})
add_executable(tarea Main.cpp)
target_link_libraries(TAREA ${OpenCV_LIBS})