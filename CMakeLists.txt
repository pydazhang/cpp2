cmake_minimum_required(VERSION 3.15.0)
project(demo VERSION 0.1.0)

INCLUDE_DIRECTORIES(
    c:/vcpkg/vcpkg/installed/x64-windows/include
)
  
LINK_DIRECTORIES(
    c:/vcpkg/vcpkg/installed/x64-windows/lib
)

add_executable(demo main.cpp)
TARGET_LINK_LIBRARIES(demo 
matplot nodesoup)

target_compile_features(demo PUBLIC cxx_std_17)
