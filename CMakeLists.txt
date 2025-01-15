cmake_minimum_required(VERSION 2.8.3)
project(cps_msgs)

find_package(catkin REQUIRED)
find_package(catkin REQUIRED COMPONENTS
   roscpp
   rospy
   std_msgs
   message_generation
   message_runtime
)

add_message_files(
  FILES
    EstimatedOdom.msg
	GroupInfo.msg
)


generate_messages(
	DEPENDENCIES
	std_msgs
)

catkin_package(
)

install(DIRECTORY launch
	DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)

