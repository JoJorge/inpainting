cmake_minimum_required(VERSION 2.8)
project(Inpainting)

find_package( OpenCV REQUIRED )
include_directories( ${OpenCV_INCLUDE_DIRS} )
include_directories( ${PROJECT_SOURCE_DIR} )
#add_library( Utility utils.cpp)

add_executable( Inpainting main.cpp utils.cpp )
target_link_libraries( Inpainting ${OpenCV_LIBS} )
#target_link_libraries( Inpainting Utility )
