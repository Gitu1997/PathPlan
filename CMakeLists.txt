cmake_minimum_required(VERSION 2.4.9)
project( opencv )
find_package( OpenCV REQUIRED )

add_executable( PathPlanning src/PathPlanning.cpp )
target_link_libraries( PathPlanning ${OpenCV_LIBS} )
set(CMAKE_BUILD_TYPE Debug)

