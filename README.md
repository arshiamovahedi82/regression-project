# Regression Project

This repository contains a regression analysis project using Python. The project demonstrates how to preprocess housing data and build predictive models to estimate property prices based on various features. Below is a comprehensive guide to understanding and replicating this project.

---

## Project Overview
The goal of this project is to predict property prices using features such as area, room count, and availability of parking, warehouse, and elevator. The models applied include:
- **Linear Regression**
- **Random Forest Regressor**

Data preprocessing and visualization techniques are also covered.

---

## Requirements

To replicate this project, the following Python libraries are required:

```bash
pandas
matplotlib
seaborn
scikit-learn
```

Install them using pip if they are not already installed:

```bash
pip install pandas matplotlib seaborn scikit-learn
```

---

## Dataset

The dataset used contains information on housing prices along with the following columns:
- **Area**: Property area in square meters.
- **Room**: Number of rooms.
- **Parking**: Availability of parking (True/False).
- **Warehouse**: Availability of a warehouse (True/False).
- **Elevator**: Availability of an elevator (True/False).
- **Address**: Location of the property.
- **Price**: Price of the property in Iranian Toman.
- **Price (USD)**: Price of the property in USD.

---

## Steps

### 1. Data Exploration
The project begins with loading and exploring the dataset:
- Checking for missing values.
- Displaying descriptive statistics.

### 2. Data Preprocessing
The preprocessing steps include:
- Converting non-numeric columns to numeric where needed.
- Removing outliers based on thresholds for property area.
- Dropping rows with missing essential data (e.g., address).

### 3. Data Visualization
Several visualizations provide insights into the relationships between features and property prices:
- Scatter plot of **Area vs. Price**.
- Box plots for:
  - Price by number of rooms.
  - Price by availability of parking, warehouse, and elevator.

### 4. Model Building
Two predictive models are implemented:

#### **Linear Regression**
- Train/test split is performed.
- Model coefficients are examined to understand the influence of each feature.

#### **Random Forest Regressor**
- Used as a non-linear model to improve performance.

### 5. Results
The model performances are evaluated using:
- **Mean Squared Error (MSE)**
- **R² Score**

#### Results Summary:
| Model                  | MSE               | R² Score |
|------------------------|-------------------|------------|
| Linear Regression      | 3.54e+19         | 0.5319     |
| Random Forest Regressor| 2.04e+19         | 0.7303     |

### 6. Visualization of Predictions
A comparative scatter plot shows actual vs. predicted prices for both models.

---

## How to Run

1. Clone this repository:
   ```bash
   git clone <repository_url>
   cd <repository_name>
   ```

2. Ensure the dataset is available in the specified directory (update paths in the script if needed).

3. Run the project script step by step to understand the process or execute the entire script using:
   ```bash
   python regression_project.py
   ```

---

## Conclusion

This project highlights the steps for conducting a regression analysis on housing data. It compares two different machine learning models and evaluates their performance.

Feel free to explore the code and provide feedback or suggestions for improvement!

---

## Author
Arshia Movahedi

