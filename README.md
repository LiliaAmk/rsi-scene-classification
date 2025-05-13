### rsi-scene-classification
## Scene Classification of High-Resolution Remote Sensing Imagery
This repository contains a two-part mini-project based on the scientific paper:  
**"Transferring Deep Convolutional Neural Networks for the Scene Classification of High-Resolution Remote Sensing Imagery"**  
[Link to paper](https://www.mdpi.com/2072-4292/7/11/14680)


## Overview

The project is divided into two parts:

### Part 1: Reproduction of the Paper's Approach
- Extracted features from a pre-trained VGG-16 network.
- Used both fully connected layer features and convolutional features.
- Compared with traditional feature descriptors: HOG and SIFT.
- Applied classifiers (e.g., SVM) on the extracted features for scene classification.
- Evaluated performance on the UC Merced Land Use Dataset.

### Part 2: Performance Enhancement
- Fine-tuned a ResNet50 model on the same dataset using PyTorch.
- Applied data augmentation and training techniques covered in the course.
- Compared the fine-tuned model’s performance with the baseline methods from Part 1.

## Results Summary

| Method                  | Accuracy |
|-------------------------|----------|
| HOG + SVM               | 62.98%   |
| SIFT + SVM              | 24.29%   |
| VGG-16 (FC features)    | 95.00%   |
| VGG-16 (Conv features)  | 96.31%   |
| Fine-tuned ResNet50     | 80.87%   |

## Dataset

- UC Merced Land Use Dataset
- 21 scene categories
- 100 images per category
- Image size: 256x256 pixels

## Dependencies

- Python 3.x
- PyTorch
- OpenCV
- Scikit-learn
- Matplotlib
- NumPy
