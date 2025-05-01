# Checkpoint18 Dijkstra_path_planning

This is part of the construct's checkpoint 18. To change Nav2 behavior to do Djikstra path planning.
Straightline path planner also provided by the construct for reference.

djikstra.ipynb file is my python recheck.

Run on Ros2 Galactic

-  Terminal 1

```
export MY_ROBOT=mp_400; export MAP_NAME=neo_track1
export GAZEBO_MODEL_PATH=/home/peerajak/ros2_ws/src/path_planning_checkpoint/neo_simulation2/models:/home/peerajak/ros2_ws/src:/home/peerajak/ros2_ws/src/neobotix_ros2
cd ~/ros2_ws && colcon build && source install/setup.bash
ros2 launch neo_simulation2 simulation.launch.py
```

- Terminal 2

```
export GAZEBO_MODEL_PATH=/home/peerajak/ros2_ws/src/path_planning_checkpoint/neo_simulation2/models:/home/peerajak/ros2_ws/src:/home/peerajak/ros2_ws/src/neobotix_ros2
cd ~/ros2_ws && colcon build && source install/setup.bash
ros2 launch neo_nav2 neo_nav2_full.launch.xml
```

