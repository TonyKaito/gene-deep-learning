# Leukemia Classification with Naive Bayes and Multilayer Perceptron

This repository contains a data science project aimed at classifying two types of leukemia—Acute Myeloid Leukemia (AML) and Acute Lymphoblastic Leukemia (ALL)—using gene expression data. The project explores two classification models: Naive Bayes and a Multilayer Perceptron (MLP), comparing their performances on a dataset of gene expression values from the 1999 study by Golub et al.
Project Overview

In this project, we utilize a dataset originally from a proof-of-concept study published by Golub et al., which demonstrated how gene expression monitoring (via DNA microarrays) can be used to classify cancer types. The dataset consists of 38 training samples and 34 test samples corresponding to ALL and AML diagnoses. The goal is to predict whether a new sample corresponds to ALL or AML using gene expression data.
### Dataset

The dataset used in this project comes from the study "Molecular Classification of Cancer: Class Discovery and Class Prediction by Gene Expression Monitoring" by Golub et al. 

https://www.kaggle.com/datasets/crawford/gene-expression/data?select=data_set_ALL_AML_train.csv

The dataset includes measurements of gene expression from Bone Marrow and Peripheral Blood samples. The intensity values in the dataset have been pre-processed and re-scaled such that the overall intensities for each chip are equivalent.
### Key Features of the Dataset:

    * Target variable: Leukemia type (ALL or AML)
    * Input features: Gene expression levels for various genes (over 7,000 features in total)
    * Training set size: 38 samples
    * Test set size: 34 samples

### Model Overview
1. Naive Bayes Model

We first implemented a Naive Bayes classifier, a probabilistic model based on Bayes' theorem. The model assumes independence between the features (genes), which may not hold in reality, but it serves as a baseline due to its simplicity and efficiency.
2. Multilayer Perceptron (MLP)

In the second phase of the project, we implemented a Multilayer Perceptron (MLP), a type of feedforward artificial neural network. This model is more complex and allows for learning non-linear decision boundaries, which may help capture the intricate relationships between the features in the dataset.
### Results and Discussion

The models performed reasonably well; however, they demonstrated flimsy precision, indicating that there may be challenges in distinguishing between the two leukemia types based on the features in the dataset. 