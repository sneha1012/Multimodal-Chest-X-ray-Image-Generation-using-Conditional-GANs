# Conditional Generative Adversarial Network (cGAN) for Synthetic Chest X-ray Image Generation
Project Overview
This repository showcases the implementation of a Conditional Generative Adversarial Network (cGAN) tailored to generate synthetic chest X-ray images representing seven distinct medical conditions. By leveraging these synthetic images, we aim to supplement authentic datasets, thereby minimizing data collection expenses and addressing prevalent privacy concerns in medical imaging.

Table of Contents
Installation
Dataset
Usage
Results
Technologies Used
Contributing
License
Acknowledgements
Installation
Clone the repository:
bash
Copy code
git clone https://github.com/sneha1012/MultiModal-Genesis
Navigate to the project directory and install required packages:
bash
Copy code
cd MultiModal-Genesis
pip install -r requirements.txt
Dataset
Chest X-ray examinations stand as one of the most recurrent and cost-effective medical imaging procedures. Despite their accessibility, interpreting these images can be intricate, often posing more challenges than chest CT scans. The scarcity of large, publicly available datasets with comprehensive annotations hinders the progress of achieving clinically pertinent computer-aided detection in real-world scenarios.

The NIH Chest X-ray Dataset employed in this project consists of 112,120 X-ray images labeled with disease indicators from 30,805 distinct patients. Disease labels were curated using Natural Language Processing techniques to mine classifications from relevant radiological reports, boasting an accuracy of over 90%, deeming it suitable for weakly-supervised learning endeavors.

For this project, a subset of 1,501 samples from the NIH dataset was used.

Dataset Source: NIH Chest X-rays on Kaggle

Usage
To train the model, execute:

bash
Copy code
python train.py
Results
The cGAN, post-training, exhibited the capability to generate synthetic X-ray images emulating the authentic medical visuals closely.


Technologies Used
Tensorflow
Keras
Google Colab
Numpy
Pandas
Matplotlib
IPython
Contributing
Pull requests are cordially welcomed. For substantial alterations, kindly open an issue first to deliberate on what you'd aspire to modify.

License
This project is licensed under the MIT License.

Acknowledgements
Sincere gratitude to the creators of the NIH Chest X-ray Dataset and all relevant publications aiding this research.


Unveiling the future of medical imaging with advanced deep learning: Synthesize diverse chest X-rays, decode multimodal insights, and enhance rare pulmonary pathology diagnostics.
