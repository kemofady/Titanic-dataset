# Titanic Dataset: Predicting Survivors

This project uses the Titanic dataset to build an SVM model to predict whether a passenger would survive the Titanic disaster. The focus is on data preprocessing, feature selection, and model evaluation.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Modeling and Evaluation](#modeling-and-evaluation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)

## Project Overview
The Titanic disaster is one of the most famous shipwrecks in history. This project uses data science techniques to predict the likelihood of survival based on features like class, age, gender, fare, etc., with an emphasis on the Support Vector Machine (SVM) algorithm for classification.

## Dataset
The dataset used in this project is the Titanic dataset, containing the following columns:
- **Survived**: Survival (0 = No, 1 = Yes)
- **Pclass**: Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd)
- **Sex**: Gender
- **Age**: Age in years
- **SibSp**: Number of siblings/spouses aboard the Titanic
- **Parch**: Number of parents/children aboard the Titanic
- **Fare**: Passenger fare
- **Embarked**: Port of Embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

## Installation
To run this project locally, you need Python and the required libraries.

1. Clone the repository:
   ```bash
   git clone https://github.com/kemofady/Titanic-dataset.git
   cd Titanic-dataset
## Modeling and Evaluation
The project focuses on building a Support Vector Machine (SVM) model to predict passenger survival. The following steps were taken in the modeling process:

1. **Data Preprocessing**:
   - **Handling Missing Values**: Missing data, especially in the `Age` and `Embarked` columns, was handled using mean imputation and mode imputation, respectively.
   - **Categorical Encoding**: Categorical variables such as `Sex` and `Embarked` were converted into numerical format using one-hot encoding.
   - **Feature Scaling**: Continuous variables like `Age` and `Fare` were scaled using standardization to ensure better performance of the SVM algorithm.

2. **Model Selection**:
   - A Support Vector Machine (SVM) classifier was selected as the primary model due to its effectiveness in classification tasks. The model separates passengers into survivors and non-survivors using a hyperplane in a multidimensional space.

3. **Hyperparameter Tuning**:
   - Grid search cross-validation was used to fine-tune the model's hyperparameters such as the kernel (`linear`, `rbf`) and the regularization parameter (`C`) to optimize model performance.

4. **Evaluation Metrics**:
   - The model was evaluated using several performance metrics:
     - **Accuracy**: The proportion of correct predictions out of all predictions.
     - **Precision**: The ratio of true positives to the sum of true and false positives.
     - **Recall**: The ratio of true positives to the sum of true positives and false negatives.
     - **F1-Score**: The harmonic mean of precision and recall.

The final model was tested on unseen data and evaluated based on these metrics to ensure generalization and performance.

## Usage
To run the SVM model:

1. Ensure that all dependencies are installed, and the environment is set up.
   
2. Run the model script:
   ```bash
   python titanic_svm_model.py


## Results
The Support Vector Machine (SVM) model achieved high accuracy in predicting passenger survival on the Titanic. The model's performance was evaluated using the following metrics:

- **Accuracy**: The overall proportion of correct predictions.
- **Precision**: The number of true positive predictions divided by the total number of positive predictions.
- **Recall**: The proportion of actual positives that were correctly identified by the model.
- **F1-Score**: The harmonic mean of precision and recall, providing a balance between both metrics.

Detailed performance metrics and visualizations of the results can be found in the `notebooks` folder, where a thorough analysis of the model's performance is provided.

## Contributing
Contributions to this project are welcome! If you'd like to improve the project or add new features, please follow these steps:

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature-branch


