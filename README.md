# Squat Detection using MediaPipe Pose Estimation

Real-time squat detection and classification using **MediaPipe Pose Landmarker** and computer vision. Detects and classifies standing vs squatting poses based on knee joint angles.

## Architecture

**MediaPipe BlazePose** [[research](https://research.google/blog/on-device-real-time-body-pose-tracking-with-mediapipe-blazepose/)] - 33 3D body landmarks detection
**Angle Calculation** - Hip-Knee-Ankle angle computation  
**Classification Logic** - Threshold-based pose classification

### Key Features
- **Real-time detection**: Processes video frames at 30+ FPS
- **33 pose landmarks**: Full-body skeletal tracking
- **Angle-based classification**: Knee angle > 160° = Standing, ≤ 160° = Squatting
- **Visualization**: OpenCV overlay with pose landmarks
