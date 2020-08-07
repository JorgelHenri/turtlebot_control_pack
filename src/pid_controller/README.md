---------------ORIGINAL PROJECT---------------
# ROS-TurtleBot-PID
This project demonstrates the simulation of ROS Turtlebot3 path tracking with PID. I have generalized the pid controller to track circular or linear trajectories.
Here is the youtube [video](https://youtu.be/okqIgZJy67E).

---------------MODIFICATION---------------
In this project I apply a file that has all the positions of my path, this is the base for the PID generate all the vectors.

---------------HOW TO START---------------
 - Create a catkin workspace
 - Clone this pack in src directory, with the command $git clone ...
 - Use the command $ catkin_make, to compile the pack
 - Start the pack using $ roslaunch pid_controller2 control.launch
 - With you have a rviz launching, add a Maker to vizualize the path.
