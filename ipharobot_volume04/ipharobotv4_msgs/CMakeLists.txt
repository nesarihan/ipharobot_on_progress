cmake_minimum_required(VERSION 3.0.2)
project(ipharobotv4_msgs)

find_package(catkin REQUIRED COMPONENTS
  std_msgs
  message_generation
)

add_message_files(FILES
  SensorState.msg
  Sound.msg
  VersionInfo.msg
)

generate_messages(DEPENDENCIES
  std_msgs
)


catkin_package(
  CATKIN_DEPENDS 
  std_msgs 
  message_runtime
)

include_directories(
# include
  ${catkin_INCLUDE_DIRS}
)

