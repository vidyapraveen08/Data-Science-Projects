
# Quarterly Retail Sales Tax Data Analysis

This project analyzes the Quarterly Retail Sales Tax Data by County and City, focusing on sales performance across different regions. The project includes data preprocessing, visualization, and the application of machine learning models to predict future taxable sales. The final deliverables include a detailed report, source code, and a video presentation.

## Project Structure

- **Notebook**: `SalesPerformanceAnalysisProject.ipynb` - Contains all the code and analysis for the project.
- **Data**: `Quarterly_Retail_Sales_Tax_Data_by_County_and_City.csv` - The dataset used in this project.
- **Final Report**: `DSC680-Week7Assignment_VidyaPraveen.pdf` - A comprehensive report detailing the project's objectives, methods, and findings.
- **Code Documentation**: `Project2Code.pdf` - Documentation of the code used in the project.
- **Presentation**: `Sales Performance Analysis.mp4` - A video presentation summarizing the project.

## Data

The data used in this project is a CSV file containing the following fields:

- **Fiscal Year**: The fiscal year of the data.
- **Quarter Ending**: The ending date of the quarter.
- **County_Number**: The identifier for the county.
- **County**: The name of the county.
- **City**: The name of the city.
- **Number of Returns**: The number of returns filed.
- **Taxable Sales**: The amount of taxable sales reported.
- **Computed Tax**: The tax computed based on the taxable sales.
- **Percent of Tax**: The percentage of the tax.
- **FIPS County Code**: The Federal Information Processing Standards (FIPS) code for the county.
- **Primary Lat Dec**: The primary latitude decimal of the county.
- **Primary Long Dec**: The primary longitude decimal of the county.

## Requirements

To run the notebook, you'll need the following Python libraries:

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `sklearn`

You can install these using pip:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Analysis Overview

1. **Data Loading and Preprocessing**:
   - Load the dataset and inspect the basic statistics.
   - Handle any missing or inconsistent data.

2. **Visualization**:
   - Explore the data through various plots such as time series plots and bar charts.
   - Visualize the relationship between different variables.

3. **Machine Learning**:
   - Split the data into training and testing sets.
   - Apply Linear Regression as a baseline model.
   - Use ARIMA and SARIMA models to capture temporal and seasonal patterns.
   - Evaluate the performance of the models using MAE, MSE, RMSE, and cross-validation scores.

4. **Report and Presentation**:
   - The final report details the entire analysis process, including challenges, assumptions, and recommendations.
   - The video presentation provides an overview of the project's findings and implications.

## How to Use

1. Clone this repository.
2. Download the dataset and place it in the same directory as the notebook.
3. Open the `SalesPerformanceAnalysisProject.ipynb` notebook in Jupyter Notebook or JupyterLab.
4. Run the notebook cells to reproduce the analysis.
5. Review the `DSC680-Week7Assignment_VidyaPraveen.pdf` report for a detailed understanding of the project.
6. Watch the `Sales Performance Analysis.mp4` video presentation for a summary of the key findings.

## Authors

- Vidya Praveen

