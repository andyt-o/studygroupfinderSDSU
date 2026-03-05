cmake_minimum_required(VERSION 3.15)
project(studyGroupFinder_Workspace VERSION 0.0.1 LANGUAGES C CXX)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(fmt CONFIG REQUIRED)

add_subdirectory(packages/core)