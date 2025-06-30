# Task 5 – Decision Trees & Random Forest (AI & ML Internship)

This notebook is part of my AI & ML Internship assignment focused on learning tree-based models for classification. For this task, I used the Heart Disease Dataset from Kaggle to build and compare two popular models: Decision Tree and Random Forest.

## Dataset

I used the publicly available [Heart Disease Dataset](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset) from Kaggle. It contains 1025 rows and 14 columns, including patient data such as age, cholesterol, and resting blood pressure. There is also a target column that shows whether the person has heart disease (1) or not (0).

## What I Did

1. **Data Loading & Exploration**  
   I loaded the dataset using Pandas, checked for null values and data types, and gained a basic understanding of each feature.

2. **Model Training**  
   - I first trained a **Decision Tree Classifier** using Scikit-learn. It achieved high accuracy (~99%), but it was clearly overfitting.
   - Then, I limited the tree depth to 3. This reduced overfitting, but the accuracy dropped to ~78%.
   - Finally, I trained a **Random Forest Classifier** with 100 trees. This model performed the best, achieving about **98.5%** accuracy on the test set.

3. **Model Evaluation**  
   - I evaluated the models using a classification report and accuracy score.
   - I plotted the full Decision Tree for visualization.
   - I also performed **5-fold cross-validation** on both models to compare their performance.

4. **Feature Importance**  
   - I plotted the feature importances from the Random Forest.
   - The most influential features were `cp` (chest pain), `thalach` (maximum heart rate), and `oldpeak`.

## Key Results

- **Decision Tree Accuracy**: ~99% (with default settings), ~78% when depth is limited
- **Random Forest Accuracy**: ~98.5%
- **Cross-validation (5-fold)**:
  - Decision Tree: ~97.0%
  - Random Forest: ~99.7%

Random Forest clearly outperformed the Decision Tree in terms of both accuracy and stability.

## Included in this Repository

- heart_analysis.ipynb – Notebook with all code, visualizations, and results
- Feature importance and tree diagrams (generated using matplotlib)
- Screenshots of outputs and visualizations
- This README file

## Tech Stack

- Python
- Pandas & NumPy
- scikit-learn
- matplotlib & seaborn
- Jupyter Notebook (Kaggle environment)
