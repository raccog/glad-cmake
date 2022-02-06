cmake_minimum_required(VERSION 3.12...3.22)

project(glad VERSION 0.1.35 LANGUAGES C 
    DESCRIPTION "Glad loader for OpenGL 4.6 Core. Includes debug and release versions.")

if (CMAKE_BUILD_TYPE EQUAL "Debug")
    add_subdirectory(glad_debug)
else()
    add_subdirectory(glad_release)
endif()
