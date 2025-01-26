# Generative vs. Discriminative Models - Assignment 2

## Overview

This project compares the performance of **Naive Bayes** (a Generative Model) and **Logistic Regression** (a Discriminative Model) in classifying penguin species. Specifically, the analysis focuses on two species from the open-source Penguins dataset: **Adelie** and **Gentoo**. The models are evaluated on accuracy, AUC (Area Under the ROC Curve), and Lift and Gain charts, with a further extension to the MNIST dataset for analysis on a more complex task (handwritten digit recognition).

## Objective

- Compare the classification performance of **Naive Bayes** and **Logistic Regression** for binary classification of two penguin species.
- Evaluate the models based on various metrics:
  - Accuracy
  - AUC (Area Under the ROC Curve)
  - Lift and Gain charts
- Extend the analysis to a more complex dataset (MNIST) and compare the performance of Generative and Discriminative models on image data.

## Directory Structure

```plaintext
│
├── 021---Assignment-2---Generativevs.-Discriminative-Models.pdf  # Assignment instructions and details.
├── README.md  # This file
├── requirements.txt  # List of dependencies for the project
└── src  # Source code and Jupyter notebooks
    ├── mnist_analysis.ipynb  # MNIST dataset analysis with Naive Bayes and Logistic Regression
    └── penguin_analysis.ipynb  # Penguin species classification analysis
```

## Requirements

Before running the code, ensure you have the necessary dependencies installed. You can install them using:

```bash
pip install -r requirements.txt
```

## How to Run the Code

### 1. Penguin Species Classification (`penguin_analysis.ipynb`)

1. Open `penguin_analysis.ipynb` in Jupyter Notebook or JupyterLab.
2. The notebook covers the following steps:
   - Load and preprocess the Penguins dataset (Adelie and Gentoo species).
   - Train a **Naive Bayes** model and a **Logistic Regression** model.
   - Evaluate the models based on **Accuracy**, **AUC**, and **Lift and Gain** charts.
   - Interpret results to compare the two models.

### 2. MNIST Analysis (`mnist_analysis.ipynb`)

1. Open `mnist_analysis.ipynb` in Jupyter Notebook or JupyterLab.
2. The notebook covers:
   - Load and preprocess the MNIST dataset.
   - Train both **Naive Bayes** and **Logistic Regression** on MNIST.
   - Compare the performance of both models in a more complex dataset scenario.
   - Evaluate and interpret performance differences.

## Key Sections in the Analysis

### Accuracy Comparison

- **Objective:** Compare how well Naive Bayes and Logistic Regression classify the two penguin species based on accuracy.
- **Metrics:** We evaluate both models on the training and test datasets to understand how accurately they distinguish between the species.
- **Insight:** Both models achieve perfect accuracy on this simple task, making them equally effective in classifying the penguin species in the given dataset.

### AUC Comparison

- **Objective:** Calculate and compare the AUC (Area Under the ROC Curve) for Naive Bayes and Logistic Regression.
- **Metrics:** AUC scores assess each model’s ability to correctly distinguish between the two penguin species.
- **Insight:** Both models achieve a perfect AUC of 1.0, indicating that they perfectly separate the classes, showing optimal performance for this dataset.

### Lift and Gain Charts

- **Objective:** Visualize model performance by generating lift and gain charts, helping to assess the effectiveness of ranking predicted probabilities.
- **Metrics:** Lift and Gain charts are plotted using deciles to evaluate how well each model ranks positive instances.
- **Insight:** Both models show similar performance in identifying positive instances, with strong results in the top deciles, though their effectiveness decreases as they consider lower-probability instances.

### Model Performance Comparison

- **Objective:** Compare the overall performance of Naive Bayes and Logistic Regression using accuracy, AUC, and Lift/Gain charts.
- **Discussion:** Both models achieve identical results in terms of accuracy and AUC, and their Lift and Gain charts show similar performance across deciles. Given the simplicity of the dataset, both models perform equally well, making them both suitable for the classification task.

### Performance on MNIST

- **Objective:** Evaluate how Naive Bayes and Logistic Regression handle the more complex MNIST dataset (handwritten digit recognition).
- **Discussion:** While Logistic Regression outperforms Naive Bayes in accuracy on MNIST, both models struggle with the dataset’s complexity. Naive Bayes shows poor performance due to its assumption of feature independence, while Logistic Regression performs better but still doesn't achieve perfect accuracy, highlighting the need for more advanced models like Convolutional Neural Networks (CNNs) for such tasks.

## Conclusion

This project compares the performance of generative (Naive Bayes) and discriminative (Logistic Regression) models in real-world classification tasks. The analysis highlights their strengths in handling simpler datasets like the penguin dataset and the challenges they face when applied to more complex image data, such as the MNIST dataset. The findings suggest that while both models perform well for the penguin classification task, more sophisticated models would be necessary for more complex datasets like MNIST.
