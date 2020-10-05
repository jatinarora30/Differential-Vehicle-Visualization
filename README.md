## Differential-Vehicle
Differential Drive URDF Simulation Project
This project is made to give a glance of some simple packages of ROS like urdf,rviz, gazebo.As mentioned it is a diffrential drive robot project, this repository has simple urdf and skid steering drive gazebo plugin visualisation.

# Features:
1. It consists of a base body, four wheels and a camera.

2. You can control the robot model in gazebo and rviz using rqt plugin robot-steering.

3. The raw image coming from the camera in the robot can be visualized using rviz camera plugin.

4. You can learn tf by visualizing it in rviz in the model, the rviz file has been configured that to give you a good experience of the working of a mobile robot.

# Further things to be implemented:
1. Addition of laser sensor and visualization of it's sensor messages.

2. Implement Navigation and SLAM in the model and it's visualization in rviz.
# How to implement it:
1. Clone the package to your workspace.

         git clone https://github.com/jatinarora30/Differential-Vehicle-Visualization.git
         
2. Run 

        catkin_make
        
3. Using roslaunch command, run the following commad

        roslaunch project_ws final1.launch


