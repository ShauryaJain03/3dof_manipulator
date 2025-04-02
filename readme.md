3 DOF Manipulator

Running and viewing URDF without any launch file in project -
ros2 launch urdf_tutorial display.launch.py model:=/home/shaurya/manipulator_ws/src/description/urdf/robot.urdf.xacro

Use launch file display.launch.py to view the urdf in rviz2
ros2 launch description display.launch.py

launch gazebo simulation - 
ros2 launch description gazebo.launch.py

launch controllers - 
ros2 launch controller controller.launch.py

sending message to gripper - 
ros2 topic pub /gripper_controller/commands std_msgs/msg/Float64MultiArray "layout:
  dim: []
  data_offset: 0
data: [-1]"