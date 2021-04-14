# Spam SMS Classification 🔔 ⚠ ✔

### Libraries
1. NumPy
2. Pandas
3. Matplotlib ( Pyplot )
4. Scikit Learn ( Count Vectorizer, TF IDF Vectorizer, Random Forest Classifier, Gradient Boosting Classifier, K Fold Cross Validation, Grid Search Cross Validation, Train Test Split )
5. NLTK ( Corpus, Stopwords, Porter Stemmer, Word Net Lemmatizer )
6. String ( Punctuation )
7. RE : Regular Expression

### Features
1. SMS ( Messages Extracted in form of `TSV` )
2. Labels ( **Spam** or **Ham** )

### Machine Learning Pipeline
1. **Import** Data ( SMS )
2. **Exploratory Data Analysis**
3. **Clean** Text 
- Remove Punctuation
- Tokenization : **Splitting** a Phrase | Sentence into List of **Individual Words** called **Tokens**.
- Remove Stopwords : Most Common Words ( Filtered out before processing Natural Language Data )
- Stemming ( Speed ) | Lemmatization ( Accuracy ) : Reduce the Word to its Base | Stem Form.

4. **Feature Engineering**
- Vectorization : Converting Text to Numbers that an Algorithm and a Machine Learning Model can Understand and Learn.
- CountVectorizer : Extract Features from Text ( Count Occurence of Text in Corpus and Consider each as Feature | Column )

5. **Fit** | **Train** Simple Model
6. **Tune Hyperparameters** and **Evaluate** with **Grid Search Cross Validation**
7. Final **Model Selection** ( Comparing Models and Selecting Best One )

### Process
1. **Split** the Data into **Training** Set and **Test** Set.
2. Train **Vectorizers** on Training Set and Use that to Transform **Test** Set.
3. Fit Best **Random Forest Model** and Best **Gradient Boosting Model** on **Training Set** and **Predict** on **Test Set**.
4. **Evaluate** Results of these Two Models to Select **Best Model**.

