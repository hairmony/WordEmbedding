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

## References

* [Maas, A. L., Daly, R. E., Pham, P. T., Huang, D., Ng, A. Y., & Potts, C. (2011). Learning word vectors for sentiment analysis. Proceedings of the 49th Annual Meeting of the Association for Computational Linguistics: Human Language Technologies, 142–150.](https://aclanthology.org/P11-1015/)
* [Pennington, J., Socher, R., & Manning, C. D. (2014). GloVe: Global vectors for word representation. Proceedings of the 2014 Conference on Empirical Methods in Natural Language Processing (EMNLP), 1532–1543.](https://aclanthology.org/D14-1162/)
* [Pedregosa, F., Varoquaux, G., Gramfort, A., Michel, V., Thirion, B., Grisel, O., Blondel, M., Prettenhofer, P., Weiss, R., Dubourg, V., Vanderplas, J., Passos, A., Cournapeau, D., Brucher, M., Perrot, M., & Duchesnay, É. (2011). Scikit-learn: Machine learning in Python. Journal of Machine Learning Research, 12, 2825–2830.](https://www.jmlr.org/papers/volume12/pedregosa11a/pedregosa11a.pdf)
