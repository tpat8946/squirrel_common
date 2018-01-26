cmake_minimum_required(VERSION 2.8.3)
project(squirrel_planning_msgs)

find_package(catkin REQUIRED COMPONENTS
  actionlib
  actionlib_msgs
  diagnostic_msgs
)

add_service_files(
  FILES
  CallAction.srv
)

generate_messages(
  DEPENDENCIES
  actionlib_msgs
  diagnostic_msgs
)

catkin_package(
#  INCLUDE_DIRS include
 #  LIBRARIES squirrel_object_perception_msgs
 CATKIN_DEPENDS
    #  DEPENDS system_lib

    actionlib_msgs
    diagnostic_msgs
)
