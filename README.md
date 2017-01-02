# realSenseCamera_ROSAprilTags
An Intel Realsense Camera R200 implementation of April Tags in ROS

## RealSense Camera + April Tags Startup ROS Calls:
This will run the drivers, give you the pose estimate from the /tag_detection_pose topic and give you visual feedback. 
1. `roslaunch realsenseCamera_aprilTags realsense_apriltags.launch`

2. `rostopic echo /tag_detections_pose`

3. `rosrun image_view image_view image:=//tag_detections_image`

This package is used in the Helix Experiments calibration Node for calibrating the position of the robot wrt the camera frame for OpenCV. Required for identifying the end effector pose in camera film frame to find extreme points on elastic rod. 

May be used for calibration.
