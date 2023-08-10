# IMU MoCap Fusion

## Quick Start

The project has been tested on Ubuntu 20.04(ROS Noetic).

### Prerequisites

Install `Eigen3`

```bash
sudo apt install libeigen3-dev
```

Install `yaml-cpp`

```bash
git clone https://github.com/jbeder/yaml-cpp.git
cd yaml-cpp
mkdir build && cd build
cmake .. && make
sudo make install
```

### Build on ROS

```bash
cd ${YOUR_WORKSPACE_PATH}/src
git clone https://github.com/helloliver/imu_mocap_fusion.git
cd ${YOUR_WORKSPACE_PATH}
catkin_make
```

### RUN !

```bash
cd ${YOUR_WORKSPACE_PATH}
source devel/setup.bash
roslaunch imu_mocap_fusion main.launch mav_name:={YOUR_ROBOT_NAME}
```

## Licence

The source code is released under [Apache 2.0](http://www.apache.org/licenses/LICENSE-2.0) license.
