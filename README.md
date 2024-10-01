# Batik-Classification

# Project Overview
This project is part of my final group project for the 4th semester Deep Learning course. Our objective is to classify batik patterns using deep learning techniques. Batik, a traditional textile art form, is internationally recognized and features intricate patterns. However, manually identifying specific batik patterns is a challenging task due to the vast number of similar designs. To address this, we employed transfer learning with EfficientNet B2 to build an effective model for batik pattern classification.

# Dataset
The dataset was retrieved from [Kaggle: Indonesian Batik Motifs](https://www.kaggle.com/datasets/dionisiusdh/indonesian-batik-motifs). It contains 20 different batik patterns, from which we were asked to select three for our project. We chose Batik Lasem, Batik Megamendung, and Batik Kawung because these three patterns have clear and distinctive features that set them apart from others. Each folder of batik pattern has 50 images in it. Each image has different resolution and sizes which were preprocessed before feeding into the model. 

# Model Architecture
We experimented with three different models: one that we built from scratch, the same model with hyperparameter tuning, and a transfer learning approach using EfficientNet B2. We tested each model with both non-augmented and augmented data. After training and evaluating these six models, we compared their performance to identify the best one.

# Training Details 
The models were trained for 10 epochs with a batch size of 32 using the Adam optimizer. Training was conducted on Google Colab with a T4 GPU provided by the platform.

# Evaluation Metrics
The models were evaluated using accuracy as reported by the classification report. The best-performing model was EfficientNet B2, achieving an accuracy of 100%, demonstrating excellent performance in distinguishing the three batik patterns.

# Results 
![image](https://github.com/user-attachments/assets/fdea9510-5eff-4ad5-808f-4fdcd08f9c19)
EfficientNet B2 achieved perfect accuracy for this classification task, largely due to its ability to handle complex image problems and its training on large datasets. Even when data augmentation was applied, the model maintained 100% accuracy.
