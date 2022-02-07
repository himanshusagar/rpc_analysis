cmake_minimum_required(VERSION 3.16)
project(rpc_analysis)

find_package(gRPC CONFIG REQUIRED)
find_package(Protobuf CONFIG REQUIRED)

set(CMAKE_CXX_STANDARD 17)

include_directories(include)
file(GLOB SOURCES "src/*.cpp")

add_executable(rpc_analysis ${SOURCES})
