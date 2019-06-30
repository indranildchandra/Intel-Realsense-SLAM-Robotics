# SLAM using Intel Realsense d435i

For installation (depending upon your OS version), run the installation script as:

```bash
./install16.sh
```
This script installs the following packages:
1) Intel Realsense SDK
2) Realsense ros-pkg
3) RTAB-Map ros-pkg alongwith RTAB-Map standalone libraries
4) ddynamic_reconfigure ros-pkg (Dependency for Realsense ros-pkg)
5) depthimage_to_laserscan ros-pkg (Dependecy for RTAB Map ros-pkg)

Once you run install.sh, run the following commands:

```bash
roslaunch realsense2_camera rs_rgbd.launch
```
On running this command, all the data regarding the IMU, Depth and RGB will be published on respective topics in real-time. Run: `rostopic info` to get a list of all topics.

Next, open a new terminal and run the next command:

```bash
roslaunch rtabmap_ros rtabmap.launch rtabmapviz:=false rviz:=true rtabmap_args:="--delete_db_on_start"
```
The rtabmap_ros package will subscribe to the some specified topics (in the [rtabmap.launch](https://github.com/indranildchandra/Intel-Realsense-SLAM-Robotics/blob/dev/src/rtabmap_ros/launch/rtabmap.launch)), and start mapping on RViz in realtime. Move the Realsense camera throughout the room you want to map

```bash
roslaunch rtabmap_ros rtabmap.launch localization:=true
```
Once ,you are done with the map, save it; the above command switches the process to 'Localization mode'. If you displace the camera in space, the same movements can be visualised in the map itself, where the current position of the camera in the map is also given.
