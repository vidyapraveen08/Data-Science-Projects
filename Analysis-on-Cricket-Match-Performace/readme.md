
# Cricket Match Data Analysis

## Description

This project analyzes cricket match data, focusing on matches played in the Asia Cup. The analysis includes data loading, cleaning, exploratory data analysis (EDA), and visualizations to uncover insights and trends.

## Installation

To run this project, you need to have Python installed along with the following libraries:
- pandas
- numpy
- matplotlib
- seaborn
- jupyter

You can install the required libraries using pip:
```bash
pip install pandas numpy matplotlib seaborn jupyter
```

## Usage

1. Clone the repository or download the notebook and the CSV file.
2. Open the Jupyter notebook:
```bash
jupyter notebook CricketmatchDataAnalysis.ipynb
```
3. Run the cells sequentially to perform data analysis on the provided dataset (`asiacup.csv`).

## Data

The dataset `asiacup.csv` contains information about cricket matches played in the Asia Cup. The columns in the dataset are:
- **Match**: The match number.
- **Date**: The date of the match.
- **Team1**: The first team.
- **Team2**: The second team.
- **Winner**: The winner of the match.
- **Margin**: The winning margin.
- **Ground**: The ground where the match was played.
- **Match_Id**: A unique identifier for the match.

## Analysis Steps

1. **Data Loading**: Load the dataset and examine the structure.
2. **Data Cleaning**: Handle missing values, correct data types, and remove duplicates.
3. **Data Analysis**: Perform exploratory data analysis to identify patterns and trends.
4. **Visualization**: Create visualizations to better understand the data.
5. **Conclusion**: Summarize the findings from the analysis.

## Results and Discussion

The project involved data preprocessing, exploratory data analysis (EDA), and machine learning model development and evaluation. The goal was to derive insights from the data and predict match outcomes.

### Key Findings:

1. **Data Preprocessing**:
   - Missing values in 'Run Scored' and 'Wicket Lost' were filled with median values.
   - Categorical to numerical conversion was applied to the 'Result' column.
   - A new feature 'Run Rate' was created.

2. **Exploratory Data Analysis (EDA)**:
   - Basic statistics and visualizations were used to understand the distribution of runs scored and their relationship with match outcomes.

3. **Modeling**:
   - A Random Forest Classifier was trained and evaluated.
   - The model achieved notable accuracy in predicting match outcomes.
   - Feature importance analysis highlighted 'Run Rate' as a significant predictor.

### Model Evaluation:

- **Accuracy**: The model's accuracy on the test set was 70.59%.

- **Classification Report**: 
   -  **Class 0 (Lose):**
      -  Precision: 0.75
      -  Recall: 0.60
      -  F1-Score: 0.67
      -  Support: 25
   -  **Class 1 (Win):**
      -   Precision: 0.68
      -   Recall: 0.81
      -   F1-Score: 0.74
      -   Support: 26
   -  **Macro Average:**
      -   Precision: 0.71
      -   Recall: 0.70
      -   F1-Score: 0.70
      -   Support: 51
   -  **Weighted Average:**
      -   Precision: 0.71
      -   Recall: 0.71
      -   F1-Score: 0.70
      -   Support: 51

- **Confusion Matrix**: True positive, true negative, false positive, and false negative counts were detailed.

### Detailed Results:

- **Accuracy**: The Random Forest Classifier achieved an accuracy of [add specific value] on the test set.
- **Classification Report**: The precision, recall, and F1-score for the classes (Win/Lose) were as follows:
  - **Precision**: [add values]
  - **Recall**: [add values]
  - **F1-Score**: [add values]
- **Confusion Matrix**: The confusion matrix showed the following counts:
  - **True Positives**: [add count]
  - **True Negatives**: [add count]
  - **False Positives**: [add count]
  - **False Negatives**: [add count]

### Discussion:

The analysis demonstrated that 'Run Rate' was a significant predictor of match outcomes. The Random Forest Classifier effectively identified patterns in the data, achieving high accuracy. The model's performance suggests it could be useful for predicting future match outcomes based on historical data.

## Authors

- Vidya Praveen
