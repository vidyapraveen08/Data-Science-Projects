# Ames Housing Price Prediction

## Introduction
This project aims to predict housing prices in Ames, Iowa, using various features from the Ames Housing dataset. The project includes data preprocessing, exploratory data analysis (EDA), feature engineering, model building, and evaluation.

## Dataset
The dataset used in this project is the "AmesHousing.csv," containing 82 features related to housing attributes.

### Dataset Features
- **Order:** Identifier for the observation.
- **PID:** Parcel identification number.
- **MS SubClass:** Identifies the type of dwelling involved in the sale.
- **MS Zoning:** Identifies the general zoning classification of the sale.
- **Lot Frontage:** Linear feet of street connected to property.
- **LotArea:** Lot size in square feet.
- **Street:** Type of road access.
- **Alley:** Type of alley access.
- **Lot Shape:** General shape of property.
- **Land Contour:** Flatness of the property.
- **Utilities:** Type of utilities available.
- **Lot Config:** Lot configuration.
- **Land Slope:** Slope of property.
- **Neighborhood:** Physical locations within Ames city limits.
- **Condition 1:** Proximity to main road or railroad.
- **Condition 2:** Proximity to main road or railroad (if a second is present).
- **Bldg Type:** Type of dwelling.
- **House Style:** Style of dwelling.
- **Overall Qual:** Rates the overall material and finish of the house.
- **Overall Cond:** Rates the overall condition of the house.
- **Year Built:** Original construction date.
- **Year Remod/Add:** Remodel date.
- **Roof Style:** Type of roof.
- **Roof Matl:** Roof material.
- **Exterior 1st:** Exterior covering on house.
- **Exterior 2nd:** Exterior covering on house (if more than one material).
- **Mas Vnr Type:** Masonry veneer type.
- **Mas Vnr Area:** Masonry veneer area in square feet.
- **Exter Qual:** Evaluates the quality of the material on the exterior.
- **Exter Cond:** Evaluates the present condition of the material on the exterior.
- **Foundation:** Type of foundation.
- **Bsmt Qual:** Evaluates the height of the basement.
- **Bsmt Cond:** Evaluates the general condition of the basement.
- **Bsmt Exposure:** Refers to walkout or garden level walls.
- **BsmtFin Type 1:** Rating of basement finished area.
- **BsmtFin SF 1:** Type 1 finished square feet.
- **BsmtFin Type 2:** Rating of basement finished area (if multiple types).
- **BsmtFin SF 2:** Type 2 finished square feet.
- **Bsmt Unf SF:** Unfinished square feet of basement area.
- **Total Bsmt SF:** Total square feet of basement area.
- **Heating:** Type of heating.
- **Heating QC:** Heating quality and condition.
- **Central Air:** Central air conditioning.
- **Electrical:** Electrical system.
- **1st Flr SF:** First-floor square feet.
- **2nd Flr SF:** Second-floor square feet.
- **Low Qual Fin SF:** Low quality finished square feet (all floors).
- **Gr Liv Area:** Above grade (ground) living area square feet.
- **Bsmt Full Bath:** Basement full bathrooms.
- **Bsmt Half Bath:** Basement half bathrooms.
- **Full Bath:** Full bathrooms above grade.
- **Half Bath:** Half baths above grade.
- **Bedroom:** Number of bedrooms above basement level.
- **Kitchen:** Number of kitchens.
- **Kitchen Qual:** Kitchen quality.
- **TotRms AbvGrd:** Total rooms above grade (does not include bathrooms).
- **Functional:** Home functionality rating.
- **Fireplaces:** Number of fireplaces.
- **Fireplace Qu:** Fireplace quality.
- **Garage Type:** Garage location.
- **Garage Yr Blt:** Year garage was built.
- **Garage Finish:** Interior finish of the garage.
- **Garage Cars:** Size of garage in car capacity.
- **Garage Area:** Size of garage in square feet.
- **Garage Qual:** Garage quality.
- **Garage Cond:** Garage condition.
- **Paved Drive:** Paved driveway.
- **Wood Deck SF:** Wood deck area in square feet.
- **Open Porch SF:** Open porch area in square feet.
- **Enclosed Porch:** Enclosed porch area in square feet.
- **3Ssn Porch:** Three season porch area in square feet.
- **Screen Porch:** Screen porch area in square feet.
- **PoolArea:** Pool area in square feet.
- **Pool QC:** Pool quality.
- **Fence:** Fence quality.
- **Misc Feature:** Miscellaneous feature not covered in other categories.
- **Misc Val:** Value of miscellaneous feature.
- **Mo Sold:** Month sold.
- **Yr Sold:** Year sold.
- **Sale Type:** Type of sale.
- **Sale Condition:** Condition of sale.
- **SalePrice:** Sale price of the property.

## Project Workflow
The project is structured as follows:

### Data Preprocessing
- **Handling Missing Values:** Missing values were handled using various imputation methods based on the nature of the feature.
- **Encoding Categorical Variables:** Categorical features were encoded to numerical values for model training.

### Exploratory Data Analysis (EDA)
- Distribution plots and histograms for numerical features.
- Boxplots to detect outliers.
- Correlation matrix to identify relationships between features.
- Scatter plots to explore relationships between variables.

### Feature Engineering
- Creating new features based on domain knowledge.
- Transforming existing features to better capture the underlying patterns in the data.

### Model Building
Several machine learning models were built and evaluated, including:
- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor

### Model Evaluation
Models were evaluated based on:
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R-squared score

## Results
The Random Forest Regressor provided the best performance, demonstrating high accuracy and robustness in predicting housing prices. Key features influencing house prices included overall quality, above ground living area, and garage area.

## Conclusion
The project successfully developed a robust model for predicting housing prices in Ames, Iowa. The insights gained from the model can help stakeholders make informed decisions regarding property investments and valuations.

## Recommendations
- **Continuous Model Monitoring:** Implement a system for ongoing model performance monitoring and regular updates.
- **Feature Importance Analysis:** Regularly review feature importance to understand the driving factors behind model predictions.
- **Further Research:** Explore additional features and advanced modeling techniques to enhance prediction accuracy.

## Ethical Considerations
- **Data Privacy:** Ensure that the data used is anonymized to protect individuals' privacy.
- **Fairness:** Implement fairness-aware algorithms to prevent bias in predictions.

## Usage
To run the project, use the provided R Markdown file `assignment_11-3_PraveenVidya.Rmd` and dataset `AmesHousing.csv`. Ensure you have the required libraries installed.

### Installation
```r
install.packages(c("tidyverse", "caret", "randomForest", "xgboost"))
```

### Running the R Markdown file
Open the R Markdown file and execute the code chunks to preprocess the data, train the models, and evaluate their performance.
```r
rmarkdown::render("assignment_11-3_PraveenVidya.Rmd")
```
