
<div align="center">
  <h1>Pet Classifier</h1>
</div>

## Tools and Concepts Applied
1. Python
2. Modules: numpy, pandas, matplotlib
3. Jupyter Notebook
4. K-Folds method of partitioning dataset
5. PCA Dimensionality Reduction
6. LDA, QDA, Closest Avg Classification 

## Introduction
My goal was to build an image classifier for differentiating pictures of cats vs. dogs. Furthermore, I wanted to evaluate the performance of LDA, QDA, and Closest Average decision rules for this task. 

## Data
The dataset consisted of 64 x 64 grayscale images of 1000 cats and 1000 dogs.
The images are registered so facial features appear in the same region for each image.
The dataset was complied by BU course staff

## Data Processing
Data Transformation:
Each picture was “unwrapped” to produce a length-4096 vector of grayscale intensity. 
Labels of either 0 or 1 were used to denote cats from dogs. 

Data Reduction: 
Principal Component Analysis (PCA) was used to reduce the dimensionality of the dataset to 6 set dimensions (10, 25, 50, 100, 250, 500). 

Testing/Training Data:
An 80-20 split was applied to partition images for training and testing data.
5 folds were used to split the data randomly.

## Evaluating Classification Techniques
For each of the 6 dimensionality reduction parameters, LDA, QDA, and Closest Average Classifiers were applied, and testing/training errors were calculated. 

## Results and Next Steps
A line chart was generated to visualize the average testing/training error rates across the set dimensions for each classifier.

## Code
https://github.com/justinl138/Pet-Classifier 

