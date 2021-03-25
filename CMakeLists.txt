cmake_minimum_required(VERSION 3.0.2)
project(smart_home_launch)

find_package(catkin REQUIRED COMPONENTS
	openni_launch
	smart_home_analg
	smart_home_hub
)

catkin_package(
	CATKIN_DEPENDS openni_launch smart_home_analg smart_home_hub
)

install(
  DIRECTORY launch/
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/launch
)
