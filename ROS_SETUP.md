# Setup workspace
```
sudo apt-get install python-wstool
mkdir -p ~/catkin_ws/src
cd ~/catkin_ws
wstool init src
wstool merge -t src https://bitbucket.org/DataspeedInc/dbw_mkz_ros/raw/default/dbw_mkz.rosinstall
```

# Update workspace and resolve dependencies
```
wstool update -t src
rosdep update && rosdep install --from-paths src --ignore-src
```

# Build workspace
```
catkin_make -DCMAKE_BUILD_TYPE=Release
```

# Launch joystick demo
```
source ~/catkin_ws/devel/setup.bash
roslaunch dbw_mkz_joystick_demo joystick_demo.launch sys:=true
```

# Launch Drive-By-Wire system only
```
source ~/catkin_ws/devel/setup.bash
roslaunch dbw_mkz_can dbw.launch
```