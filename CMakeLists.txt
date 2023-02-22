cmake_minimum_required(VERSION 3.14)
project(main CXX)
set(CMAKE_CXX_STANDARD 17)

add_executable(main main.cpp)

find_package(open62541 1.2.3)

target_link_libraries(main PRIVATE open62541::open62541)