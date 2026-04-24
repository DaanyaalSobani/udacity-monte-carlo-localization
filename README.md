# udacity-monte-carlo-localization

The third project in the [Udacity Robotics Software Engineering Nanodegree](https://www.udacity.com/course/robotics-software-engineer--nd209).

Implements Monte Carlo Localisation (MCL) — also known as a particle filter — using the [Adaptive Monte Carlo Localisation (AMCL)](http://wiki.ros.org/amcl) ROS package to localise a robot within a known map.

## Stack

- [ROS](https://www.ros.org/) (Robot Operating System)
- [Gazebo](http://gazebosim.org/) — physics simulation
- [AMCL](http://wiki.ros.org/amcl) — particle filter localisation
- `teleop_twist_keyboard` — keyboard teleoperation

## Usage

After building the catkin workspace:

```bash
source devel/setup.bash

# Launch simulation world and robot
roslaunch my_robot world.launch

# Launch AMCL localisation stack in a separate terminal
roslaunch main amcl.launch
```

Set a 2D Nav Goal in RViz or drive with `teleop_twist_keyboard` — watch the particle cloud converge as the robot localises itself.

## Screenshots

![Gazebo simulation](Localization.png)
