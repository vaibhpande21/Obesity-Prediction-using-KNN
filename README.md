# Obesity Prediction using k-Nearest Neighbors (kNN)

## Project Overview
This project leverages the k-Nearest Neighbors (kNN) algorithm to predict obesity levels based on individuals' eating habits and physical conditions. The primary goal is to analyze the factors contributing to obesity and build a machine learning model that can classify individuals into various obesity categories.

### Dataset Description
The dataset contains attributes related to individuals' eating habits and physical conditions. Below is a breakdown of the features:

#### Eating Habits Attributes:
- **FAVC**: Frequent consumption of high caloric food.
- **FCVC**: Frequency of vegetable consumption.
- **NCP**: Number of main meals consumed daily.
- **CAEC**: Frequency of eating between meals.
- **CH20**: Daily water consumption.
- **CALC**: Alcohol consumption frequency.

#### Physical Condition Attributes:
- **SCC**: Monitoring of calorie intake.
- **FAF**: Frequency of physical activity.
- **TUE**: Time spent using technology devices.
- **MTRANS**: Primary mode of transportation.

#### Target Variable:
- **NObeyesdad**: Obesity levels, classified into multiple categories.

## Project Steps

### 1. Exploratory Data Analysis (EDA)
- Inspected the dataset structure, data types, and statistical summaries.
- Visualized relationships using heatmaps, box plots, scatter plots, and histograms.
- Handled outliers and missing values.

### 2. Data Preprocessing
- Encoded categorical variables using one-hot encoding and label encoding.
- Applied scaling using `StandardScaler` to standardize numerical features.
- Addressed class imbalance with SMOTE (Synthetic Minority Oversampling Technique).

### 3. Model Building
- Split the dataset into training and testing sets using an 80-20 split.
- Applied kNN with various distance metrics (Euclidean, Manhattan, Cosine).
- Used k-fold cross-validation to evaluate the model.
- Determined the optimal hyperparameters (e.g., number of neighbors) by comparing accuracy scores.

### 4. Model Evaluation
- Evaluated the kNN model using accuracy, confusion matrix, precision, recall, and F1-score.
- Analyzed both training and testing performance to ensure the model's generalizability.

## Results
- **Optimal k**: Found the best value of \( k = 7 \).
- **Best Metric**: Manhattan distance performed the best, achieving the highest accuracy.
- **Model Performance**: Achieved a high accuracy and balanced classification metrics for training and testing datasets.

## Key Files
1. **Dataset**: The dataset is loaded directly from an online source using a CSV file.
2. **Python Code**: Contains the implementation of data preprocessing, kNN model training, evaluation, and visualization.

## How to Run the Project
1. Clone this repository:
   ```bash
   git clone https://github.com/vaibhpande21/Obesity-Prediction-KNN.git
