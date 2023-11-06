# Conditional Generative Adversarial Network (cGAN) for Synthetic Chest X-ray Image Generation
# Multimodal Chest X-ray Image Generation using Conditional GANs

## About the Project
<img width="541" alt="results with labels" src="https://github.com/sneha1012/MultiModal-Genesis/assets/79008130/2b790fd1-37f1-458b-951a-703cd52a67d1">

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

There are 15 classes, including 14 disease types and one 'No findings' category. Diseases include Atelectasis, Consolidation, Infiltration, and more. But here for our research we have used 6 different dieases. In total of 7 classes, one being "no finding"

<img width="1180" alt="preprocessed data 128*128" src="https://github.com/sneha1012/MultiModal-Genesis/assets/79008130/d1d474d1-e88f-427e-a97a-b0eb85e3aaae">


```python
tensorflow
numpy
matplotlib
google.colab
opencv-python
IPython
scikit-image
ipykernel
```

# Model Performance
Accuracy Over Epochs
![Unknown-5](https://github.com/sneha1012/MultiModal-Genesis/assets/79008130/02506ead-fb47-45fe-9d6f-81b4c7c63f3c)


# Loss Over Epochs
Loss Graph

![Unknown-4](https://github.com/sneha1012/MultiModal-Genesis/assets/79008130/e090e694-89ca-4469-8d85-fe9d72351d08)


# Acknowledgements
This project has been made possible through the resources provided by the NIH Clinical Center and the National Library of Medicine. We extend our gratitude to the dataset authors for making it publicly available.

# Citations
Please cite the following work when using this dataset or the cGAN model:
@inproceedings{wang2017chestx,
  title={ChestX-ray8: Hospital-scale Chest X-ray Database and Benchmarks on Weakly-Supervised Classification and Localization of Common Thorax Diseases},
  author={Wang, X. and Peng, Y. and Lu, L. and Lu, Z. and Bagheri, M. and Summers, R.M.},
  booktitle={Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition (CVPR)},
  year={2017}
}








