# Text Data Preprocessor for NLP using Python

This project demonstrates a step-by-step guide to preprocessing text data for Natural Language Processing (NLP) tasks using Python and the pandas library. The dataset used for this project is the **disaster_tweet.csv**, which contains tweets labeled as either disaster-related or not.

The dataset consists of 5 columns:

- **id**: Unique identifier for each tweet.
- **keyword**: A keyword from the tweet (may be missing).
- **location**: Location of the tweet's author (may be missing).
- **text**: The full text of the tweet.
- **target**: Label indicating whether the tweet is disaster-related (1) or not (0).

## Preprocessing Steps

1. **Handling Missing Values**:
   - Missing values in the `keyword` and `location` columns were handled in two ways:
     - Rows with missing values were dropped.
     - Alternatively, missing values were filled with an empty string.

2. **Removing Duplicates**:
   - The dataset was checked for duplicate entries and any duplicates were removed to ensure data consistency.

3. **Text Preprocessing**:
   - **Lowercase Conversion**: All text was converted to lowercase to standardize the format.
   - **Punctuation and Number Removal**: Punctuation and numbers were removed to focus only on meaningful words.
   - **Whitespace Handling**: Extra spaces between words were removed.
   - **Stopword Removal**: Common stopwords such as "the", "is", "in", etc., were removed to reduce noise and improve the quality of the dataset.

4. **Final Cleaned Data**:
   - The cleaned text data was saved to `disaster_tweet_cleaned.csv` for further analysis and modeling.
