cmake_minimum_required(VERSION 3.6)
project(GiBUU)
enable_language(Fortran)

set(CMAKE_Fortran_FLAGS "${CMAKE_Fortran_FLAGS} -cpp -fdefault-real-8 -fdefault-double-8 -ffree-line-length-none -fbounds-check -fbacktrace -fcheck=all")

add_subdirectory(code)