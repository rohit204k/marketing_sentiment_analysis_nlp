# Market Sentiment Analysis of Amazon Reviews - Video Games Category

## Overview

This project aims to analyze the sentiment of Amazon reviews in the video games product category. By focusing on reviews with extreme ratings (1 and 5 stars), we aim to gain insights into customer satisfaction and dissatisfaction. The sentiment analysis is performed using the TextBlob library, which calculates polarity scores for the review text and summary. 

## Project Structure

The project is organized into two main Jupyter notebooks:

1. **data_preparation.ipynb**: This notebook is responsible for downloading the data, filtering the reviews, and preparing the dataset.
2. **Sentiment_Analysis_Using_Textblob.ipynb**: This notebook performs sentiment analysis on the prepared dataset and evaluates the performance of the sentiment prediction.

## Data Preparation

### data_preparation.ipynb

This notebook performs the following tasks:
1. **Data Download**: Downloads the dataset containing Amazon reviews for video games.
2. **Filtering Reviews**: Selects reviews with overall ratings of 1 and 5 to focus on extreme sentiments.
3. **Data Cleaning**: Removes irrelevant columns to streamline the dataset.
4. **CSV Generation**: Outputs the cleaned and filtered data to a .csv file for further analysis.

## Sentiment Analysis

### Sentiment_Analysis_Using_Textblob.ipynb

This notebook performs the sentiment analysis using the following steps:
1. **Data Import**: Loads the .csv file generated in the data preparation step.
2. **Sentiment Scoring**: Uses TextBlob to calculate the polarity scores for the `reviewText` and `summary` columns.
3. **Sentiment Prediction**: Predicts sentiment scores based on the calculated polarity.
4. **Evaluation**: Assesses the performance of the sentiment prediction using standard metrics.

### Evaluation Metrics

- **Accuracy**: 0.7894
- **Precision**: 0.7950
- **Recall**: 0.7894
- **F1 Score**: 0.7885

## Requirements

To run this project, you'll need the following Python libraries:
- pandas
- numpy
- TextBlob
- seaborn
- ndjson
- nltk
- sklearn (for evaluation metrics)

You can install the necessary libraries using the following bash command:

```bash
pip install pandas numpy textblob scikit-learn nltk ndjson seaborn
```

## Usage
1. Data Preparation: Run the data_preparation.ipynb notebook to download and clean the data. This will generate a filtered_reviews.csv file.
2. Sentiment Analysis: Run the Sentiment_Analysis_Using_Textblob.ipynb notebook to perform the sentiment analysis and evaluate the results.

## Results
The sentiment analysis achieved the following performance metrics:

* Accuracy: 0.7894
* Precision: 0.7950
* Recall: 0.7894
* F1 Score: 0.7885

These results indicate a reasonably accurate model for predicting the sentiment of Amazon reviews in the video games category.

## Conclusion
This project provides a comprehensive approach to analyzing customer sentiment in Amazon reviews for video games. By focusing on extreme reviews and leveraging TextBlob for sentiment scoring, we can gain valuable insights into customer satisfaction and dissatisfaction.

For any questions or further information, please feel free to contact the project maintainers.