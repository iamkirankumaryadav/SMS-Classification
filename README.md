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

### 1. **Import** Data ( SMS )

### 2. **Exploratory Data Analysis**

### 3. **Clean** Text 

- Remove Punctuation.
- Change to Lowercase.
- Tokenization : **Splitting** a Phrase | Sentence into List of **Individual Words** called **Tokens**.
- Remove Stopwords : Most Common Words ( Filtered out before processing Natural Language Data )
- Stemming ( Speed ) | Lemmatization ( Accuracy ) : Reduce the Word to its Base | Stem Form.

### 4. **Feature Engineering**

- Vectorization : Allocate Text to Numbers or Vectors that an Algorithm and a Machine Learning Model can Understand and Learn.
- CountVectorizer : Extract Features from Text ( Count Occurence of Text in Corpus and Consider each as Feature | Column )
- Bag of Words : Count Occurence of the Word in each Document and each Word becomes Feature Represented by a Vector. 
- TF-IDF : Represents **Importance** of the Word in the Document. 
- Term Frequency : Number of Time the Term Appears in the Document. 
- Inverse Document Frequency : Number of Documents containing the Word.
- Word2Vec : Learn Word Association from a Large Corpus of Text, Once Trained can Detect Synonyms and can Suggest Words.

Word2Vec Matrix | TF-IDF Matrix
:--- | :--- 
Multi Dimensional Vector | Sparse Matrix
Capture Words Relationship with other Words | Captures the Importance of Word in a given Documment
Applied on each Word Individully | Applied to each Training Document
More Memory Intensive | Less Memory Intensive
Ideal for Single Word Problems | Ideal for Problems with Multiple Words or Document Files.

### BERT 
- Google's Pre trained **Bidirectional Encoder Representation for Transformers** used for **Transfer Learning**.

### 5. **Fit** | **Train** Simple Model

### 6. **Tune Hyperparameters** and **Evaluate** with **Grid Search Cross Validation**

### 7. Final **Model Selection** ( Comparing Models and Selecting Best One )

### Process
1. **Split** the Data into **Training** Set and **Test** Set.
2. Train **Vectorizers** on Training Set and Use that to Transform **Test** Set.
3. Fit Best **Random Forest Model** and Best **Gradient Boosting Model** on **Training Set** and **Predict** on **Test Set**.
4. **Evaluate** Results of these Two Models to Select **Best Model**.

