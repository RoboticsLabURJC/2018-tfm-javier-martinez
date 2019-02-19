# 2018-tfm-javier-martinez

# SDSLAM
I'm using an application named SDSLAM, but I have the code in [another repository](https://github.com/javimdr/slam-SD-SLAM) and I still have to move the project to this repository.

## Improvements
### ROSify output
The first improvement that has been made to this SDSLAM project has been to publish through ROS messages the position of the camera as TF and posestamped.

In addition to this, from the YAML file, the parent and child frames can be edited (odom and camera link by default respectively) to calculate the tf. The topic in which the pose is published can be edited as well ("sdslam/pose" by default)

The result can be observed in the following [video](https://youtu.be/AcKQcqukvYM).

## Intel D435 Post-Processing
The D435 camera includes a series of post-processed filters (decimation, disparity, spatial and temporal) in order to improve the depth image.

For this reason, I'm attempting to quantify how much the depth image improves each one of its filters by combining them.
