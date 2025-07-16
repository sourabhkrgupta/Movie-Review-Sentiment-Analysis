**Movie-Review-Sentiment-Analysis**

This project is a binary classification task to determine the sentiment of movie reviews (positive or negative).

Here's a summary of what has been done so far:

**Data Loading and Exploration**: The IMDB movie reviews dataset was loaded, and basic information and value counts were checked.
**Data Preprocessing**: The review text has been cleaned by:
1. Removing HTML tags
2. Removing special characters
3. Converting text to lowercase
4. Removing stopwords
5. Stemming the words
   
**Model Creation:**
The text data was transformed into numerical data using the Bag of Words (BOW) model with CountVectorizer.
The data was split into training and testing sets.
Three Naive Bayes models (Gaussian, Multinomial, and Bernoulli) were trained on the data.
The accuracy of each model was evaluated, and the Bernoulli Naive Bayes model was chosen as the best performing one.
The trained Bernoulli Naive Bayes model was saved using pickle.

Prediction on a New Review: The saved model was loaded, and a new review was preprocessed and used to predict its sentiment.

Gradio Interface: A Gradio web interface was created to allow users to input a movie review and get a sentiment prediction using the trained Bernoulli Naive Bayes model and the fitted CountVectorizer. The interface has been launched.
