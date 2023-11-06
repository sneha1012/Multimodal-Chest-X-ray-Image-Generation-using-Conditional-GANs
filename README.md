# Conditional Generative Adversarial Network (cGAN) for Synthetic Chest X-ray Image Generation
# Multimodal Chest X-ray Image Generation using Conditional GANs

## About the Project

This repository houses a sophisticated Conditional Generative Adversarial Network (cGAN) designed to generate synthetic chest X-ray images, depicting six distinct medical conditions. The primary aim of this endeavor is to expand existing datasets with high-fidelity synthetic images, thereby enhancing the robustness of machine learning models used in medical diagnostics.

## Dataset Overview

The NIH Chest X-ray Dataset serves as the backbone for this project, comprising 112,120 X-ray images from 30,805 patients. Each image is labeled for various disease classes, derived using Natural Language Processing (NLP) on accompanying radiological reports.

### Paper Reference

For a thorough understanding of the dataset and labeling process, please refer to:

Wang X, Peng Y, Lu L, Lu Z, Bagheri M, Summers RM. "ChestX-ray8: Hospital-scale Chest X-ray Database and Benchmarks on Weakly-Supervised Classification and Localization of Common Thorax Diseases." in IEEE CVPR, 2017.

[Access the full paper here](https://link.to.the.paper/if/available)

### Data Limitations

- NLP-extracted labels with an estimated accuracy above 90%.
- Bounding box annotations are limited in quantity.
- The radiology reports are not included in the dataset.

### File Structure

The dataset is organized into multiple ZIP archives, each containing a segment of the full image collection, accompanied by a `README_ChestXray.pdf` for detailed dataset information, `BBox_list_2017.csv` for bounding box coordinates, and `Data_entry_2017.csv` for class labels and patient data.

### Class Descriptions

There are 15 classes, including 14 disease types and one 'No findings' category. Diseases include Atelectasis, Consolidation, Infiltration, and more.

## Preprocessing Code

Data preprocessing is a vital step. Below is the code used for resizing and preparing the images for training the cGAN model.

```python
from google.colab import drive
import os
from PIL import Image
import numpy as np
import matplotlib.pyplot as plt '''



