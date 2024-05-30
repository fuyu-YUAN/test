cmake_minimum_required(VERSION 3.0.2)
project(parameter_manager)

find_package(catkin REQUIRED COMPONENTS
  roscpp
  rospy
  std_msgs
  std_srvs
)


add_executable(para_config src/para_config.cpp)
target_link_libraries(para_config ${catkin_LIBRARIES})

catkin_package(
)


include_directories(
# include
  ${catkin_INCLUDE_DIRS}
)

