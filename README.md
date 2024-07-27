# Robot-ARM
- here you can fine the files after editing on the the Arduino_robot_arm.urdf file and maximize the angle of the elbpw joint






Steps of robot arm Task :

I used the codes from @smart methods github account
```ruby
$ cd ~/catkin_ws/src

$ sudo apt install git

$ git clone:  https://github.com/smart-methods/arduino_robot_arm
```


Second:

I creating a workspace for catkin by using this codes
```ruby
$ mkdir -p ~/catkin_ws/src

$ cd ~/catkin_ws/

$ catkin_make
```

Then I make sure that these functions exist or install them again using the following codes:

```ruby
$ cd ~/catkin_ws

$ rosdep install --from-paths src --ignore-src -r -y

$ sudo apt-get install ros-melodic-moveit

$ sudo apt-get install ros-melodic-joint-state-publisher ros-melodic-joint-state-publisher-gui

$ sudo apt-get install ros-melodic-gazebo-ros-control joint-state-publisher

$ sudo apt-get install ros-melodic-ros-controllers ros-melodic-ros-control
```

Third:

I can lunch the backage by using this codes:
```ruby
$ roslaunch robot_arm_pkg check_motors.launch
```

```ruby
$ roslaunch robot_arm_pkg check_motors_gazebo.launch
```

```ruby
$ roslaunch moveit_pkg demo.launch
```



