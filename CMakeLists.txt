cmake_minimum_required(VERSION 2.8.12)
project(mitlm)
ADD_DEFINITIONS(
    -std=c++11 # Or -std=c++0x
    -DPACKAGE_STRING="MITLM CMake custom build"
    -Ofast
)
enable_language (C Fortran)
file(GLOB f_sources src/optimize/*.f)
file(GLOB sources src/*/*.cpp src/*/*.cpp src/*.cpp)
file(GLOB to_remove src/*-ngram.cpp)
list(REMOVE_ITEM sources ${to_remove})

add_library(mitlm SHARED ${f_sources} ${sources})
target_include_directories(mitlm PUBLIC src)
target_link_libraries(mitlm gfortran)

add_executable(interpolate-ngram src/interpolate-ngram.cpp)
target_link_libraries(interpolate-ngram gfortran mitlm)
target_include_directories(interpolate-ngram PUBLIC src)

add_executable(estimate-ngram src/estimate-ngram.cpp)
target_link_libraries(estimate-ngram gfortran mitlm)
target_include_directories(estimate-ngram PUBLIC src)

add_executable(evaluate-ngram src/evaluate-ngram.cpp)
target_link_libraries(evaluate-ngram gfortran mitlm)
target_include_directories(evaluate-ngram PUBLIC src)