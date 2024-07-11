Insurance Data Science Project
This repository contains code and resources for a data science project focusing on predicting insurance charges based on various factors.

-Dataset
The dataset used for this project (`insurance.csv`) contains the following columns:
- `age`: Age of the insured person.
- `sex`: Gender of the insured person (male/female).
- `bmi`: Body mass index (BMI) of the insured person.
- `children`: Number of children/dependents covered by the insurance plan.
- `smoker`: Smoking status of the insured person (yes/no).
- `region`: Region where the insured person resides.

-Project Structure
- `README.md`: Overview of the project and setup instructions.
- `insurance.csv`: Dataset file.
- `insurance_analysis.ipynb`: Jupyter notebook containing the code for data exploration, preprocessing, model training, and evaluation.
- `requirements.txt`: List of Python dependencies required to run the code.

-Code Overview
The Jupyter notebook (`insurance_analysis.ipynb`) includes the following sections:
1. **Data Loading and Exploration**:
   - Loading the dataset from `insurance.csv`.
   - Exploring basic statistics and information about the dataset.
2. **Data Preprocessing**:
   - Handling missing values (if any).
   - Encoding categorical variables (`sex`, `smoker`, `region`) using LabelEncoder.
   - Dropping original categorical columns.
3. **Exploratory Data Analysis (EDA)**:
   - Visualizing correlations between variables using heatmap.
   - Creating pair plots and scatter plots to understand relationships between features and insurance charges, differentiated by smoking status.
4. **Feature Engineering**:
   - Scaling numerical features using StandardScaler.
   - Adding polynomial features to capture non-linear relationships.
5. **Model Building and Evaluation**:
   - Training and evaluating several regression models:
     - Linear Regression
     - Ridge Regression
     - Random Forest Regression
     - Support Vector Regressor (SVR) with hyperparameter tuning using RandomizedSearchCV.
6. **Performance Comparison**:
   - Comparing the performance (R^2 score and RMSE) of all models using bar plots.
7. **Conclusion**:
   - Summary of findings and insights from the analysis.

-Requirements
To run the code, ensure you have the following Python libraries installed:
pandas
scikit-learn
matplotlib
seaborn
numpy
You can install these dependencies using pip:
pip install -r requirements.txt

This README provides an overview of the project, its structure and how to set up the environment.
