cmake_minimum_required(VERSION 2.8)
project( camera_opencv_sample )
# Debug, Release, RelWithDebInfo and MinSizeRe
set(CMAKE_BUILD_TYPE Debug)
find_package( OpenCV REQUIRED )

add_executable( camera_opencv_sample camera_opencv_sample.cpp )
target_link_libraries( camera_opencv_sample ${OpenCV_LIBS} )
