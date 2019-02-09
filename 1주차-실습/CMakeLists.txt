project(opencv_test)

set (CMAKE_CXX_STANDARD 11)
cmake_minimum_required(VERSION 2.8)
find_package( OpenCV REQUIRED )
 
file(GLOB SOURCES  *.cpp)
 
add_executable("Example_001(webcam)" "Example_001(webcam).cpp" )
target_link_libraries( "Example_001(webcam)" ${OpenCV_LIBS} )