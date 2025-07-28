
This project, "FAKE_NEWS_PREDICTION.ipynb", focuses on building a machine learning model to classify news articles as real or fake.

Here's a summary of the project:

The project utilizes a dataset containing news article information, including id, title, author, text, and a label (0 for real news, 1 for fake news).

Data Preprocessing:

The dataset is loaded into a Pandas DataFrame.

Missing values in the news_url and source_domain columns are identified and replaced with empty strings.

A new 'content' column is created by merging the 'news_url' and 'title' columns.

Textual data in the 'content' column undergoes a stemming process using the Porter Stemmer from NLTK. This involves removing non-alphabetic characters, converting text to lowercase, tokenizing, and removing English stopwords.

The processed textual content (X) and the 'real' labels (Y) are separated for model training.

TF-IDF Vectorization is applied to transform the textual data into numerical feature vectors.

Model Training and Evaluation:

The dataset is split into training and testing sets with a 80/20 ratio, ensuring stratified sampling for consistent class distribution.

A Logistic Regression model is initialized and trained on the preprocessed training data.

The model's performance is evaluated using accuracy scores.

It achieves an accuracy of approximately 94.8% on the training data.

It achieves an accuracy of approximately 92.7% on the test data.

Predictive System:

The trained model can be used to predict whether a new news article is real or fake based on its content.
