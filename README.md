# Cuffless Blood Pressure Estimation using PPG and Deep Learning

This project explores cuffless blood pressure (BP) estimation using photoplethysmogram (PPG) signals combined with deep learning techniques. The approach leverages advanced signal processing and computer vision by converting 1D PPG signals into 2D representations, enabling CNN-based regression models to estimate systolic and diastolic BP without the need for physical contact or cuffs.

## Key Features

- PPG Signal to Image Conversion  
  Converted PPG signals from the PulseDB dataset into various 2D image representations:
  - Visibility Graphs
  - Poincaré Maps
  - Recurrence Plots

- Deep Feature Extraction with CNNs  
  Used pre-trained CNNs such as:
  - VGG19
  - MobileNet
  
  for extracting deep features from generated images.

- Regression-based BP Estimation  
  Applied regression models to predict blood pressure:
  - Ridge Regression
  - K-Nearest Neighbors (KNN)

- Hydra Model for Multi-Scale Fusion  
  Implemented a Hydra architecture to fuse multi-scale features, improving prediction accuracy by capturing temporal and spatial relationships more effectively.

- Mobile PPG from Face Videos  
  Extended the system to process face videos captured via smartphone cameras:
  - Extracted PPG signals from skin regions using color channel analysis (e.g., green channel enhancement)
  - Applied temporal filtering to clean the signal for further processing

## Dataset

- PulseDB: A large-scale open-access PPG dataset containing synchronized PPG and BP readings.
- Mobile video samples (for skin-based PPG extraction) are either self-collected or taken from publicly available video BP datasets.

## Project Structure

