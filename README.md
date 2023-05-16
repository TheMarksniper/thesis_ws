# thesis_ws
Master thesis of Marek Raska

litlle helpers
colcon build
source install/setup/bash
ros2 launch box_bot_gazebo multi_box_bot_launch.py
-----supression of wno-dev error----------
colcon build --symlink-install --packages-select box_bot_gazebo --cmake-args -Wno-dev
-----------------------------------------

ros2 run teleop_twist_keyboard teleop_twist_keyboard --ros-args --remap cmd_vel:=/linorobot_x000_y000/cmd_vel

-------Lunch with gazebo paused-------------------------------------

ros2 launch box_bot_gazebo multi_box_bot_launch.py pause:=true
