# Diabetes Prediction System using Pima Indian Dataset

This project is a machine learning application to predict diabetes using the **Pima Indian Diabetes Dataset**. It includes a **Tkinter-based GUI** for individual and batch predictions, and features a **Login and Registration system** to manage user access securely.

---

## Features

- **Authentication System:**
  - User **Registration** with secure password hashing.
  - **Login** functionality with input validation.
  - Encrypted user credentials storage.
  
- **Machine Learning Models:**
  - Random Forest Classifier
  - K-Nearest Neighbors (KNN)
  - Ensemble Voting Classifier (Soft Voting)

- **Exploratory Data Analysis (EDA):**
  - Visualizations (Histograms, Boxplots, Pairplots, Correlation Heatmap)

- **GUI:**
  - Predict individual diabetes outcomes.
  - Batch prediction from CSV files.
  - Light/Dark themes.
  - Validation of inputs.
  - Save prediction results.

- **Model Persistence:** Save and load trained models with `joblib`.

---

## Table of Contents
1. [Installation](#installation)
2. [Authentication System](#authentication-system)
3. [Dataset](#dataset)
4. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
5. [Machine Learning Workflow](#machine-learning-workflow)
6. [Tkinter GUI Application](#tkinter-gui-application)
7. [Results](#results)
8. [Usage](#usage)
9. [Contributing](#contributing)
10. [License](#license)

---

## Authentication System

Before using the prediction system, users must register and log in through a secure interface. This ensures that only authorized users can access the application.


## Dataset

- **Name:** Pima Indian Diabetes Dataset
- **Description:** This dataset contains medical diagnostic measurements for predicting the onset of diabetes based on specific factors. It has 768 entries with 8 features and a target variable (`Outcome`).

---

## Machine Learning Workflow

### Steps:
1. **Data Preprocessing:**
   - Handle missing values using median imputation.
   - Address outliers using the **IQR method**.
   - Scale features using `StandardScaler`.

2. **Class Imbalance Handling:**
   - Applied **SMOTETomek** for oversampling the minority class and undersampling the majority class.

3. **Model Training:**
   - Models Used:
     - Random Forest Classifier
     - K-Nearest Neighbors (KNN)
     - Ensemble Voting Classifier
   - Train-Test Split: 80%-20% with stratification.

4. **Model Evaluation:**
   - Metrics:
     - Confusion Matrix
     - Accuracy
     - Classification Report
     - ROC-AUC Score

---

## Tkinter GUI Application

The **Tkinter-based GUI** provides an intuitive interface for predictions.

- **Individual Predictions:** Enter patient data manually.
- **Batch Predictions:** Load and predict multiple records from a CSV file.
- **Themes:** Switch between Light/Dark themes.
- **Help Section:** Tooltips for input fields and detailed instructions.


---

## Results

### Model Performance:
| Metric               | Score  |
|----------------------|--------|
| **Accuracy**         | 86%    |
| **ROC-AUC Score**    | 92%    |

---

## Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository.
2. Create a new branch 
3. Commit your changes.
4. Push to the branch.
5. Open a Pull Request.

---

## License

This project is licensed under the Creative Commons Legal Code License. See the `LICENSE` file for details.
