# Automatic-staining-set-robot
 In this project, a robot was used to automate a manual staining set.

In this project, a robot was used to automate a manual staining set. 
The purpose of the robot is to automate the manual and time-consuming 
immersion of specimen plates in different liquids.The Arduino used in 
this project takes care of controlling the stepper motors, the Python 
code is the brains behind operating the robot, which sends commands to 
the Arduino via serial communication. 

The control of the robot was realized using three Python files. The 
first file "GUI_robot_controls" was generated using Qt Designer and 
provides a control interface for the user. A second file 
"zuurkast_setup" provides visualization in the control interface. 
Also, this file keeps the information about the state of the staining 
set. The third file "gui_robot_zuurkast" is the main program that 
indicates what to do in what situation and provides communication with 
the Arduino.

 ____________
|Controls GUI|
|____________|

Home: Move the robot to the defined mechanical home position to set the 
      zero point.
	  
Stop: Tells the stepper motors to stop executing the current command.
	  
Move X/Y/Z/Gripper: Moves the robot over a specified distance. Moves the gripper arms over a specified distance.

Relative/absolute selection: Used in conjunction with Move X/Y/Z to choose the type of movement. 

Joystick: Allows the use of the joystick to control the robot.

Click on the graph: Robot moves to the position where it was clicked. 

Add new basket to the base station: Adds a basket in the visualization at the base station.

Apply: Have the robot move a basket from position A to position B. 

Clear baskets: removes all baskets in the visualization.

Open/Close Lid: Opens/closes the specified fluid box. 

Make new sequence/edit sequence: An edit mode to create or edit sequences is activated.

Delete sequence: Deletes the specified sequence. 

Simulate sequence: Have the robot execute the specified sequence.

