cmake_minimum_required(VERSION 3.21.1)

project(imgui)

set(CMAKE_CXX_STANDARD 20)

add_library(imgui STATIC 
    "imconfig.h"
    "imgui.cpp"
    "imgui.h"
    "imgui_demo.cpp"
    "imgui_draw.cpp"
    "imgui_internal.h"
    "imgui_tables.cpp"
    "imgui_widgets.cpp"
    "imstb_rectpack.h"
    "imstb_textedit.h"
    "imstb_truetype.h"
)

set(CMAKE_CONFIGURATION_TYPES "Debug;Release" CACHE STRING "" FORCE)

target_include_directories(imgui INTERFACE ./)
