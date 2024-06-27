# rb704
My repo run in ros-noetic, ubuntu 20.04.

## LiDAR HOKUYO
If you want to use lidar hokuyo, you just need to install folder urg_node.

Then, you need to install package "laser_proc" and "urg_c" by command:
    
    git clone https://github.com/ros-perception/laser_proc.git
    git clone https://github.com/ros-drivers/urg_c.git

After that, you make by 'catkin_make'. 

To use lizar hokuyo and visual data in Rviz, you need to run command:

    source devel/setup.bash
    roslaunch urg_node urg_lidar.launch

## Camera Realsense
If you want to use and visual data in Rviz, you need to run command: 

    source devel/setup.bash
    roslaunch realsense2_camera demo_t265.launch

You can set params of camera in 'rs_t265.launch': 'enable_fisheye' to visual fisheye image, 'enable_sync', ... 