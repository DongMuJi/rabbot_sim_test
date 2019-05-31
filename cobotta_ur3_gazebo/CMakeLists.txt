cmake_minimum_required(VERSION 2.8.3)
project(cobotta_ur3_gazebo)

find_package(catkin REQUIRED)

catkin_package()

#############
## Install ##
#############

# other files
foreach(dir launch worlds controller)
   install(DIRECTORY ${dir}
      DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})
endforeach()
