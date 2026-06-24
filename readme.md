# Text Similarity Analysis Using CountVectorizer

## Project Overview

This project demonstrates how to convert text data into numerical vectors using **CountVectorizer** from Scikit-Learn and calculate the similarity between sentences using the **Dot Product** technique.

The project uses three example sentences containing the word **"light"** and compares their similarity based on word occurrence frequencies.

---

## Objectives

* Understand the Bag-of-Words (BoW) model.
* Convert textual data into numerical vectors.
* Generate a vocabulary from text.
* Create a document-term matrix.
* Calculate sentence similarity using the dot product.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-Learn

---

## Dataset

The program loads the first **50,000 rows** from the Amazon Fine Food Reviews dataset:

`Reviews.csv`

Although the dataset is loaded, the similarity calculation is performed on three manually defined sample sentences.

---

## Sample Sentences

1. This olive oil is wonderful and very light on the stomach.
2. The packaging was broken and let too much light inside the box.
3. I prefer this brand because it is a light and healthy snack.

---

## Project Workflow

### Step 1: Import Libraries

Import required Python libraries:

* Pandas
* NumPy
* CountVectorizer

### Step 2: Load Dataset

Load the first 50,000 records from the dataset using Pandas.

### Step 3: Text Vectorization

Use CountVectorizer to:

* Tokenize text
* Build vocabulary
* Create a document-term matrix

### Step 4: Generate Dense Matrix

Convert sparse matrix into a dense matrix for easy visualization.

### Step 5: Extract Sentence Vectors

Store each sentence vector separately.

### Step 6: Calculate Similarity

Compute dot product similarity scores between:

* Sentence 1 and Sentence 2
* Sentence 1 and Sentence 3

---

## Output

### Vocabulary

```text
['and' 'because' 'box' 'brand' 'broken' 'healthy' 'inside' 'is' 'it'
 'let' 'light' 'much' 'oil' 'olive' 'on' 'packaging' 'prefer' 'snack'
 'stomach' 'the' 'this' 'too' 'very' 'was' 'wonderful']
```

### Similarity Scores

```text
Sentence 1 vs Sentence 2: 4
Sentence 1 vs Sentence 3: 4
```

---

## Interpretation

A higher dot product value indicates that two sentences share more common words.

In this project:

* Sentence 1 and Sentence 2 have a similarity score of 4.
* Sentence 1 and Sentence 3 also have a similarity score of 4.

This means both sentence pairs share a similar number of common terms according to the Bag-of-Words representation.

---

## Key Concepts

### Bag of Words (BoW)

A text representation technique that counts the frequency of words in a document.

### CountVectorizer

A Scikit-Learn tool that converts text into numerical feature vectors.

### Document-Term Matrix

A matrix showing the frequency of each word in each document.

### Dot Product Similarity

A mathematical operation used to measure similarity between two vectors.

---

## Future Improvements

* Implement Cosine Similarity for better similarity measurement.
* Perform sentiment analysis on review data.
* Visualize similarity scores using graphs.
* Process the complete review dataset instead of sample sentences.
* Compare multiple NLP vectorization techniques such as TF-IDF and Word Embeddings.

---

