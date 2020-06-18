cmake_minimum_required(VERSION 2.8)
project( main )

find_package( OpenCV REQUIRED )
include_directories("./include")
add_executable( main main.cpp feature_descriptor.cpp helper.cpp  hog.c ldmarkmodel.cpp )
target_link_libraries( main ${OpenCV_LIBS} )
