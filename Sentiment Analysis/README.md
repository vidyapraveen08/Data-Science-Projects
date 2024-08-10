
# Sentiment Analysis of Amazon Product Reviews

This project focuses on analyzing the sentiment of Amazon product reviews using Natural Language Processing (NLP) techniques. The analysis includes data preprocessing, text normalization, and the application of machine learning models to classify sentiments.

## Project Structure

- **Notebook**: `SentimentAnalysisProject.ipynb` - Contains all the code and analysis for the project.
- **Data**: `amazon_review.csv` - The dataset used for sentiment analysis.
- **Final Report**: `DSC680-Project3-FinalReport.pdf` - A comprehensive report detailing the project.
- **Code Documentation**: `Project3Code.pdf` - Documentation of the code used in the project.

## Data

The dataset contains the following fields:

- **reviewerID**: Unique identifier for the reviewer.
- **asin**: Amazon Standard Identification Number (ASIN) for the product.
- **reviewText**: The full text of the review.
- **overall**: The rating given by the reviewer (1-5).
- **summary**: A brief summary of the review.
- **reviewTime**: The date when the review was posted.
- **day_diff**: The difference in days from the review date to the current date.
- **helpful_yes**: The number of "helpful" votes the review received.
- **total_vote**: The total number of votes the review received.

## Requirements

To run the notebook, you'll need the following Python libraries:

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `nltk`
- `sklearn`

You can install these using pip:

```bash
pip install pandas numpy matplotlib seaborn nltk scikit-learn
```

## Analysis Overview

1. **Data Loading and Preprocessing**:
   - Load the dataset and inspect the basic statistics.
   - Handle missing values, if any, and preprocess the text data.

2. **Text Normalization**:
   - Convert text to lowercase, remove stop words, punctuation, and apply lemmatization.
   - Tokenize the text into individual words.

3. **Sentiment Analysis**:
   - Use machine learning models such as Logistic Regression, Naive Bayes, and LSTM (Long Short-Term Memory) to classify sentiments.
   - Evaluate models using accuracy, precision, recall, F1-score, and ROC-AUC metrics.

4. **Visualization**:
   - Visualize sentiment trends over time and across different product categories.
   - Display sentiment distribution for top-selling products.

5. **Report and Presentation**:
   - The final report details the entire analysis process, including challenges, assumptions, and recommendations.

## How to Use

1. Clone this repository.
2. Download the dataset and place it in the same directory as the notebook.
3. Open the `SentimentAnalysisProject.ipynb` notebook in Jupyter Notebook or JupyterLab.
4. Run the notebook cells to reproduce the analysis.
5. Review the `DSC680-Project3-FinalReport.pdf` report for a detailed understanding of the project.

## License

This project is licensed under the MIT License.
