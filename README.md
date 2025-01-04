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

---

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

---

## 3. Calibration and Setup
- Use checkerboard patterns for **intrinsic calibration**.
- Ensure cameras are stable and aligned, especially for stereo and multi-camera setups.

---

## 4. Camera Placement in SLAM
- **Monocular**: Typically mounted forward-facing.
- **Stereo**: Baseline distance must match the target depth range.
- **RGB-D**: Avoid reflective or transparent surfaces to prevent interference.

---

## 5. Popular Cameras for SLAM
- **Intel RealSense**: RGB-D and stereo options.
- **ZED Stereo Cameras**: High-quality stereo imaging.
- **Microsoft Azure Kinect**: Combines advanced depth sensing and color capture.

---

