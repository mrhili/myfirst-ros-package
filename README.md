# myfirst-ros-package

Steps i followd after creating ros correctly


cd ~/catkin_ws/src/

mkdir mypackage

cd mypackage

touch package.xml

---------------------------Open it & Fill it

You can see her: http://wiki.ros.org/ROS/Tutorials/Creating%20a%20Package%20by%20Hand


-------------------------------

cd ../..

source devel/setup.bash

rospack find mypackage

------OUTPUT: /home/mam/catkin_ws/src/mypackage

cd src/mypackage

touch CMakeLists.txt

-----------------------------Open it & Fill it

cmake_minimum_required(VERSION 2.8.3)
project(mypackage)
find_package(catkin REQUIRED roscpp std_msgs)
catkin_package()

------------------------------------

TIP : WHen you need some required package wich you dont have just run

sudo rosdep init
rosdep update

OR

rosdep resolve <my_dependency_name>








