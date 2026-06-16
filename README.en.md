# MUSASHI Player ROS 2

[日本語](README.md)

MUSASHI Player ROS 2 is a robot software platform based on ROS 2 Jazzy.

This project is designed as a software framework for RoboCup Middle Size League (MSL) robots.

## Features

* ROS 2 Jazzy
* Gazebo Harmonic simulation
* Docker + Dev Container support
* Real robot control using EPOS2
* Extensible architecture for RoboCup MSL
* Designed for seamless transition from simulation to hardware

## Directory Structure

```text
musashi_player_ros2/
├── .devcontainer/
├── docker-compose.yml
├── src/
│   ├── behavior/
│   ├── bringup/
│   ├── communication/
│   ├── hardware/
│   ├── simulation/
│   └── vision/
├── LICENSE
└── README.md
```

### behavior

Strategy and behavior modules.

### bringup

Launch files and system startup configurations.

### communication

RefBox and team communication modules.

### hardware

Interfaces for physical devices.

### simulation

Gazebo simulation packages.

### vision

Image acquisition and perception modules.

## Development Environment

* Ubuntu 24.04
* Docker
* VS Code
* Dev Containers
* ROS 2 Jazzy
* Gazebo Harmonic

## Setup

### 1. Clone the repository

```bash
git clone <repository-url>
cd musashi_player_ros2
```

### 2. Launch the Dev Container

Open the project in VS Code and run:

```
Dev Containers: Reopen in Container
```

### 3. Build

```bash
source /opt/ros/jazzy/setup.bash

colcon build --symlink-install

source install/setup.bash
```

## License

Please refer to the LICENSE file for license information.
