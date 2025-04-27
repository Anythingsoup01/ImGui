cmake_minimum_required(VERSION 3.30)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
project(ImGui-Prebuild LANGUAGES CXX)
set(SRCS
    imconfig.h
    imgui.h
    imgui.cpp
    imgui_draw.cpp
    imgui_internal.h
    imgui_tables.cpp
    imgui_widgets.cpp
    imstb_rectpack.h
    imstb_textedit.h
    imstb_truetype.h
    imgui_demo.cpp
)
add_library(ImGui STATIC ${SRCS})
set_property(TARGET ImGui PROPERTY CXX_STANDARD 17)

