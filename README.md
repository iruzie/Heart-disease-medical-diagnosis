HEART DISEASE MEDICAL DIAGNOSIS MODEL.

## Overview
This project is a machine learning application designed to predict the risk of heart disease in individuals based on various health metrics. Using a dataset from the Cleveland Heart Disease database, the model classifies whether a person is at high risk (1) or low risk (0) of heart disease.

## Table of Contents
- [Technologies Used](#technologies-used)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [How It Works](#how-it-works)
- [Model Evaluation](#model-evaluation)
- [Contributing](#contributing)
- [License](#license)

## Technologies Used
- Python 3.11
- Pandas
- Scikit-learn
- NumPy

## Dataset
The dataset used for training and evaluation can be found in the `Heart_disease_cleveland_new.csv` file. It includes the following features:
- `age`: Age of the patient
- `sex`: Gender (1 = Male, 0 = Female)
- `cp`: Chest Pain Type (0-3)
- `trestbps`: Resting Blood Pressure (in mm Hg)
- `chol`: Serum Cholesterol in mg/dl
- `fbs`: Fasting Blood Sugar > 120 mg/dl (1 = Yes, 0 = No)
- `restecg`: Resting Electrocardiographic Results (0-2)
- `thalach`: Maximum Heart Rate Achieved
- `exang`: Exercise Induced Angina (1 = Yes, 0 = No)
- `oldpeak`: ST Depression Induced by Exercise
- `slope`: Slope of Peak Exercise ST Segment (0-2)
- `ca`: Major Vessels Colored by Fluoroscopy (0-4)
- `thal`: Thalassemia (1-3)
- `target`: Diagnosis (1 = Heart Disease, 0 = No Heart Disease)

## Installation
1. Clone the repository:
   ```bash
   git clone <your-repo-url>
   ```
2. Navigate to the project directory:
   ```bash
   cd heart-disease-diagnosis
   ```
3. Install the required packages:
   ```bash
   pip install pandas scikit-learn
   ```

## Usage
Run the script to start the heart disease prediction application:
```bash
python heart_disease_diagnosis.py
```
Follow the prompts to input the required health metrics for risk assessment.

## How It Works
The model uses the K-Nearest Neighbors (KNN) algorithm to classify the risk of heart disease. After training on a portion of the dataset, it predicts the risk based on user input using the following steps:
1. Data Loading: Loads the dataset and separates features and target labels.
2. Data Preprocessing: Checks for missing values and splits the dataset into training and test sets.
3. Model Training: Initializes and trains the KNN model.
4. User Input: Collects user health metrics and makes a prediction.

## Model Evaluation
The model's accuracy was evaluated using a test set, achieving an accuracy of approximately 68.13%. This can be improved by experimenting with different algorithms, hyperparameters, and feature engineering techniques.

## Contributing
Contributions are welcome! If you have suggestions for improvements or new features, please fork the repository and submit a pull request.

