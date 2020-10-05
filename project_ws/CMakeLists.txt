cmake_minimum_required(VERSION 3.0.2)
project(project_ws)

## Compile as C++11, supported in ROS Kinetic and newer
# add_compile_options(-std=c++11)

## Find catkin macros and libraries
## if COMPONENTS list like find_package(catkin REQUIRED COMPONENTS xyz)
## is used, also find other catkin packages
find_package(catkin REQUIRED COMPONENTS
  roscpp
  rospy
  std_msgs
  diff_drive_controller
  controller_manager
  cv_bridge 
  image_transport 
 	
 
)

find_package(OpenCV REQUIRED)

catkin_package()

include_directories(
  ${catkin_INCLUDE_DIRS}
  ${OpenCV_INCLUDE_DIRS}
)

add_executable(image_converter src/image_converter.cpp)

target_link_libraries(image_converter ${catkin_LIBRARIES} ${OpenCV_LIBS})

