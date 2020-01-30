//Dependencies
*sudo apt-get install ros-(ROS version name)-cv-bridge
* pip install opencv-python==3.1.0 


//How to run
*	Unzip the catkin_ws file 
*	run catkin_make inside the "catkin_ws" directory
*	source /devel/setup.sh
*	"roslaunch rosbot_description  rosbot.launch" to launch gazebo
*	"rosrun devrim_pkg devrim_pkg_node" to start the laser_scan node
*	"rosrun devrim_pkg sign.py" to start the sign detector node
*	"rosrun devrim_pkg motor_control.py" to start the motor controller
(Python file should be executable run chmod u+x <filename>.py if needed)

//Incase any error on "roslaunch rosbot_description rosbot.launch"
edit the asgard.sdf under /catkin_ws/src/rosbot_description/src/rosbot_gazebo/worlds
replace all "gurbuz" with your username 


//Optional View camera
rosrun image_view image_view image:=/camera/rgb/image_raw

//Our Demo Video
https://www.youtube.com/watch?v=kr4oyFGjZic&feature=youtu.be
