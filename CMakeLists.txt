cmake_minimum_required(VERSION 2.6)
project(kevtest)
include_directories("/usr/local/include")
find_package( OpenCV REQUIRED )

add_executable(kevtest main.cpp)

install(TARGETS kevtest RUNTIME DESTINATION bin)
target_link_libraries( kevtest  ${OpenCV_LIBS} )
