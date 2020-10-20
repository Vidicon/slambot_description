cmake_minimum_required(VERSION 3.0.2)
project(slambot_description)

find_package(catkin
  REQUIRED COMPONENTS
    roslaunch
)

catkin_package(
  CATKIN_DEPENDS
)

# Install directories
install(
  DIRECTORY
    launch
    urdf
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})
