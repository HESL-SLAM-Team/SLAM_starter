# Introduction to SLAM: A Beginner’s Guide for Students

## Introduction to ROS (Robot Operating System)

### What is ROS?
ROS, or **Robot Operating System**, is a flexible framework for writing robot software. It provides tools, libraries, and conventions aimed at simplifying the task of creating complex and robust robot behavior across a wide variety of robotic platforms.

### Installation
ROS Noetic Ninjemys for Ubuntu 20.04 (Focal) release. Instruction (here)[https://wiki.ros.org/noetic/Installation/Ubuntu].

## Key Features of ROS
- **Modularity**: ROS is built around a publish/subscribe communication model that promotes modular design, enabling developers to focus on specific components without worrying about the entire system.
- **Tools**: Includes tools for simulation, visualization, and debugging, such as:
  - `rviz`: For 3D visualization of robot states and sensor data.
  - `Gazebo`: For simulating robots in a virtual environment.
- **Cross-Platform Support**: Runs on various operating systems like Ubuntu and supports hardware abstraction.
- **Wide Ecosystem**: Contains a large library of pre-built packages for tasks like navigation, control, and perception.

## 1. Types of Cameras for SLAM
### Monocular Camera
- Captures a single 2D image stream.
- **Advantages**: Cost-effective, lightweight.
- **Limitations**: Cannot directly measure depth; relies on algorithms like triangulation and structure-from-motion (SfM).

### Stereo Camera
- Uses two cameras with a fixed baseline to mimic human binocular vision.
- **Advantages**: Provides depth information by comparing disparity between images.
- **Use Case**: Environments where depth accuracy is crucial.

### RGB-D Camera
- Combines color (RGB) and depth information.
- **Depth Technology**: Structured light or time-of-flight (ToF).
- **Examples**: Microsoft Kinect, Intel RealSense.


## 2. Key Camera Parameters
### Intrinsic Parameters
- Focal length, principal point, and distortion coefficients.
- Typically represented in the **camera intrinsic matrix**.
- **Calibration**: Essential for accurate SLAM.

### Field of View (FoV)
- Determines the visible area of the scene.
- Wider FoV helps capture more context but can introduce distortion.

### Resolution
- Higher resolution provides more details but increases computational load.

### Frame Rate
- Higher frame rates are crucial for smooth tracking in fast-moving environments.


## 3. Calibration and Setup
- Use checkerboard patterns for **intrinsic calibration**.
- Ensure cameras are stable and aligned, especially for stereo and multi-camera setups.

### Strongly Suggested Reading!!!
- [Camera Calibration Course by First Principles of Computer Vision](https://www.youtube.com/playlist?list=PL2zRqk16wsdoCCLpou-dGo7QQNks1Ppzo)

### Calibration Tools
- ROS [Camera_calibration](https://wiki.ros.org/camera_calibration) (Recommended for monocular and stereo cameras calibration)
- [kalibr](https://github.com/ethz-asl/kalibr)

## 4. Popular Cameras for SLAM
- **Intel RealSense**: RGB-D and stereo options. SDK installation instruction [here](https://github.com/IntelRealSense/librealsense/blob/master/doc/distribution_linux.md).
- **ZED Stereo Cameras**: High-quality stereo imaging. SDK installation instruction [here](https://www.stereolabs.com/en-sg/developers/release).



