# Homework4

After cloning the repository, build the packages by doing:

     $ colcon build

Then, use the source command:

    $ source install/setup.bash

To launch Gazebo and spawn the robot write the following command in a terminal:

    $ ros2 launch rl_fra2mo_description gazebo_fra2mo.launch.py

To explore the goals as requested in the point 2, in a second terminal write the following command:

    $ ros2 launch rl_fra2mo_description fra2mo_explore.launch.py

If you want to test the point 4 instead, you have to launch in the second terminal the new launch file we created as follows:

    $ ros2 launch rl_fra2mo_description vision_based_navigation.launch.py

In a third terminal write:

    $ ros2 run rl_fra2mo_description follow_waypoints.py

If you want to monitor the robot's movement in RViz, particularly the mapping with the specific configuration required by the task, you can use the following command:

    $ ros2 launch rl_fra2mo_description display_fra2mo.launch.py
