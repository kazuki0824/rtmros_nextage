cmake_minimum_required(VERSION 3.5)
project(nextage_moveit_config)

find_package(ament_cmake REQUIRED)

install(DIRECTORY launch config test
  DESTINATION share/${PROJECT_NAME}
)


if(CATKIN_ENABLE_TESTING)
  find_package(joint_state_publisher REQUIRED)
  find_package(robot_state_publisher REQUIRED)
 # find_package(rostest REQUIRED)

#  add_rostest(test/joy.test)
#  add_rostest(test/nxo_moveit.test)
#  add_rostest(test/moveit_trackik.test)
endif()

ament_package()
