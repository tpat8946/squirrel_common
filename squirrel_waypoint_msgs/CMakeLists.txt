cmake_minimum_required(VERSION 2.8.3)
project(squirrel_waypoint_msgs)

## Find catkin macros and libraries
find_package(catkin REQUIRED COMPONENTS
  message_generation
<<<<<<< HEAD
  diagnostic_msgs
  geometry_msgs
=======
  squirrel_object_perception_msgs
>>>>>>> upstream/indigo_dev
  std_msgs
)

## Generate services in the 'srv' folder
add_service_files(
  FILES
  ManipulationWaypointService.srv
  ExamineWaypoint.srv
)

## Generate added messages and services with any dependencies listed here
generate_messages(
<<<<<<< HEAD
   DEPENDENCIES
   diagnostic_msgs
   geometry_msgs
   std_msgs
=======
  DEPENDENCIES
  geometry_msgs
  squirrel_object_perception_msgs
  std_msgs
>>>>>>> upstream/indigo_dev
)

## Declare a catkin package
catkin_package(
<<<<<<< HEAD
   CATKIN_DEPENDS 
  message_runtime 
  std_msgs 
  geometry_msgs
  diagnostic_msgs
=======
#  INCLUDE_DIRS include
 #  LIBRARIES squirrel_object_perception_msgs
 CATKIN_DEPENDS
    #  DEPENDS system_lib

    geometry_msgs
    squirrel_object_perception_msgs
    message_runtime
    std_msgs
>>>>>>> upstream/indigo_dev
)

###########
## Build ##
###########

include_directories(
  ${catkin_INCLUDE_DIRS}
)
