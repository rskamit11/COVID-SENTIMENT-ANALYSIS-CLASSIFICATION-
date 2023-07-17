# COVID-SENTIMENT-ANALYSIS-CLASSIFICATION-

SUMMARY
The present prediction analysis is based on the tweets done between the months of March and April, 2020 which is the first wave of COVID-19 pandemic disease. Coronavirus disease (COVID-19) is an infectious disease caused by the SARS-CoV-2 virus. Henceforth, due to panic situation people started tweeting on Twitter (it is social media platform) following with different sentiments associated with that. The present provided dataset consist of (41157, 6) numbers of rows and columns. But our present prediction analysis performed using two columns only of original tweets and sentiments. 5 types of sentiments were provided namely: Extremely Positive, Positive, Neutral, Negative and Extremely Negative.
Dataset Information
Username: Unique user-IDs of the users
Location: Location of the user
Tweet At: Date at which the tweet was made
Original Tweet: The exact tweet
Sentiment: Sentiment of the tweet

EDA
The original dataset has 6 columns and 41157 rows.
Null values in Location column
There are 20.87%(8567) null values in various places of location column.
There are five types of sentiments- Extremely Negative, Negative, Neutral, Positive and Extremely Positive.
All tweets data collected from the months of March and April 2020. Bar plot shows us the number of tweets as per days of the month.
Most of the tweets came from London followed by U.S.

DATA PREPROCESSING
The preprocessing of the text data is an essential step as it makes the raw text ready for mining.
The objective of this step is to clean noise those are less relevant to find the sentiment of tweets such as punctuation, special characters, numbers, and terms which don’t carry much weightage in context to the text.
Stop words are those words in natural language that have a very little meaning, such as "is", "an", "the", etc.To remove stop words from a sentence, you can divide your text into words and then remove the word if it exits in the list of stop words provided by NLTK.
The tweets contain lots of twitter handles (@user). We will remove all these twitter handles from the data as they don’t convey much information.
We are having twitter links in the data which are not useful for our Model. It will make our data noisy.
Punctuations, numbers and special characters do not help much. It is better to remove them from the text just as we removed the twitter handles,links and hashtags.
Stemming is a rule-based process of stripping the suffixes (“ing”, “ly”, “es”, “ed”, “s” etc) from a word. For example – “play”, “player”, “played”, “plays” and “playing” are the different variations of the word – “play”.
Lemmatization is a more powerful operation, and it takes into consideration morphological analysis of the words. It returns the lemma which is the base form of all its inflectional forms.
In tokenization we convert group of sentence into token . It is also called text segmentation or lexical analysis. It is basically splitting data into small chunk of words. Tokenization in python can be done by python NLTK library’s word_tokenize() function.

CONCLUSION
 We applied 3 different machine learing models namely, Logistic Regression with Grid Search CV, Desision Tree Classifier,SVM Classifier for both Count Vector And TF IDF Vectorisation techniques.We conclude that the machine is generating best results for Logistic Regression with Grid Search CV model with and Accuracy score of 78% and 77% respectively for Count vector and TF/idf Vector, followed by SVM. Also, we observed that no overfitting is seen for the data, and we can deploy this model.The sentiments of future tweets can be easily predicted using this model.
