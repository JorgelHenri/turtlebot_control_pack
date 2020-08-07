This package is for put a turtlebot2 in a "labyrinth" envarioment, and inicialize a path for the robot follow.

---------------HOW TO START---------------
 - Install all the package following the readme in each one.
 - After that use this commands to start all:
 - $ roslaunch turtlebot_fieldpath turtle_arena.launch
 - $ roslaunch turtlebot_gazebo amcl_demo.launch map_file:=FILE_DIRECTORY/turtlebot_control_pack/src/turtlebot_fieldpath/map_field3/map_entregavel3.yaml
 - $ roslaunch turtlebot_rviz_launchers view_robot.launch
 - $ roslaunch pid_controller2 control.launch
 - In the rviz add the maker to see the path
 - The labrynth model are without collision
