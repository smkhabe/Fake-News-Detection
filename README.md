# Fake-News-Detection

![image](https://github.com/smkhabe/Fake-News-Detection/assets/110238344/9d1c41d1-330a-438d-8e81-7a2c910a0d55)

- You can find the CSV Files into Fake_csv.zip and True_csv,zip files

  
**The data is preprocessed using the following steps:**

Tokenization: The text is split into individual words using the word_tokenize function from the nltk.tokenize module.

Stopword Removal: The stopwords.words('english') list from the nltk.corpus module is used to remove common words like 'is', 'the', 'and', etc.

Stemming: The PorterStemmer class from the nltk.stem module is used to reduce words to their root form.
Vectorization: The CountVectorizer class from the sklearn.feature_extraction.text module is used to convert the text into a matrix of token counts.

Model Training: Four different models are used to classify the news as either fake or not fake:

Logistic Regression: The LogisticRegression class from the sklearn.linear_model module is used.

Decision Tree Classifier: The DecisionTreeClassifier class from the sklearn.tree module is used.

Gradient Boosting Classifier: The GradientBoostingClassifier class from the sklearn.ensemble module is used.

Random Forest Classifier: The RandomForestClassifier class from the sklearn.ensemble module is used.

Model Evaluation: The accuracy of each model is evaluated using the score method. The classification_report function from the sklearn.metrics module is used to generate a detailed report of the precision, recall, and F1-score of each model.

Manual Testing: The manual_testing function takes a news article as input and predicts its label using all four models. The output_lable function is used to convert the numeric labels into human-readable strings.
