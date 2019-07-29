cmake_minimum_required(VERSION 2.8.3)
project(turtlebot_teleop)

## Find catkin macros and libraries
find_package(catkin REQUIRED COMPONENTS roscpp geometry_msgs joy)

include_directories(${catkin_INCLUDE_DIRS})

catkin_package(
  INCLUDE_DIRS
  CATKIN_DEPENDS roscpp geometry_msgs joy
  DEPENDS
)



#############
## Install ##
#############

## Mark all other useful stuff for installation
install(DIRECTORY launch config
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
