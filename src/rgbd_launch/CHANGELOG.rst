^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package rgbd_launch
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

2.1.3 (2016-09-10)
------------------
* [feat] add prefix to nodelet name `#28 <https://github.com/ros-drivers/rgbd_launch/issues/28>`_
* [maintenance] Enable rostest `#29 <https://github.com/ros-drivers/rgbd_launch/issues/29>`_, `#31 <https://github.com/ros-drivers/rgbd_launch/issues/31>`_
* Contributors: Isaac I.Y. Saito, Kentaro Wada, Yuki Furuta

2.1.2 (2016-05-07)
------------------
* [feat] depth_registered_filtered injection `#25 <https://github.com/ros-drivers/rgbd_launch/issues/25>`_
* [sys] [Travis CI] Update config to using industrial_ci with Prerelease Test. `#23 <https://github.com/ros-drivers/rgbd_launch/issues/23>`_
* Contributors: Jonathan Bohren, Isaac I.Y. Saito

2.1.1 (2015-11-16)
------------------
* 1st ROS Jade release
* [feat] Add convert_metric nodes to depth_registered.launch.xml (`#13 <https://github.com/ros-drivers/rgbd_launch/issues/13>`_ from kbogert/hydro-devel)
* [feat] Add the metric nodes to output a depth image
* [fix] Merge pull request `#1 <https://github.com/ros-drivers/rgbd_launch/issues/1>`_ from piyushk/piyush/kbogert-depth-registered-metric
  fixed rect convert metric to conform to both s/w and h/w pipelines. fixe...
* Contributors: Kenneth Bogert, Piyush Khandelwal

2.1.0 (2014-05-05)
------------------
* Revert "Add machine parameter". closes `#5 <https://github.com/ros-drivers/rgbd_launch/issues/5>`_
* Contributors: Piyush Khandelwal

2.0.1 (2013-09-06)
------------------
* Merge pull request `#2 <https://github.com/ros-drivers/rgbd_launch/issues/2>`_ - added machine parameter to launch nodelet manager on a remote machine.
* Merge pull request `#1 <https://github.com/ros-drivers/rgbd_launch/issues/1>`_ - added debayer_processing argument

2.0.0 (2013-08-19)
------------------
* explicit s/w and h/w processing chains with flags to enable/disable
* marked and moved all launch files as internal
* added a script to serve as an upgrade notice for ROS Hydro. This notice should be removed for ROS Indigo
* fixed cloud processing when device registration is enabled
* added tf prefix resolution to kinect_frames
* Migrated from openni_launch v1.9.1 and removed all openni specific files

