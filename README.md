# MRE462_SLAM
SLAM Project

Data Download and Initialization: Download and initialize the dataset containing RGB-D images. This step sets up the environment for working with the visual data.
Data Visualization and Inspection: Create a visual interface to inspect the dataset and ensure it's loaded correctly. This step helps in understanding the data and verifying its integrity.
Card Initialization for 3D Mapping: Initialize the structure to hold 3D map points (referred to as the "card"). This structure stores information about the 3D world, including the location of map points.
Tracking: Implement the tracking component, which continuously estimates the camera pose as it moves through the environment. This involves feature matching and motion estimation techniques to determine how the camera moves relative to the scene.
Local Mapping: Perform local mapping for each keyframe, updating and refining the map points based on the newly added frames. This step ensures that the map accurately represents the environment as more data becomes available.
Loop Closure Detection: Implement loop closure detection to identify and close loops in the trajectory. This involves comparing current images with past images to find similar scenes and calculate relative poses, aiding in improving the map's accuracy.
Bundle Adjustment: Optimize camera poses and 3D points using bundle adjustment techniques to minimize errors in the reconstruction. This step enhances the accuracy of the map and trajectory estimation.
Comparison with Ground Truth: Compare the estimated trajectory with ground truth data to evaluate the SLAM system's accuracy. This validation step ensures that the system is performing as expected.
Code Generation: Generate optimized code using MATLAB Coder to compile MATLAB functions into a MEX file, enhancing efficiency and performance.
Implementation Concerns: Address concerns about the computational requirements of the SLAM system, particularly in the context of mobile robotics. Evaluate whether the processing demands are feasible for deployment on a mobile robot, considering hardware limitations and real-time performance constraints.
Implementation: 

I would use this in a mobile robot so I could view the current surroundings and map them making it easier to maneuver. However, I worry that this would be too much processing for a mobile robot my laptop was struggling to do it in a timely manner.   

