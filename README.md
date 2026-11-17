# WordEmbedding
Word Embedding for Sentiment Analysis using the stanfordnlp/imdb dataset

## Overview

This project compares two word embedding algorithms for sentiment analysis and classification using the Stanford IMDb movie reviews dataset. The pipeline evaluates performance of TF-IDF Vectorizer and the pre-trained word representations Static Embeddings via GloVe, with both using a Logistic Regression classifier for training and evaluation.

## Project Files

| File | Description |
| ---- | ----------- |
| Name_Project1.ipynb | Jupyter notebook containing project code. |
| ReadMe.pdf Project | documentation PDF. |
| requirements.txt | List of dependencies used in the project. |

## Running the Program

1. **Install dependencies.** Open terminal in project directory and run the following to install required libraries:
```bash
pip install -r requirements.txt
```

2. **Execute the project.** The dataset is loaded in the cells. Run them sequentially or use `Run All` to train the model, view the performance metrics, and test it with user input.

## Dataset Description

The Stanford IMDb movie review dataset contains ~50,000 labelled movie reviews with binary positive/negative labels. The dataset is divided into 2 separate training and testing subsets each containing ~25,000 entries.

## Methodology

### Pre-Processing and Data Cleaning

On the Stanford dataset, several text normalization processes are performed including; converting to lowercase, removing HTML tags and punctuation, and removing whitespace.

### Model I: TF-IDF

Term Frequency-Inverse Document Frequency model assigns importance to more informative words within a document with respect to their frequency of appearance in the document.

### Model II: GloVe

GloVe or Global Vectors for Word Representation uses pre-trained dense word embeddings where each word is represented in vector space as a 50-dimensional vector.
