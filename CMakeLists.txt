cmake_minimum_required(VERSION 3.0.2)
project(rosbag_to_csv)

find_package(catkin REQUIRED COMPONENTS
  rospy
)

catkin_package()

catkin_install_python(PROGRAMS
  scripts/rosbag_to_csv.py
  scripts/SimplePyQtGUIKit.py # temporary until properly packaged...
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)
