project( camera_opencv_sample )
cmake_minimum_required(VERSION 2.8)
# Debug, Release, RelWithDebInfo and MinSizeRe
set(CMAKE_BUILD_TYPE RelWithDebInfo)
SET(CMAKE_VERBOSE_MAKEFILE ON)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall -Wextra") # add extra warnings

find_package( OpenCV REQUIRED )

add_executable( camera_opencv_sample camera_opencv_sample.cpp )
target_link_libraries( camera_opencv_sample ${OpenCV_LIBS} )
