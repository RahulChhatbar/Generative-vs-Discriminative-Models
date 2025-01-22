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
C:\CourseWork\GenerativeArtificialIntelligence\Assignments\Assignment 2
│
├── 021---Assignment-2---Generativevs.-Discriminative-Models.pdf  # Assignment instructions and details.
├── README.md  # This file
├── requirements.txt  # List of dependencies for the project
└── src  # Source code and Jupyter notebooks
    ├── mnist_analysis.ipynb  # MNIST dataset analysis with Naive Bayes and Logistic Regression
    └── penguin_analysis.ipynb  # Penguin species classification analysis```

## Requirements

Before running the code, ensure you have the necessary dependencies installed. You can install them using:

```bash
pip install -r requirements.txt```

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

- **Objective:** Compare the accuracy of Naive Bayes and Logistic Regression.
- **Metrics:** Evaluate performance on both training and test datasets.
- **Insight:** Determine which model better distinguishes between the two penguin species.

### AUC Comparison

- **Objective:** Compute the AUC (Area Under the ROC Curve) for both models.
- **Metrics:** Assess the model’s ability to distinguish between the penguin species.
- **Insight:** Interpret AUC scores to identify which model provides better discrimination.

### Lift and Gain Charts

- **Objective:** Visualize the effectiveness of both models using lift and gain charts.
- **Metrics:** Generate Lift and Gain plots using deciles, comparing both models.
- **Insight:** Evaluate how well each model ranks predicted probabilities.

### Model Performance Comparison

- **Objective:** Compare overall model performance based on the above metrics.
- **Discussion:** Provide a summary of which model is better suited for the penguin species classification task and explain why.

### Performance on MNIST

- **Objective:** Evaluate how Naive Bayes and Logistic Regression perform on the MNIST dataset (handwritten digit recognition).
- **Discussion:** Compare the models' behavior when applied to image data and provide insights into the differences observed between the simpler penguin dataset and the complex MNIST dataset.

## Conclusion

This project demonstrates the application of both Generative and Discriminative models to real-world classification tasks, showcasing their respective strengths and weaknesses. The comparison provides insights into how each model type handles different data complexities.
