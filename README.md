# yolo-waterlevel-detection
A custom object detection pipeline using Ultralytics YOLOv8, trained on a self-collected dataset to detect glass fill levels, with modular code for training, inference, and visualization.

# Project Overview

This project showcases an end-to-end pipeline for training and testing a YOLOv8 object detection model on a custom dataset that I personally collected and annotated. The dataset focuses on detecting glass fill levels, with images captured under varied conditions and annotated in YOLO format.
The project includes:

  Training module (train_yolo) — Trains a YOLOv8 model using a dataset YAML file, chosen model variant (e.g. yolov8n.pt), image size, and number of epochs. Training results and model weights are saved automatically.
  
  Inference module (display_predictions) — Loads the trained model, runs predictions on test images, and visualizes bounding boxes, class labels, and confidence scores using OpenCV and Matplotlib.
  
  The code is modular and can be easily adapted to new datasets or object detection tasks by replacing the dataset YAML file and training parameters.

# Tech Stack

Python — Core programming language

Ultralytics YOLOv8 — Model training and inference framework

OpenCV — Image processing and drawing bounding boxes

Matplotlib — Visualization of predictions

NumPy — Numerical operations and array handling

Google Colab — Development and training environment with GPU acceleration

# Dataset

The dataset was manually collected and annotated by me using bounding boxes in YOLO format.

It is organized with train/, val/, and test/ folders, plus a .yaml configuration file defining class names and paths.
