

**README.md**

# Sentiment Analysis on Restaurant Reviews (Pandas and NumPy)

This repository contains a Python script that performs sentiment analysis on restaurant reviews using only the pandas and numpy libraries.

## Requirements

- Python 3.x
- pandas
- numpy

## Usage

1. **Install Dependencies**: Install the required Python libraries using pip:

   ```bash
   pip install pandas numpy
   ```

2. **Prepare the Dataset**: Ensure that you have a CSV file named `Restaurant_Reviews.csv` with a column named `review` containing the text of the restaurant reviews.

3. **Run the Script**: Run the Python script to classify the sentiment of the reviews:

   ```bash
   python sentiment_analysis.py
   ```

## Output

The script will output a table with the review text and the corresponding sentiment classification as either "Positive review", "Negative review", or "Neutral review".

## How it Works

1. **Data Loading**: The script loads the restaurant reviews dataset from the `restaurant_reviews.csv` file using the `pd.read_csv` function.

2. **Sentiment Classification**: The `classify_sentiment` function is defined to classify the sentiment of a review. It checks for the presence of positive and negative keywords in the review text and returns the appropriate sentiment classification.

3. **Sentiment Application**: The `classify_sentiment` function is applied to the `review` column of the DataFrame using the `apply` method, and the results are stored in a new column called `sentiment`.

4. **Output**: The script prints the review text and the corresponding sentiment classification.

## Customization

You can customize the script in the following ways:

- **Dataset**: Replace the `restaurant_reviews.csv` file with your own dataset of restaurant reviews.
- **Keyword Lists**: Modify the `positive_keywords` and `negative_keywords` lists to include or exclude specific words that you want to use for sentiment classification.
- **Classification Logic**: Adjust the `classify_sentiment` function to use more advanced sentiment analysis techniques, such as sentiment analysis libraries or machine learning models, to improve the accuracy of the sentiment classification.

## Contributions

Contributions to this project are welcome. Please submit pull requests or issues to improve the sentiment analysis model or add new features.
