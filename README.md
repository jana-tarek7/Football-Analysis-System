# Football-Analysis-System
Description:
This project is an end-to-end AI-powered football analysis system that leverages Computer Vision and Deep Learning to automatically analyze football match videos. It combines state-of-the-art object detection, tracking, motion estimation, and geometric transformations to extract meaningful player and match statistics.

The system uses YOLO to detect players, referees, and the ball in each video frame, while multi-object tracking algorithms maintain the identities of detected objects throughout the match. To further improve detection performance, a custom object detection model is trained and integrated into the pipeline.

To distinguish between teams, the project applies K-Means clustering for jersey color segmentation and classification. Optical Flow is used to estimate camera movement between consecutive frames, allowing the system to compensate for camera motion and accurately measure player movement.

Additionally, Perspective Transformation is employed to model the field's geometry, converting player movement from image coordinates (pixels) into real-world distances (meters). This enables the calculation of key performance metrics such as player speed, distance covered, and movement trajectories.

Key Features
Real-time detection of players, referees, and the ball using YOLO
Multi-object tracking across video frames
Custom-trained object detection model for enhanced accuracy
Team classification based on jersey colors using K-Means Clustering
Camera motion estimation using Optical Flow
Perspective transformation for real-world distance estimation
Player performance analytics, including speed, distance covered, and movement trajectories
End-to-end video analysis pipeline built with Python, OpenCV, and modern deep learning techniques

This project demonstrates the practical application of computer vision and machine learning techniques in sports analytics, integrating object detection, tracking, clustering, motion estimation, and geometric transformations into a unified analysis framework.
# Datasets:
kaggle Dataset: https://www.kaggle.com/competitions/d... Video link used because Kaggle removed the videos from the kaggle dataset above: https://drive.google.com/file/d/1t6ag... Robowflow Football Dataset: https://universe.roboflow.com/roboflow-jvuqo/football-players-detection-3zvbc/dataset/1

Dependencies:
To run this project, you need to have the following requirements installed:

Python 3.x ultralytics supervision OpenCV NumPy Matplotlib Pandas
