THAT PACKAGE IS FOR RUN THE TURTLEBOT IN A ENVAIORMENT
GIT FOR THE TURTLEBOT 2 : https://github.com/gaunthan/Turtlebot2-On-Melodic
   INSTALLING THE PACKAGE USING
   - create a workspace catkin
   - made a git clone of this folder
   - copy the folder map_filed (in this folder)
   - paste the folder in your .gazebo at home directory (this folder is hidden)
   - update your source by 
      $ source devel/setup.bash
   - run 
      $ roslaunch turtlebot_fieldpath turtle_arena.launch


      $ roslaunch turtlebot_gazebo amcl_demo.launch map_file:=FILE_DIRECTORY/turtlebot_control_pack/src/turtlebot_fieldpath/map_field3/map_entregavel3.yaml

      PS: This last command line is for load the map with amcl program.

