# 教程 how to use

## 1.前期准备 preparation

安装一些功能包 Install some  packages:

```
sudo apt install ros-melodic-joint-state-publisher-gui
sudo apt install ros-melodic-ros-control
sudo apt install ros-melodic-ros-controllers
sudo apt install ros-melodic-gmapping
sudo apt install ros-melodic-ackermann-msgs
sudo apt install ros-melodic-navigation
sudo apt install ros-melodic-teb-local-planner
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





### tianracer一键导航(tianracer one launch file to navigation)

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

## 4.视频地址
[阿克曼移动机器人gazebo仿真项目开源](https://www.bilibili.com/video/BV1ku411r7wG/?spm_id_from=333.999.0.0&vd_source=ddf5e64a1dfd3bc5bcc336b44c063a29)

