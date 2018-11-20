# Extended Kalman Filter Sensor Fusion for Radar and Lidar Data

## Overview

This project consists of implementing a sensor fusion software using Extended Kalman Filter (EKF) programmed in C++. Udacity provided a simulator which generates noisy RADAR and LIDAR measurements of the position and velocity of an object, and the Extended Kalman Filter (EKF) must fuse those measurements to predict the position of the object. The communication between the simulator and the EKF is done using WebSocket using the uWebSockets implementation on the EKF side. To get this project started, Udacity provides a sample project that could be found [here](https://github.com/udacity/CarND-Extended-Kalman-Filter-Project).

 ## Prerequisites
The project has the following dependencies (from Udacity's sample project):

1. cmake >= 3.5
2. make >= 4.1
3. gcc/g++ >= 5.4
4. Udacity's simulator [Link](https://github.com/udacity/self-driving-car-sim/releases/)

For instructions on how to install these components on different operating systems, please visit Udacity's sample project [Link](https://github.com/udacity/CarND-Extended-Kalman-Filter-Project)

## Compiling and executing the project

These are the suggested steps (From the root of the repo):
1. mkdir build && cd build
2. cmake .. && make
3. ./ExtendedKF
4. Then start Simulator

The output should be:

```
Listening to port 4567
Connected!!!
```

## Running the Filter

The simulator provides two datasets. The difference between them are:

1. The direction the car (the object) is moving.
2. The order the first measurement which is sent to the EKF. In dataset 1, the LIDAR measurement is sent first. In the dataset 2, the RADAR measurement is sent first.

This is how my output looks like for the two datasets:

## [Dataset1 Output Video](https://github.com/AllenMendes/Extended-Kalman-Filter-Sensor-Fusion-for-Radar-and-Lidar-Data/blob/master/Dataset%201%20output_Extended_Kalman_Filter.mp4)

![image1](https://github.com/AllenMendes/Extended-Kalman-Filter-Sensor-Fusion-for-Radar-and-Lidar-Data/blob/master/Dataset%201.JPG)

## [Dataset2 Output Video](https://github.com/AllenMendes/Extended-Kalman-Filter-Sensor-Fusion-for-Radar-and-Lidar-Data/blob/master/Dataset%202%20output_Extended_Kalman_Filter.mp4)

![image2](https://github.com/AllenMendes/Extended-Kalman-Filter-Sensor-Fusion-for-Radar-and-Lidar-Data/blob/master/Dataset%202.JPG)




