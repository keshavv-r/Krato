# Carnival-Vision-Challenge
**Crater Detection Using Faster R-CNN Model**

This project focuses on automated lunar crater detection using Faster R-CNN, a state-of-the-art deep learning object detection model. It aims to assist planetary scientists and researchers in identifying impact craters from satellite imagery more accurately and efficiently.

**Overview**

Traditional crater detection methods rely heavily on manual marking or rule-based image processing, which are time-consuming and error-prone. This project uses a deep learning–based approach (Faster R-CNN) to automatically detect crater locations and bounding boxes from lunar surface images.

**Methodology**

Dataset Preparation:
  Collected lunar surface images with crater annotations (xmin, ymin, xmax, ymax).
  Converted labels into Pascal VOC / COCO-style annotation formats.

Model Architecture:
  Backbone: ResNet-50 + FPN
  Region Proposal Network (RPN): Generates candidate regions
  ROI Head: Classifies and refines bounding boxes

Training
  Implemented using PyTorch & torchvision
  Trained with custom dataset
  Loss monitored for both RPN and ROI components

Evaluation Metrics
  mAP (Mean Average Precision)
  IoU (Intersection over Union)
  Precision / Recall Curves
