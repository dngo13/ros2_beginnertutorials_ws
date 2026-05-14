# ROS2 Beginner Tutorials Workspace
## Requirements
- Ubuntu 24.02
- ROS2 Kilted (Install [here](https://docs.ros.org/en/jazzy/Installation/Ubuntu-Install-Debs.html))

This ROS2 workspace has the packages from the beginner tutorials from the ROS 2 Kilted documentation. 
## Packages in `/src`
- `cpp_pubsub` - Example C++ publisher and subscriber
- `cpp_srvcli` - Example C++ action client service
- `examples` - Examples from the ROS2 github
- `more_interfaces` - Custom message interface with publisher subscriber
- `my_package` - Example C++ simple package
- `my_package_py` - Example Python simple package
- `py_pubsub` - Example Python publisher and subscriber
- `py_srvcli` - Example Python action client service
- `ros_tutorials` - Examples from ROS2 turtlesim
- `tutorial_interfaces` - Example custom msg and srv

## Running code
- Ensure the workspace is built with `colcon build`
- If you need to build a specific package then run `colcon build --packages-select "package name"`
- Make sure the environment is sourced with `source install/setup.bash`
- Install any missing dependencies by going to root folder `ros2_ws` and run `rosdep install -i --from-path src --rosdistro kilted -y`