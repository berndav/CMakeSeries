cmake_minimum_required(VERSION 3.23)
project(HelloApp
        VERSION 0.0.1
        DESCRIPTION "The leading world app"
        LANGUAGES CXX)

add_compile_options("$<$<C_COMPILER_ID:MSVC>:/utf-8>")
add_compile_options("$<$<CXX_COMPILER_ID:MSVC>:/utf-8>")
        
add_executable(HelloAppBinary main.cpp)
target_compile_features(HelloAppBinary PRIVATE cxx_std_20)