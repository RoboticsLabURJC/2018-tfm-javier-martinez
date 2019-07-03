---
layout: default
---

# Javier Martínez’s TFM
Welcome to the official web for my [MOVA](https://mastervisionartificial.es/) Master Thesis. This web will be updated in order to show my progress. 

The project follows Eduardo Perdices' work on  [SD-SLAM](https://github.com/JdeRobot/SDslam). What he developed was an SLAM algorithm that can be run in 3 differents ways: *Monocular* system, monocular with inertial information (IMU) called *Fusion* and with *RGBD* cameras. 

The main aim that my professors and I looked forward to achieving was to detect and delete dynamic objects from a scene in order to improve the results in these circumstances. Nevertheless, due to the fact that we had an Intel RealSense D435 camera and that the RealSense D435i (which includes an inertial sensor) was just released, we decided to try to improve SD-SLAM fusion (whose results were almost identical to the monocular results) with the aim of using this new camera. 

---

Below, you can check our progress in each of the different aspects that we are going to be tackling through the development of my project. 

#### Intel RealSense D435 / D435i
Because we want to use these gadgets, it is necessary to know as much as possible about them. For this reason, they have been subjected to different analysis. 
* Image quality analysis

#### SD-SLAM
Due to the fact that we have been constantly working with SDSLAM, it´s normal to be continuously fixing and adding new improvements. These general improvements will be gathered in this section. 
* ROSify camera pose

#### SLAM *Fusion* (*Monocular* + IMU)
The tests and improvements carried out specifically with the aim of improving the results obtained while using the SDSLAM Fusion will be added here. 

* Initial state: Monocular vs Fusion
* Code analysis: How and when is the IMU used?
* Trajectory analysis: Monocular vs Fusion
* Analysis of the IMU´s noise. 
* Tool for the objective comparison of the results: SLAM TestBed
* Buffer of IMU´s messages for the improvement of SLAM Fusion results

## Datasets
In order to carry out different SD-SLAM tests, there have been selected different datasets which provide GroundTruth about the camera pose (position and orientation) in time. At the moment, we are using the following:

* [EuRoC MAV](https://projects.asl.ethz.ch/datasets/doku.php?id=kmavvisualinertialdatasets)
* [UZH-FPV Drone Racing](http://rpg.ifi.uzh.ch/uzh-fpv.html)
* Our sequences


