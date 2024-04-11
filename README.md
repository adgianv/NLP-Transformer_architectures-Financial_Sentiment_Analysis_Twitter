# Financial News Sentiment Analysis on Twitter: Advanced augmentation techniques, Large Language models and Knowledge Distillation

## Overview
This repository contains code and documentation for sentiment analysis on Twitter financial news using various methodologies, including conventional techniques like TF-IDF and advanced deep learning models such as distilBERT and LLM Text Generated Model. 

The aim of this research is to predict sentiment in financial tweets, using a labelled dataset retrieved from Hugging face and simulating the situation of limited data availability (dataset of 32 labelled examples) to compute augmentation techniques such as Text Generation, Zero/Few Shot Learning, Word2Vec Similarities and other.

## Dataset
The Twitter Financial News dataset comprises English-language tweets labelled as 'Bearish' (LABEL_0), 'Bullish' (LABEL_1), or 'Neutral' (LABEL_2) for sentiment analysis. The training set contains 9,938 tweets, and the validation set has 2,486 tweets.

## Methodologies Explored
- **Preprocessing**: Employed the Ekphrasis package for social media text processing.
- **Random Classifier and Baseline Model**: Tested a random classifier and Spacy matcher for sentiment prediction.
- **BERT Models**: Utilized distilBERT for tweet embeddings and explored integrating an RNN layer.
- **Data Augmentation**: Implemented translation, backtranslation, Word2Vec similarity, synonym replacement, and random swap techniques.
- **LLM Text Generation**: Generated synthetic data using Large Language Models (LLMs) and Retrieval-Augmented Generation (RAG).
- **Combined Technique Model**: Integrated data augmentation and LLM text generation for improved sentiment prediction.

## Results
- With only 32 labelled examples:
  - **Data Augmentation**: Achieved 48.16% accuracy, 46.91% precision, and 50.35% recall.
  - **LLM Text Generated**: Achieved 50.92% accuracy, 44.28% precision, and 48.26% recall.
  - **Combined Technique**: Achieved 54.06% accuracy, 44.57% precision, and 48.07% recall.

- Entire dataset results:
  - **distilBERT model**: Achieved 86.85% accuracy, 83.73% precision, and 81.27% recall.

## Conclusion
The study highlights the effectiveness of data augmentation and LLM text generation techniques for improving sentiment analysis on Twitter financial news, especially with limited labelled data. Integrating diverse methodologies led to robust predictive outcomes, although challenges related to false predictions and class imbalance persisted. Future research could focus on further refining class rebalancing techniques and exploring more advanced preprocessing steps and model architectures.

For more details, refer to the complete report and code in this repository.

## Getting Started

To explore the project:
1. Clone the repository.
2. Review the Jupyter notebooks in the `Notebook-Twitter_Financial_News_Classification` notebook for detailed steps.

--- 

For further details and usage instructions, refer to the complete report and project documentation.


