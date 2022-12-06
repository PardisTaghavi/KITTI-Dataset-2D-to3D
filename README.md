# KITTI-Dataset-2D-to3D

### requirements
* Ubuntu 18.04
* ROS Melodic

#### other required packages
* LaneAtt_ROS
* MMsegmentation_ROS

### Lane_to_3DKitti.py

subscribed topics:
- /kitti/velo/pointcloud
- /laneattNode/LanesArrays

published topics:
- /my_pcl_topic (3D pointcloud of the detected lanes)
- /used_pcl (configurable, cropped pointcloud based on the input)

### Seg_to3DKitti.py

subscribed topics:
- /kitti/velo/pointcloud
- /mmsegmentor/roadarea

published topics:
- /segmented_pcl (3D pointcloud of the detected road area)
- /used_pcl (configurable, cropped pointcloud based on the input)
