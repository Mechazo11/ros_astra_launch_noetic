cmake_minimum_required(VERSION 3.5.0)
project(astra_launch)

find_package(catkin REQUIRED)
find_package(rgbd_launch REQUIRED)
find_package(depth_image_proc REQUIRED)
find_package(image_proc REQUIRED)
find_package(nodelet REQUIRED)
find_package(astra_camera REQUIRED)
find_package(tf REQUIRED)

catkin_package()

# install the launch files
install(DIRECTORY launch/
        DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/launch)

