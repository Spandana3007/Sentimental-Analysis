**Introduction:** This repository contains the code and documentation for performing sentiment analysis on Twitter tweets related to Kent State University. The sentiment analysis aims to classify tweets into positive, negative, or neutral attitudes, providing insights into the opinions and viewpoints surrounding the university.

**Web Scraping:**
The Twitter API was utilized for scraping tweets regarding Kent State University. The Tweepy library was employed for this purpose, and all necessary keys and tokens were generated from the Twitter Developer Account. Duplicate tweets were removed using a set structure (unique_tweets). The collected information includes tweet content, user details, associated hashtags, and timestamps.

**Data Processing Steps**
**Preprocessing:**
Raw tweet data was preprocessed to remove URLs, punctuation, and stop words. The nltk library was used for this task, along with WordNetLemmatizer for lemmatization.
The preprocessed text data was then further processed into numerical forms using CountVectorizer and TfidfVectorizer from the scikit-learn library.

**Sentiment Labeling:**
VADER sentiment analyzer was employed for sentiment labeling. The SentimentIntensityAnalyzer was utilized to assign sentiment labels (positive, negative, or neutral) based on polarity scores.

**Model Architecture:**
The sentiment analysis model was built and trained using machine learning techniques and libraries. The architecture includes layers such as Embedding, Conv1D, MaxPooling1D, LSTM, and Dense. The dataset was split into training and testing sets using train_test_split from sklearn.model_selection. The model was trained using model.fit() over multiple epochs.

**Results and Evaluation Metrics:**
The model's performance was evaluated using various metrics including accuracy, precision, recall, and F1-score. Visualization techniques such as heatmaps and confusion matrices were employed for result analysis. Classification report provided detailed metrics for each sentiment class.

**Limitations:**
The sentiment analysis model is subject to certain limitations:

+ Dependency on the quality of training data.
+ Difficulty in comprehending context and characteristics associated with Kent State University.
+ Challenges in analyzing humor or complex language.
+ Domain-specific issues when analyzing tweets related to Kent State University.

**Conclusion:**
In conclusion, while the sentiment analysis model provides valuable insights into the opinions surrounding Kent State University, it is essential to acknowledge its limitations. Further refinement and adjustment of the analysis data may enhance accuracy and reliability. Understanding the model's strengths and weaknesses is crucial for interpreting results effectively.
