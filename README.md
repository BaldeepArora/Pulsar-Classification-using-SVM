# Pulsar Star Classification using SVM

### Project Overview
This project applies a Support Vector Machine (SVM) classifier to identify pulsar stars from noise, based on the dataset provided by the High Time Resolution Universe Survey. The focus is on handling the class imbalance using Synthetic Minority Over-sampling Technique (SMOTE) and optimizing the SVM model with various kernels.

### Dataset used
The dataset comprises several features derived from integrated pulse profiles and DM-SNR curves, which are typical indicators used for pulsar analysis. Data preprocessing steps include normalization and SMOTE for balancing class distribution.<br>
URL link - https://archive.ics.uci.edu/dataset/372/htru2

### Features
1. Mean of the integrated profile: Statistical features of the integrated profile of the pulse.
2.Standard deviation of the integrated profile
3. Excess kurtosis of the integrated profile
4. Skewness of the integrated profile
5. Mean of the DM-SNR curve
6. Standard deviation of the DM-SNR curve
7. Excess kurtosis of the DM-SNR curve
8. Skewness of the DM-SNR curve
9. Target: Binary label (Pulsar/Noise)

### Methods
1. Data Preprocessing: Scaling features and applying SMOTE to balance the dataset.
2. SVM Classification: Training SVM classifiers with different kernel functions (linear, polynomial, rbf, and sigmoid) and tuning the penalty parameter C.
4. Evaluation: Model performance is evaluated using accuracy, precision, recall, and F1-score metrics.

### Requirements
To run this project, you will need Python and the following packages:
1. NumPy
2. Pandas
3. Matplotlib
4. Scikit-learn
5. Imbalanced-learn

### Usage
Clone the repository and install the required packages:
```
git clone https://github.com/BaldeepArora
cd Pulsar-Classification-using-SVM
```

### Results
The SVM model achieved promising results, with the polynomial kernel showing the best performance at higher C values, balancing the trade-off between bias and variance effectively.



