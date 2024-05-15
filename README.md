# Optical Flow and Object Tracking

This project demonstrates the use of optical flow algorithms for tracking objects in video streams. It includes examples using Farneback's dense optical flow and Lucas-Kanade's sparse optical flow. The project is divided into three main scripts, each demonstrating different tracking techniques.

## Prerequisites

Ensure you have the following installed:

- Python 3.x
- OpenCV
- NumPy

You can install the required libraries using pip:

pip install opencv-python numpy

## Files and Scripts

### 1. Dense Optical Flow (Farneback Method)

This script uses Farneback's method to compute dense optical flow. It visualizes the flow using both line representation and HSV color encoding.

- **File**: `dense_optical_flow.py`
  
- **Description**: Computes and visualizes dense optical flow.
  
- **Usage**: 
  python dense_optical_flow.py
  
- **Features**:
  - Computes optical flow between frames.
  - Visualizes flow using line representation and HSV encoding.
  - Displays FPS for performance monitoring.

### 2. Sparse Optical Flow (Lucas-Kanade Method)

This script uses the Lucas-Kanade method for tracking a sparse set of features. It tracks the features over frames and displays the motion trajectories.

- **File**: `sparse_optical_flow.py`
  
- **Description**: Tracks sparse features using Lucas-Kanade method and displays trajectories.
  
- **Usage**: 
  python sparse_optical_flow.py
  
- **Features**:
  - Detects good features to track.
  - Tracks features across frames.
  - Displays motion trajectories and FPS.

### 3. Object Tracking with ROI Update

This script demonstrates object tracking by selecting a Region of Interest (ROI) and dynamically updating the ROI based on the tracked object's movement.

- **File**: `roi_tracking.py`
  
- **Description**: Tracks objects by dynamically updating the Region of Interest (ROI).
  
- **Usage**: 
  python roi_tracking.py
  
- **Features**:
  - Allows user to select an initial ROI.
  - Tracks objects and updates ROI based on movement.
  - Displays tracking integrity and FPS.

## How to Run

1. **Clone the Repository**:
   git clone https://github.com/yourusername/optical-flow-tracking.git
   cd optical-flow-tracking

2. **Run the Desired Script**:
   - For dense optical flow:
     python dense_optical_flow.py
     
   - For sparse optical flow:
     python sparse_optical_flow.py
     
   - For object tracking with ROI update:
     python roi_tracking.py

## Additional Information

- Ensure your webcam is connected, as the scripts use it to capture video.
- Press `q` to quit the application at any time.
- In the `roi_tracking.py` script, press `a` to start tracking after selecting the ROI.

This project provides a hands-on demonstration of optical flow techniques and can be a useful reference for implementing similar algorithms in your own projects.
