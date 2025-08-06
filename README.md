# Football Analysis Project

## Introduction
s project aims to detect and track football players, referees, and the ball in match footage using YOLO, one of the most powerful real-time object detection models available. We go beyond basic detection by implementing several advanced computer vision techniques to generate meaningful match analytics.

🔍 Key Features
Object Detection & Tracking
We use YOLO to detect key entities (players, referees, ball) in each frame, and then track their movements across frames using object IDs.

Team Classification using K-Means Clustering
Players are classified into respective teams by applying K-Means clustering on the pixel colors of their jerseys, enabling team-wise analysis.

Ball Possession Estimation
Based on proximity and interaction between players and the ball, we calculate each team’s ball possession percentage.

Camera Movement Detection using Optical Flow
To account for camera panning or zooming, we implement optical flow, helping in adjusting player movement data relative to a stable ground plane.

Perspective Transformation
We apply perspective transformation to convert player positions from pixel space to real-world units (meters), making distance and speed measurements more accurate.

Speed & Distance Tracker
By combining tracking, frame rate, and transformed coordinates, we calculate:

Real-time player speed (m/s)

Total distance covered during the match (meters)

🧠 Technologies Used
YOLOv5 / YOLOv8 (for object detection)

OpenCV (for tracking, image processing, optical flow, perspective transformation)

Scikit-learn (for K-Means clustering)

NumPy, Pandas, Matplotlib (for data handling & visualization)

🎯 Why This Project?
This project covers a range of real-world computer vision challenges, combining detection, tracking, clustering, and transformation. It provides a practical foundation for sports analytics and is suitable for:

⚙️ Beginner ML/AI enthusiasts learning to work with real-world data

🧠 Experienced engineers interested in applying vision techniques to structured sports analysis
## Requirements
To run this project, you need to have the following requirements installed:
- Python 3.x
- ultralytics
- supervision
- OpenCV
- NumPy
- Matplotlib
- Pandas
