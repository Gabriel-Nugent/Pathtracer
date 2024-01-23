cmake_minimum_required(VERSION 3.8)

set(CMAKE_TOOLCHAIN_FILE "c:/vcpkg/scripts/buildsystems/vcpkg.cmake")
set(CMAKE_CXX_STANDARD 20)
project(pathtracer VERSION 0.1 LANGUAGES C CXX)

file(GLOB_RECURSE CPP_FILES ${CMAKE_CURRENT_SOURCE_DIR}/src/*.cpp)
file(GLOB_RECURSE HPP_FILES ${CMAKE_CURRENT_SOURCE_DIR}/src/*.h)

add_executable(app ${CPP_FILES} ${HPP_FILES})