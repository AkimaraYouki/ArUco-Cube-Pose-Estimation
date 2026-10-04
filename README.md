ArUco Cube Pose Estimation

OpenCV와 ArUco Marker를 이용하여 큐브의 3D 위치와 자세(Pose) 를 추정하는 프로젝트입니다.

Features

* Camera calibration using a checkerboard
* Lens distortion correction
* ArUco marker detection
* 3D position and orientation estimation
* Coordinate correction for multiple cube faces
* Cube center pose estimation using multiple markers

Tech Stack

* Python
* OpenCV
* NumPy

Overview

각 큐브 면에 부착된 ArUco Marker의 위치와 회전을 추정한 뒤,
각 마커의 좌표계를 큐브 중심 좌표계로 변환하여 큐브의 전체 Pose를 계산합니다.

Camera
  ↓
Camera Calibration
  ↓
ArUco Detection
  ↓
Marker Pose Estimation
  ↓
Coordinate Transformation
  ↓
Cube Pose Estimation

Main Files

* 캠 켈리브레이션용 캡처기.py — Calibration image capture
* 카매라 켈리브레이터.py — Camera calibration
* 캐니엣지 검출.py — Canny edge detection test
* main.py — Camera distortion correction test
* 진짜 최종.py — Multi-marker cube pose estimation
