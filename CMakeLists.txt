cmake_minimum_required(VERSION 3.29.0)
project(imgui VERSION 0.1.0 LANGUAGES C CXX)

set(CMAKE_CXX_STANDARD 23)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_library(${PROJECT_NAME} 
  imgui_demo.cpp
  imgui_draw.cpp
  imgui_tables.cpp
  imgui_widgets.cpp
  imgui.cpp
)
target_include_directories(${PROJECT_NAME} PUBLIC .)