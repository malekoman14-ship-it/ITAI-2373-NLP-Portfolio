# Lab 04 – Text Representation: From Words to Numbers

**Course:** ITAI 2373 – Natural Language Processing  
**Student:** Oman Aiyubkhan Malek  
**Platform:** Google Colab  
**Language:** Python

## Overview

In this lab, I explored how Natural Language Processing (NLP) converts written text into numerical features that machine learning models can understand. I worked with Bag of Words (BOW), TF-IDF, N-grams, and word embeddings, then compared text representations in a classification task.

## Learning Objectives

- Clean and preprocess text using tokenization, stop word removal, and stemming.
- Implement Bag of Words and understand sparse word-count vectors.
- Calculate and use TF-IDF to identify important words.
- Explore N-grams to capture neighboring word sequences.
- Understand dense word embeddings and semantic similarity.
- Compare text representations in a simple machine learning application.

## Tools and Libraries

Python, Google Colab, NLTK, NumPy, pandas, scikit-learn, Gensim, Matplotlib, Seaborn, and WordCloud.

## Lab Activities

### 1. Text Preprocessing and Bag of Words
I cleaned sample movie reviews, created a reusable preprocessing function, built BOW vectors from scratch, and compared them with scikit-learn's `CountVectorizer`.

### 2. TF-IDF and N-grams
I explored how TF-IDF assigns greater importance to distinctive terms and how N-grams represent sequences of words rather than isolated words.

### 3. Word Embeddings
I examined dense representations and how embeddings can capture semantic relationships between words.

### 4. Classification and Practical Applications
I compared BOW, TF-IDF, and unigram-plus-bigram representations in a text classification experiment. I also explored text similarity and a simple TF-IDF-based search application.

## Results and Observations

- My BOW implementation generated a **5-document × 27-word** matrix for the sample movie reviews.
- In the notebook's small, balanced teaching classification dataset, **BOW, TF-IDF, and N-grams each achieved 1.000 accuracy** in the recorded run.
- These results are specific to the teaching dataset and do not guarantee equivalent performance on larger real-world datasets.
- BOW captures word frequency, TF-IDF highlights distinctive terms, N-grams preserve some local word order, and embeddings represent semantic relationships.

## How to Run

1. Open the Lab 04 `.ipynb` notebook in Google Colab.
2. Run the installation and import cells.
3. Execute the remaining cells in order.
4. Review the printed matrices, charts, classification reports, and reflection answers.

The notebook includes fallback behavior for some NLTK resources when downloads are unavailable.

## What I Learned

I learned that machine learning models need numerical representations of text and that each method captures different information. I also learned why preprocessing choices, dataset size, and evaluation conditions matter when comparing model performance.

## Real-World Applications

Document classification, sentiment analysis, search engines, spam detection, news categorization, and text similarity.

## Conclusion

Lab 04 helped me understand the full process of turning raw text into useful numerical features and applying those features to practical NLP tasks.
