## How to use
### Install
clone this repository in your workspace.
```shell
git clone git@github.com:DeanKH/ft_sensor_gazebo_sample.git
```

### Run
run following command in your terminal. 
```shell
roslaunch ft_sensor_gazebo_sample robot_gazebo.launch
```

Gazebo publish force/torque sensor data named */ftsensor/raw*.
Message type is *geometry_msgs/WrenchStamped*. 

The default sensor data contain gravity force about end effector.

To get reaction force, drive linear joint, *base_to_arm_joint*.
This joint can drive through ros_control, EfforctController.
publish Float64 scalar value to the topic */simple_bot/linear_joint_position_controller*.




