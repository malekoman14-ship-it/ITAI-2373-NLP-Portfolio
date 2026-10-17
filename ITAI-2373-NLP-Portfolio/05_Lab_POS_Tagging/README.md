# Lab 05 – Part-of-Speech (POS) Tagging

**Course:** ITAI 2373 – Natural Language Processing  
**Student:** Oman Malek  
**Platform:** Google Colab  
**Language:** Python

## Overview

This lab focuses on **Part-of-Speech (POS) tagging**, which identifies the grammatical role of each word in a sentence, such as noun, verb, adjective, or adverb. I compared NLTK and spaCy and tested tagging on simple sentences, ambiguous words, informal language, and customer service text.

## Learning Objectives

- Understand common POS tags and their meanings.
- Perform POS tagging using NLTK and spaCy.
- Compare detailed Penn Treebank tags with simpler Universal tags.
- Explore how word context affects grammatical interpretation.
- Analyze messy text and customer service transcripts.
- Benchmark tagging methods and investigate tagging errors.

## Tools and Libraries

Python, Google Colab, NLTK, spaCy (`en_core_web_sm`), pandas, Matplotlib, and Seaborn.

## Lab Activities

### Part 1 – In-Class Exercises

**Activity 1: First POS Tags**  
I used NLTK to tag a sample sentence and identify determiners, adjectives, nouns, verbs, and prepositions.

**Activity 2: NLTK vs. spaCy**  
I compared both libraries on the same sentence. NLTK produced detailed tags such as `DT`, `JJ`, and `VBZ`, while spaCy also provided readable categories such as `DET`, `ADJ`, and `VERB`.

**Activity 3: Word Ambiguity**  
I examined words such as *lead* and *bank* in different contexts to see how grammatical roles depend on the surrounding sentence.

**Activity 4: Tag Set Comparison**  
I compared Penn Treebank and Universal tags to understand the trade-off between detailed grammatical information and simpler categories.

### Part 2 – Homework Lab

**Exercise 1: Messy Text Challenge**  
I examined informal language, speech-like text, slang, abbreviations, and social media expressions to understand why real-world tagging can be difficult.

**Exercise 2: Customer Service Analysis**  
I applied POS tagging to customer service scenarios and explored patterns in the language, including visualizations.

**Exercise 3: Tagger Performance Benchmarking**  
I compared tagging approaches and considered speed, reliability, and the limitations of interpreting automated tags.

**Exercise 4: Edge Cases and Error Analysis**  
I explored difficult inputs and examined how POS taggers can make mistakes when language is ambiguous or unusual.

## Results and Observations

- On the sample sentence, NLTK and spaCy generally identified similar grammatical roles but used different tag formats.
- The recorded NLTK output tagged **“brown”** as a noun (`NN`), while spaCy tagged it as an adjective (`ADJ`).
- In the ambiguity exercise, NLTK tagged **“I bank with Chase”** as `NN` for *bank*, illustrating a possible tagging error.
- For the sample tag-set comparison, the notebook reported **8 distinct Penn Treebank tags** and **6 distinct Universal tags**.
- Informal text, ambiguous words, and context-dependent expressions showed why POS tagging is not always perfect.

## How to Run

1. Open the Lab 05 `.ipynb` notebook in Google Colab.
2. Install the required packages:
   ```bash
   pip install nltk spacy matplotlib seaborn pandas
   python -m spacy download en_core_web_sm
   ```
3. Run the setup cells to download the NLTK resources and load the spaCy model.
4. Execute the exercises in order and review the tagging outputs, charts, and written answers.

## What I Learned

I learned how computers identify grammatical roles and why sentence context matters. Comparing NLTK and spaCy showed me that tag sets differ in detail and readability, while the real-world exercises showed that slang, ambiguity, and incomplete speech can reduce tagging reliability.

## Real-World Applications

Customer support analytics, search engines, voice assistants, grammar checking, information extraction, and chatbot language understanding.

## Conclusion

Lab 05 gave me hands-on experience with POS tagging and helped me understand both the strengths and limitations of automated grammatical analysis in real-world NLP systems.
