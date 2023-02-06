cmake_minimum_required(VERSION 3.0.2)
project(mecheye_ros_msg)

find_package(catkin REQUIRED std_msgs sensor_msgs message_generation genmsg)

add_service_files(
  DIRECTORY
  srv
)

generate_messages(
  DEPENDENCIES
  std_msgs
  sensor_msgs
)

catkin_package(CATKIN_DEPENDS std_msgs sensor_msgs message_runtime)
