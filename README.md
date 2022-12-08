# turtlebot_tutorial_simulation

source : 

    https://emanual.robotis.com/docs/en/platform/turtlebot3/basic_examples/#position-control
    https://www.youtube.com/watch?v=Xg1pKFQY5p4

## Turn On
  
 - gazebo(world)
---
    export TURTLEBOT3_MODEL=burger (option : burger / waffle / waffle_pi)
    roslaunch turtlebot3_gazebo turtlebot3_empty_world.launch (option1)
    roslaunch turtlebot3_gazebo turtlebot3_world.launch (option2)
    roslaunch turtlebot3_gazebo turtlebot3_house.launch (option3)
    
 - rviz
---
     roslaunch turtlebot3_gazebo turtlebot3_gazebo_rviz.launch
     
 - keyboard
---
    export TURTLEBOT3_MODEL=${TB3_MODEL} (option : burger / waffle / waffle_pi)
    roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch 
    
## 1. Obstacle Detection by lidar

    roslaunch turtlebot3_example turtlebot3_obstacle.launch
    
## 2. Postion operation
The TurtleBot3 can be moved by 2D point (x, y) and z-angular. For example, if you insert (0.5, 0.3, 60), TurtleBot3 moves to point (x = 0.5m, y = 0.3m) and then rotates 60 deg.


    roslaunch turtlebot3_example turtlebot3_pointop_key.launch


## 3. Patrol

    rosrun turtlebot3_example turtlebot3_server
    
    roslaunch turtlebot3_example turtlebot3_client.launch
