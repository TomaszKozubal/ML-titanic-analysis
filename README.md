# Titanic Data Analysis and Classification Project

This repository contains a series of data analysis and machine learning experiments conducted on the Titanic dataset. The project includes feature engineering, exploratory data analysis, and implementation of classification models like Decision Trees and Logistic Regression.

---

## Project Structure

1. **Titanic Data Analysis**  
   - Data cleaning and preprocessing
   - Exploratory analysis on survival rates
   - Visualization and statistical insights

2. **Decision Tree Classifier**  
   - Implementation of a basic decision tree classifier
   - Evaluation metrics: confusion matrix, precision, recall, F1-score
   - Feature importance analysis
   - Model pruning using cost-complexity parameter `ccp_alpha`

3. **Logistic Regression**  
   - Model fitting for comparison
   - Analysis of results vs. pruned decision tree

4. **Bootstrapping**  
   - Separate bootstrapping project for enhanced statistical analysis

---

## Data Preprocessing

- Removed irrelevant columns (`PassengerId`, `Name`, `SibSp`, `Parch`, `Ticket`, `Cabin`, `Embarked`)
- Handled missing values
- Converted categorical data (`Sex`) to numeric
- Split dataset into training and testing sets (70:30)

---

## Models and Results

### Decision Tree Classifier
- Basic model achieved **70% accuracy**.
- Pruned model with `ccp_alpha = 0.1` improved accuracy to **77%**, with better precision and recall for classifying survivors.

### Logistic Regression
- Achieved **70.2% accuracy**, slightly less effective than the pruned decision tree.

### Feature Importance (Decision Tree)
| Feature | Importance |
|---------|------------|
| Pclass  | 0.1133     |
| Sex     | 0.3134     |
| Age     | 0.2741     |
| Fare    | 0.2992     |

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your_username/titanic-classification.git
   cd titanic-classification
