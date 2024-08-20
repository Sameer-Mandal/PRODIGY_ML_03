# PRODIGY_ML_03
Task 3 of Machine learning internship at Prodigy Infotech 

## Introduction to Support Vector Machines (SVMs)

Support Vector Machines (SVMs) are supervised learning models used for classification and regression tasks. They are particularly effective in high-dimensional spaces and are versatile in terms of the decision boundary's shape. The core idea of SVM is to find the optimal hyperplane that maximizes the margin between different classes in the dataset. This makes SVMs robust classifiers, especially when dealing with linear and non-linear data through the use of kernel functions.

In this project, SVM is integrated as the final classification layer of a Convolutional Neural Network (CNN) to improve the classification accuracy of image data.

## Project Overview

### Objective
The goal of this project is to build an image classification model using CNN for feature extraction, followed by SVM as the final layer for classification. The integration of SVM is expected to enhance the model's ability to generalize well on unseen data.

### Methodology

1. **Environment Setup**:
   - Configured TensorFlow to manage GPU resources effectively, ensuring efficient training of the model.

2. **Data Preprocessing**:
   - Utilized `ImageDataGenerator` for data augmentation, which included rescaling, shearing, zooming, and flipping of images to create a more robust model.
   - The dataset was split into training and test sets, with 8,000 images for training and 2,000 images for testing, belonging to two classes.

3. **Convolutional Neural Network (CNN) Architecture**:
   - A CNN was designed to extract meaningful features from the images. The architecture included several convolutional layers followed by pooling layers to down-sample the feature maps.
   - After feature extraction, the final layer was replaced with an SVM classifier instead of the usual softmax layer to enhance the classification process.

4. **Training and Evaluation**:
   - The model was trained using the preprocessed training dataset.
   - Evaluation of the model was carried out on the test set to measure its accuracy and performance.

### Results and Insights

- The combination of CNN and SVM provided a robust model for image classification, showing improved generalization on test data.
- Data augmentation played a significant role in improving model performance by making it more resilient to variations in the input data.
- The SVM layer contributed to better decision boundaries, particularly in cases where the classes were not linearly separable in the feature space extracted by the CNN.

### Conclusion

This project demonstrates the effectiveness of combining CNN for feature extraction with SVM for classification, resulting in a powerful image classification model. The methodology and insights derived from this project can be applied to various other classification tasks, especially those involving complex and high-dimensional data.
