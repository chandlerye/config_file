cmake_minimum_required(VERSION 3.0)
project(main)
set(CMAKE_CXX_STANDARD 11)
# set(OpenCV_DIR C:\\Users\\chandler\\Documents\\source_code\\build\\buildcv45\\install)
find_package(OpenCV REQUIRED)
add_executable(${PROJECT_NAME} "example.cpp")
include_directories(${OpenCV_INCLUDE_DIRS})
target_link_libraries(${PROJECT_NAME} ${OpenCV_LIBS})
