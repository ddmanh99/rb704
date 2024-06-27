# rb704
My repo run in ros-noetic, ubuntu 20.04

You just need to install folder urg_node

Then, you need to install package "laser_proc" and "urg_c" by command:
    '''
    git clone https://github.com/ros-perception/laser_proc.git
    git clone https://github.com/ros-drivers/urg_c.git
    '''
After that, you make by 'catkin_make'. 

To use lidar hokuyo and visual data in Rviz, you need to run command:
    '''
    source devel/setup.bash
    roslaunch urg_node urg_lidar.launch
    '''