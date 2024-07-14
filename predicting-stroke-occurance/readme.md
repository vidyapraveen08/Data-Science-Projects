# Stroke Prediction Model

## Introduction
This project aims to develop a predictive model for stroke occurrence based on a dataset of patient health records. Predicting strokes can help in early intervention and potentially save lives by identifying high-risk individuals and managing their health proactively.

## Dataset
The dataset used in this project is the "Healthcare Dataset Stroke Data," containing various health-related attributes of patients.

### Dataset Features
- **id:** Unique identifier for each patient.
- **gender:** Gender of the patient.
- **age:** Age of the patient.
- **hypertension:** Whether the patient has hypertension (0: No, 1: Yes).
- **heart_disease:** Whether the patient has heart disease (0: No, 1: Yes).
- **ever_married:** Marital status of the patient.
- **work_type:** Type of work the patient does.
- **Residence_type:** Type of residence (Urban/Rural).
- **avg_glucose_level:** Average glucose level of the patient.
- **bmi:** Body mass index of the patient.
- **smoking_status:** Smoking status of the patient.
- **stroke:** Whether the patient had a stroke (0: No, 1: Yes).

## Data Preparation
- **Handling Missing Values:** Missing values in the 'bmi' column were filled using interpolation to maintain data integrity.
- **Encoding Categorical Variables:** Categorical variables such as 'gender,' 'ever_married,' 'work_type,' 'Residence_type,' and 'smoking_status' were encoded to numerical values for model training.

## Exploratory Data Analysis (EDA)
EDA was performed to understand the distribution of data and identify patterns. Key visualizations include:
- Distribution plots for numerical features.
- Correlation matrix to identify relationships between features.
- Feature importance analysis to determine the most influential factors for stroke prediction.

## Modeling Approach
Several machine learning algorithms were used to develop the predictive model, including:
- Logistic Regression
- Random Forest
- Gradient Boosting

The models were evaluated based on accuracy, precision, recall, and F1-score.

## Results
The Gradient Boosting model provided the best performance, achieving high accuracy, precision, and recall on the test dataset. The most important features for predicting strokes were age, average glucose level, and body mass index (BMI).

## Conclusion
The Gradient Boosting model is effective for predicting strokes and can be used for early intervention strategies. The model highlights the significance of regular health monitoring, especially for older adults and those with higher glucose levels and BMI.

## Recommendations
- **Continuous Monitoring:** Implement a system for ongoing model monitoring and regular assessment.
- **Feedback Mechanism:** Establish a feedback loop with healthcare providers to continuously improve the model.
- **Periodic Updates:** Regularly update the model to adapt to new data and changing health trends.

## Ethical Considerations
Ensuring the privacy and fairness of patient data is crucial. Strategies include:
- Data anonymization to protect patient identity.
- Fairness-aware algorithms to mitigate bias in predictions.

## References
- Kaggle: [Healthcare Dataset Stroke Data](https://www.kaggle.com/fedesoriano/stroke-prediction-dataset)
- Scikit-learn Documentation: [Scikit-learn](https://scikit-learn.org/stable/documentation.html)

## Usage
To run the project, use the provided Jupyter notebook `projectcode.ipynb` and dataset `healthcare-dataset-stroke-data.csv`. Ensure you have the required libraries installed, including pandas, numpy, scikit-learn, and matplotlib.

### Installation
```bash
pip install pandas numpy scikit-learn matplotlib
```

### Launch Jupyter Notebook:
    ```bash
    jupyter notebook
    ```

### Open and run the `ProjectCode.ipynb` notebook to execute the analysis.
