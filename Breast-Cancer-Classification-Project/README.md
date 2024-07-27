# Breast Cancer Classification Project

## Background Information

The objective of this project is to build a model to classify breast cancer based on various medical measurements. The dataset contains features computed from a digitized image of a fine needle aspirate (FNA) of a breast mass. The features describe characteristics of the cell nuclei present in the image. This classification model will help in predicting whether the breast cancer is benign or malignant.

## Problem Statement and Business Goals

Building an accurate model to classify breast cancer as benign or malignant is crucial for early detection and treatment. This will assist healthcare professionals in making informed decisions, optimizing patient care, and potentially saving lives by enabling timely interventions.

## Methodology

### Data Copying and Cleaning

- **Import the dataset:** Load the data from a CSV file.
- **Recategorize data:** Convert categorical features to the appropriate data types.
- **Check for null values:** Identify and handle missing values if any.
- **Drop duplicate values:** Ensure the dataset is free from duplicate entries.

### Exploratory Data Analysis

- **Graphs and visualizations:** Conduct exploratory data analysis (EDA) using various graphs to understand the data distribution and relationships between features.
- **Interpret the graphs:** Draw insights from visualizations to inform further analysis and modeling steps.

### Feature Engineering

- **Check for outliers:** Identify and handle outliers in the dataset.
- **Correlation analysis:** Analyze the correlation between features to identify important predictors.
- **One-hot encoding:** Perform encoding for categorical features if necessary.
- **Feature selection:** Select relevant features for modeling.

### Data Handling

- **Imbalance handling:** Apply oversampling techniques (e.g., SMOTE) to handle class imbalance in the target variable.

### Model Building

- **Train-test split:** Split the data into training and testing sets.
- **Standardization:** Standardize the features using `StandardScaler`.
- **Base models:** Create and evaluate different models including SVM, Random Forest, and XGBoost.

### Model Validation

- **Model diagnostics:** Evaluate models using accuracy, precision, recall, confusion matrix, and other metrics.
- **Best model selection:** Choose the model with the highest accuracy and performance on validation metrics.

### Model Testing on Test Data

- **Load test data:** Import the test dataset and preprocess it as done with training data.
- **Prediction:** Use the trained model to make predictions on the test data.

### Model Output Saving

- **Save predictions:** Save the predicted results along with IDs in a CSV file.
- **Export the results:** Store the results for further analysis and reporting.

## Conclusions

- From the dataset, we found distinct patterns that differentiate benign and malignant tumors.
- Features such as texture, area, smoothness, and compactness have significant importance in classifying the diagnosis.
- The models built provide reliable accuracy and can be used to assist in the early detection of breast cancer.

## Model Results

The following table summarizes the evaluation metrics of the different models used:

| Model         | Accuracy | Precision | Recall | F1 Score |
|---------------|----------|-----------|--------|----------|
| SVM           | 0.97     | 0.96      | 0.95   | 0.96     |
| Random Forest | 0.96     | 0.95      | 0.94   | 0.95     |
| XGBoost       | 0.98     | 0.97      | 0.96   | 0.97     |

The XGBoost classifier showed the highest accuracy and F1 score, making it the best model for this classification task.

## Contribution

We are still learning and open to contributions. If you have suggestions or improvements, feel free to contribute to this project. Thank you!
