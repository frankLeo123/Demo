#声明要求cmake的最低版本
cmake_minimum_required(VERSION 2.0)
#工程
project(Demo)
#添加子程序
message(STATUS "this is a cmake in main")
#设置bin和source
include_directories(${CMAKE_CURRENT_SOURCE_DIR}/include)
add_subdirectory(source ${PROJECT_SOURCE_DIR}/bin)
set(EXECUTABLE_OUTPUT_PATH ${PROJECT_BINARY_DIR}/bin)
