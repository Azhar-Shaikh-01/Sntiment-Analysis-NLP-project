# Sntiment-Analysis-NLP-project


# Dataset Overview:
The dataset contains an extensive collection of tweets, consisting of text, language labels, and sentiment labels. There are a total of 937,854 entries in the dataset, each accompanied by its respective language and sentiment labels. The dataset exhibits diversity in terms of the languages used, with 929,544 unique texts found among the entries. Additionally, the dataset includes a wide range of language and sentiment labels, providing a comprehensive representation of public sentiment across various languages.

Text:
The "Text" column refers to the actual content of each tweet. With almost a million unique texts, the dataset captures a rich variety of statements and opinions expressed on social media platforms.

Language:
The "Language" column indicates the language in which each tweet is composed. There are 72 different language labels found in the dataset. This diversity highlights the multilingual nature of the tweets and the challenge of identifying languages accurately.

Label:
The "Label" column represents the sentiment label associated with each tweet. Sentiment labels are categorized into four classes: positive, negative, uncertainty, or litigious. This categorization allows us to understand the emotional tone and sentiment conveyed by the tweets.

Dataset Link: https://www.kaggle.com/datasets/tariqsays/sentiment-dataset-with-1-million-tweets

# Problem Statement:
This project revolves around two fundamental tasks: language identification and sentiment classification. For language identification, the goal is to predict the language of each tweet from the 72 available language labels. For sentiment classification, the objective is to classify the sentiment of each tweet into one of the four predefined sentiment categories: positive, negative, uncertainty, or litigious.
# Conclusions
## Pipeline for Language Identification:
LinearSVC is renowned for its efficiency in handling high-dimensional data and is particularly effective for multiclass classification tasks like language identification. Its ability to draw clear boundaries between classes in a high-dimensional space aligns well with the diverse language labels.A pipeline for language identification is established, incorporating the TF-IDF vectorizer and the LinearSVC classifier. This pipeline is trained on the tweets and their corresponding language labels. With a remarkable accuracy of 98%, the pipeline excels in accurately identifying the language of a given tweet.

## Pipeline for Sentiment Classification:
Multinomial Naive Bayes is widely used for text classification tasks due to its simplicity and effectiveness in handling text data. It performs well in scenarios where features are discrete (word frequencies in this case) and often yields competitive results. Another pipeline, built for sentiment classification, integrates the TF-IDF vectorizer and the Multinomial Naive Bayes classifier. This pipeline is trained on the tweets and their associated sentiment labels. Achieving an accuracy of 82%, the pipeline proficiently classifies the sentiment expressed in each tweet.
