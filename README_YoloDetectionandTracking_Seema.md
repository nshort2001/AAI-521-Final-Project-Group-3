# AAI-521-Final-Project-Group-3

## YOLO Detection and Tracking
This section provides an overview of the system setup and implementation details for a computer vision system designed to detect and track drones and birds in real-time using YOLOv11 for object detection and DeepSORT for tracking. The system is tailored for applications such as drone airspace monitoring, wildlife conservation, and other aerial surveillance tasks.

## Prerequisites
The setup is performed on Google Colab. The necessary code to install the required packages is already included in the respective notebook. Below are the key dependencies:

    Python: 3.8+
    Libraries:
    ultralytics
    torch
    opencv-python
    matplotlib
    numpy
    pandas
    
## Dataset Preparation
Drone Dataset: Utilized the Drone Dataset UAE ((Drone Dataset (UAV) from Kaggle).
Bird Dataset: Extracted bird images and annotations from the COCO 2017 dataset using a custom script.
Merged Dataset: Combined the drone and bird datasets into a single dataset with consistent annotation formats.

## Training the YOLOv11 Model
Update the yolo_config.yaml file with the path to the dataset, dataset split (train/val/test), and the classes to be detected.
Open and run the notebook drone_bird_classification_detection_yolo11L_Seema.ipynb to train the YOLOv11 model on the prepared dataset.
## Running Detection and Tracking
To perform detection and tracking on a video, open and run the notebook bird_drone_tracking_yolo_deepsort_Seema.ipynb. This notebook integrates YOLOv11 with DeepSORT to track objects in real-time.
