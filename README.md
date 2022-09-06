# ROS2-HDR

In this project, a holonomic drive robot called duke is designed and simulated to learn ROS2 and Control Systems.

In this project, we have designed the duke bot for exploring the ros2 navigation stack. This project is open source and built in such a manner that it can be used by robotics enthusiasts for their projects. Also, the necessary instructions are provided to develop a new project based on the user’s interests.

This repository contains all the codes with the necessary details to re-build this project.

## Installation

In this project, we have used humble distribution on ubuntu 22.04 LTS, But this project should work on other ROS 2 distributions. 
Install ROS2 from official [site](https://docs.ros.org/en/humble/Installation/Ubuntu-Install-Debians.html). While installing ROS2 make sure you use this command.

    sudo apt install ros-humble-desktop-full # Instead sudo apt install ros-humble-desktop

You can use this site to get started with ROS2 and understand its concepts. This will help you to understand any ROS2 projects available on the internet.

After verifying ROS2 Installation, Check whether Gazebo-11 is installed. By Running the below-mentioned command. This command will print the gazebo version and launches it.

    gazebo --verbose

If the gazebo is not recognized, install gazebo-11 using this [link](https://classic.gazebosim.org/tutorials?tut=ros2_installing&cat=connect_ros). Make sure to use the appropriate distro in the command.

Apart from the above-mentioned installation, you might need to install some ROS2 binary packages which are mentioned below.

    sudo apt-get install ros-humble-rosidl-typesupport-c
    sudo apt-get install ros-humble-joint-state-publisher
    sudo apt-get install ros2-controllers -y
    sudo apt-get install ros-humble-turtle-tf2-py ros-humble-tf2-tools ros-humble-tf-transformations
    sudo apt install ros-humble-navigation2
    sudo apt install ros-humble-nav2*
    sudo apt install ros-humble-robot-localization
    sudo apt install ros-humble-slam-toolbox
    sudo apt install ros-humble-rqt-robot-steering
    sudo pip3 install transforms3d

Do not forget to source ROS2 and Gazebo setup.bash in the ~/.bashrc file.

    # For Colcon Auto-Completion
    source /usr/share/colcon_argcomplete/hook/colcon-argcomplete.bash
    # ROS 2 Bash
    source /opt/ros/humble/setup.bash
    # Gazebo 11 Bash
    source /usr/share/gazebo-11/setup.sh
    # ROS2 Workspace
    source ~/<ROS2-Workspace>/install/setup.bash
## Repository Structure

* duke_bot_description – ROS2 python package containing all the files related to holonomic drive robot for simulation
* hdr_navigation – ROS2 python package to explore the navigation stack using the duke bot in gazebo simulation
* nav_world – ROS2 CPP package containing all the files related to add simulation world in the gazebo
* designFiles – duke bot design in Fusion360, SolidWorks and SketchUp Format are attached.

## Demonstration


### Project Members

Hari Vikinesh, Jerish Abijith Singh
