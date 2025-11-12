# NLP: BBC News Article Classification
This project is an end-to-end data science capstone focused on Natural Language Processing (NLP). I built and compared three different machine learning models to accurately classify news articles into their correct categories (e.g., 'Business', 'Tech', 'Sport').

**Final Result:** The **Naive Bayes** model was the most successful, achieving **98.2% accuracy** on the test data.

---

## Business Problem
The goal of this project is to build an automated system that can read and correctly categorize large volumes of unstructured text data. This has direct real-world applications for:
* News organizations (automating content tagging)
* Content aggregators (sorting articles for users)
* Spam filters (classifying text)

## Technical Workflow

This project followed a complete data science workflow, from data cleaning to model evaluation.

### 1. Data Sourcing & Cleaning
* **Dataset:** Used the classic "BBC News" dataset, which contains 2,225 articles across 5 categories.
* **Text Cleaning (NLP):** Before modeling, the text was heavily pre-processed using:
    * **Tokenization:** Splitting sentences into individual words.
    * **Stop Word Removal:** Removing common, non-informative words (e.g., 'the', 'is', 'a').
    * **Lemmatization:** Standardizing words to their root (e.g., "running" and "ran" both become "run").

### 2. Feature Engineering (TF-IDF)
To convert text into numbers that a model can understand, I used an industry-standard technique:
* **TF-IDF Vectorization:** This method (Term Frequency-Inverse Document Frequency) analyzes the text and gives a higher "importance" score to words that are rare and unique to a specific category, rather than words that appear everywhere.

### 3. Model Building & Competition
I trained and evaluated three different classification models to find the best one for the job.

* **Model 1: Logistic Regression**
* **Model 2: K-Nearest Neighbors (KNN)**
* **Model 3: Naive Bayes**

All models were scientifically compared based on their accuracy, precision, and recall on an unseen test dataset.

## Results
The Naive Bayes model was the clear winner, demonstrating exceptionally high performance in classifying news articles.

| Model | Accuracy |
| :--- | :--- |
| **Naive Bayes** | **98.2%** |
| Logistic Regression | 97.3% |
| K-Nearest Neighbors | 95.1% |

This project demonstrates the ability to handle unstructured text data and build a high-accuracy classification pipeline from the ground up.

## Tools Used
* **Python**
* **Pandas & NumPy:** For data manipulation.
* **Scikit-learn (sklearn):** For `TF-IDF`, modeling (`LogisticRegression`, `KNN`, `NaiveBayes`), and evaluation.
* **NLTK:** For all Natural Language Processing (NLP) and text-cleaning tasks.
