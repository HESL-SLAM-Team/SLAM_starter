# Introduction to SLAM: A Beginner’s Guide for Students

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



