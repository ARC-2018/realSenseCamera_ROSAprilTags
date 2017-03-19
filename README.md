# realSenseCamera_ROSAprilTags
An Intel Realsense Camera R200 implementation of April Tags in ROS

The AprilTags C++ wrapper used in the MOARbot repos don't return the poses of the corners of the tags needed for conventional 2d-3d correspondence calibration.

This implementation adds a topics /ApriltagsPointsRaw for the corners of the tags for analysis. 

Tested in ROS Indigo and Jade, should also work in Kinetic with added std C++11 tags in the make files. 
