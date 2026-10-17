# Lab 02 – Basic NLP Preprocessing Techniques

**Course:** ITAI 2373 – Natural Language Processing  
**Student:** Oman Malek  
**Platform:** Google Colab

## Overview

This lab explores how raw text is prepared for Natural Language Processing. I compared NLTK and spaCy and investigated how preprocessing choices affect the information preserved in text.

## Topics Covered

- Word and sentence tokenization
- Stop-word removal
- Stemming versus lemmatization
- Cleaning punctuation and special characters
- Processing social media text, emojis, hashtags, and contractions
- Building a configurable preprocessing pipeline

## Key Observations

- In one example, NLTK stop-word removal reduced the token count by **28.6%**, while spaCy's stop-word and punctuation removal reduced it by **50%**.
- Removing words such as *not*, *no*, and *never* can change sentiment.
- Stemming is often faster but can produce unnatural word forms; lemmatization preserves meaningful base forms.
- Social media symbols and punctuation may carry useful information and should not always be discarded.

## Included Files

- `Lab_02_Text_Preprocessing_Notebook_Export.pdf` — executed notebook PDF export.
- `Lab_02_Reflection_Journal.pdf` — personal learning reflection, challenges, and future exploration.

## How to Use

Read the notebook export to review the code, activities, and outputs. For executable code, open the original `.ipynb` notebook in Google Colab if available.

## What I Learned

Good preprocessing does not mean deleting as much text as possible. The right cleaning strategy depends on the application, such as sentiment analysis, chatbots, or text classification.

## Applications

Sentiment analysis, chatbots, search, text classification, and social media analytics.
