
cmake_minimum_required(VERSION 2.8)
project(rosmon)

find_package(catkin)

catkin_package()

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11 -Werror")

catkin_install_python(
	PROGRAMS src/rosmon
	DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)
