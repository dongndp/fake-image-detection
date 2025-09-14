# CSCA: Introduction to Deep Learning Final Project

## 1. Project Overview

While deepfake technology can be useful in some areas such as entertainment and education, its misuse can cause harm to individuals, communities, and society. Detecting deepfakes can help combat fake news and other forms of fraud. 

In this project, we're going to build deep learning models to detect and classify whether a face image is real or fake based on the input images.

### About the dataset
We will be using the [140k Real and Fake Faces](https://www.kaggle.com/datasets/xhlulu/140k-real-and-fake-faces/) dataset from Kaggle. This dataset contains 70,000 real faces (from Flickr) and 70,000 fake faces (GAN-generated), divided into 3 subsets:
- Training set: 50,000 fake images, 50,000 real images, total 100,000 images
- Validation set: 10,000 fake images, 10,000 real images, total 20,000 images
- Test set: 10,000 fake images, 10,000 real images, total 20,000 images

Files:
- train.csv: Training dataset
- valid.csv: Validation dataset
- test.csv: Test dataset

Directory structure:

- 140k-real-and-fake-faces/
    -  real_vs_fake/
        - real-vs-fake/
            - train/
                - fake/
                    - *.jpg <== 50,000 fake images
                - real/
                    - *.jpg <== 50,000 real images
            - valid/
                - fake/
                    - *.jpg <== 10,000 fake images
                - real/
                    - *.jpg <== 10,000 real images
            - test/
                - fake/
                    - *.jpg <== 10,000 fake images
                - real/
                    - *.jpg <== 10,000 real images
            
All images are 256x265px, RGB color, JPEG format.

### Summary of Tasks:
- Load dataset
- Perfom EDA
- Build, evaluate test our CNN models.
- Hyperparameter tuning (Keras tunner).
- Transfer learning (InceptionV3).
- Summarize, compare and discuss the results.
