roslaunch vmrc_gazebo sandisland.launch 



roslaunch vmrc_gazebo sandisland.launch light_buoy:=false

roslaunch vmrc_gazebo sandisland.launch thrust_config:=X


xx:   
GPS + imu  + 一个相机 + 一个hokuyo激光

roslaunch vmrc_gazebo vmrc.launch 
roslaunch wamv_gazebo localization_example.launch
roslaunch wamv_gazebo rviz_vmrc_xx.launch 
roslaunch vmrc_gazebo usv_keydrive.launch 
rosbag 

no map nav :
roslaunch vmrc_gazebo vmrc.launch 
roslaunch wamv_gazebo localization_example.launch
roslaunch wamv_gazebo rviz_vmrc_xx.launch 
roslaunch vmrc_gazebo usv_vel_trans.launch
roslaunch husky_navigation move_base_mapless_demo.launch

