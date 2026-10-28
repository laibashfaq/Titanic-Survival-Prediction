# Titanic Survival Prediction 🚢

An end-to-end Machine Learning project that explores passenger survival on the Titanic using data analysis, feature engineering, classification models, and model evaluation.

## 📌 Project Overview

This project investigates the factors associated with passenger survival on the Titanic and compares multiple machine learning algorithms to predict whether a passenger survived.

The notebook covers the complete workflow, from data loading and exploratory data analysis (EDA) to model training, hyperparameter tuning, and performance evaluation.

## 🎯 Objectives

- Explore the Titanic passenger dataset and identify patterns in survival.
- Analyze missing values and relationships between passenger features and survival.
- Perform data preprocessing and feature engineering.
- Train and compare multiple classification algorithms.
- Evaluate model performance using appropriate classification metrics.
- Identify important features associated with survival predictions.

## 📂 Project Structure

```text
titanic-survival-prediction/
│
├── README.md
├── Titanic_Analysis.ipynb
├── titanic.csv
└── requirements.txt
```

## 🛠️ Technologies Used

- **Python** — programming language
- **Pandas & NumPy** — data manipulation and numerical operations
- **Matplotlib & Seaborn** — data visualization
- **Scikit-learn** — preprocessing, model training, cross-validation, hyperparameter tuning, and evaluation
- **Jupyter Notebook / Google Colab** — interactive development environment

## 📊 Project Workflow

### 1. Data Loading and Exploration

- Load the Titanic dataset containing 891 passenger records.
- Inspect the dataset structure, descriptive statistics, and duplicate records.
- Analyze missing values and the distribution of the target variable, `Survived`.

### 2. Exploratory Data Analysis (EDA)

Investigate survival patterns based on:

- Gender
- Passenger class
- Age
- Fare
- Port of embarkation
- Number of siblings, spouses, parents, and children aboard

Visualizations include survival distributions, survival rates, age distributions, fare comparisons, and correlation analysis.

### 3. Data Preprocessing and Feature Engineering

The notebook includes:

- Missing-value imputation for age and embarkation port.
- Extraction of passenger titles from names.
- Creation of family size and solo-traveler indicators.
- Cabin availability and deck features.
- Ticket group size and fare-per-person features.
- Age groups and a women-and-children indicator.
- Categorical encoding and removal of unused columns.

### 4. Model Training

The following classification algorithms are compared:

- Logistic Regression
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)
- Random Forest
- Gradient Boosting

Stratified 5-fold cross-validation is used for baseline model comparison. Grid search is applied to tune Random Forest and Gradient Boosting hyperparameters.

### 5. Model Evaluation

Models are evaluated on a held-out test set using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Classification report
- Confusion matrix
- ROC curves

The notebook also visualizes feature importance from the tuned Random Forest model.

## 🔎 Key Findings

The exploratory analysis highlights several patterns:

- Female passengers had substantially higher survival rates than male passengers.
- First-class passengers generally had better survival outcomes than passengers in lower classes.
- Passenger titles, gender-related features, and fare-related features provide useful predictive information.
- Family composition and passenger characteristics can help explain differences in survival outcomes.

The notebook reports approximately 80–82% test accuracy and 0.84–0.86 ROC-AUC across the evaluated models. Logistic Regression is reported as the best model on the held-out test set by ROC-AUC, with approximately 81.6% accuracy and 0.863 ROC-AUC.

These results are specific to the notebook's train/test split and should not be interpreted as guaranteed performance on new data.

## 🚀 Getting Started

### Prerequisites

Install Python and the required libraries.

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/YOUR-USERNAME/titanic-survival-prediction.git
   ```

2. Navigate to the project directory:

   ```bash
   cd titanic-survival-prediction
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Open the notebook:

   ```bash
   jupyter notebook Titanic_Analysis.ipynb
   ```

5. Run the notebook cells sequentially.

**Note:** Keep `titanic.csv` in the project directory. If the dataset is not included, obtain it from the original dataset source and update the data path as needed. The CSV must have the column names expected by the notebook.

## 📈 Future Improvements

- Add repeated cross-validation for more stable performance estimates.
- Explore surname-based family survival features.
- Investigate ensemble methods and stacking.
- Perform additional feature selection and error analysis.
- Develop a simple interface for interactive survival predictions.

## 📚 Learning Outcomes

This project demonstrates practical experience with:

- Exploratory Data Analysis
- Data Cleaning and Preprocessing
- Feature Engineering
- Supervised Machine Learning
- Classification Algorithms
- Cross-Validation and Hyperparameter Tuning
- Model Evaluation and Visualization

## 👩‍💻 Author

**Laiba Ashfaq**

Computer Science Graduate | Interested in Artificial Intelligence, Machine Learning, and Data Analysis.

## 📄 License

A license has not yet been specified. If you decide to make the project open source, add a license appropriate to your intended use and ensure that the dataset's terms permit redistribution.
