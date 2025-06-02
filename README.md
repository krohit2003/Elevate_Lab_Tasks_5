# Elevate_Lab_Tasks_5
INTERN AT ELEVATE LABS TASKS

# Heart Disease Prediction using Decision Tree and Random Forest

This project uses a heart disease dataset to train and evaluate classification models (Decision Tree and Random Forest) to predict whether a patient has heart disease or not.

## 📁 Dataset

- File: `heart.csv`
- Target Column: `target` (1 = Disease, 0 = No Disease)
- Features: Various health parameters such as age, cholesterol, resting blood pressure, maximum heart rate, etc.

## 📌 Steps Performed

### 1. Load and Explore the Dataset
- Read `heart.csv` into a pandas DataFrame.
- Display the shape and the first few rows.

### 2. Data Preparation
- `X`: Feature matrix (all columns except `target`)
- `y`: Target labels (`target`)
- Split into training and testing sets (70% train, 30% test)

### 3. Decision Tree Classifier
- Train a Decision Tree with `max_depth=10`
- Visualize the decision tree structure
- Compute accuracy on both training and testing data
- Analyze overfitting by comparing train vs test accuracy

### 4. Random Forest Classifier
- Train a Random Forest with 100 estimators
- Compare its test accuracy with the Decision Tree

### 5. Feature Importance
- Visualize which features are most important using Random Forest

### 6. Cross-Validation
- Evaluate both models using 5-fold cross-validation

## 📊 Model Performance

- **Decision Tree Accuracy** (Test Set)
- **Random Forest Accuracy**
- **Cross-Validation Scores** for both models
- Visualization of feature importances and decision tree

## 📦 Libraries Used

- `pandas`
- `matplotlib`
- `seaborn`
- `sklearn` (`DecisionTreeClassifier`, `RandomForestClassifier`, `train_test_split`, `cross_val_score`, etc.)

## 📉 How Overfitting is Analyzed

Overfitting is identified by a **high training accuracy** but **low testing accuracy**.  
To reduce overfitting:
- The tree depth is controlled using `max_depth` in `DecisionTreeClassifier`.

---

