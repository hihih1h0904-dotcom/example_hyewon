# example_hyewon
키보드로 조작하고 장애물 감지 시 후진 및 우회전

1 Terminal
ros2 launch storagy bringup.launch.py

2 Terminal
colcon build --symlink-install
source install/setup.bash
ros2 run project hw_node

3 Terminal
ros2 run teleop_twist_keyboard teleop_twist_keyboard --ros-args --remap cmd_vel:=key_vel
