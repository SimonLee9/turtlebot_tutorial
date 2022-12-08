# turtlebot_tutorial
source : https://emanual.robotis.com/docs/en/platform/turtlebot3/basic_examples/#position-control

## Turn On

 - keyboard

    export TURTLEBOT3_MODEL=${TB3_MODEL}
    roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch

    export TURTLEBOT3_MODEL=burger
    roslaunch turtlebot3_gazebo turtlebot3_world.launch
    

## 1. Obstacle Detection by lidar

    roslaunch turtlebot3_example turtlebot3_obstacle.launch
    
## 2. Postion operation
The TurtleBot3 can be moved by 2D point (x, y) and z-angular. For example, if you insert (0.5, 0.3, 60), TurtleBot3 moves to point (x = 0.5m, y = 0.3m) and then rotates 60 deg.


    roslaunch turtlebot3_example turtlebot3_pointop_key.launch


## 3. Patrol

    rosrun turtlebot3_example turtlebot3_server
    
    roslaunch turtlebot3_example turtlebot3_client.launch
