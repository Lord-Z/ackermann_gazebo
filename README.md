# 教程 how to use

## 1.前期准备 preparation

安装一些功能包 Install some packages:

```
sudo apt install ros-noetic-joint-state-publisher-gui
sudo apt install ros-noetic-ros-control
sudo apt install ros-noetic-ros-controllers
sudo apt install ros-noetic-gmapping
sudo apt install ros-noetic-ackermann-msgs
sudo apt install ros-noetic-navigation
sudo apt install ros-noetic-teb-local-planner
```

将三个功能包放进工作空间src目录下，进行编译

```
cp /three packages /***_ws/src
cd ..
catkin_make
source devel/setup.bash
```

## 2.使用教程 using tutorial

### racebot建图 (racebot slam)

```
roslaunch racebot_gazebo racebot.launch

roslaunch racebot_gazebo gmapping.launch
```

### tianracer建图(tianracer slam)

```
roslaunch racebot_gazebo tianracer.launch

roslaunch racebot_gazebo gmapping.launch
```

将鼠标点击键盘控制窗口，即可控制小车运动进行建图。Click the mouse on the keyboard control window, you can control the movement of the car to build a map.

### racebot导航(racebot navigation)

```
roslaunch racebot_gazebo tianracer.launch

roslaunch racebot_gazebo navigation.launch
```

### racebot一键导航(racebot one launch file to navigation)

```
roslaunch racebot_gazebo teb_demo.launch
```

### racebot导航建图(racebot navi&slam)

```
roslaunch racebot_gazebo racebot.launch

roslaunch racebot_gazebo slam_navi.launch
```

### tianracer导航建图(tianracer navi&slam)

```
roslaunch racebot_gazebo tianracer.launch

roslaunch racebot_gazebo slam_navi.launch 
```

## 3.博客地址

[Lord_ZYX](https://blog.csdn.net/qq_48427527?type=blog)

