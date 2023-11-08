# Text Classification with Pretrained GloVe Embeddings and LSTM

## Context

This project focuses on using pre-trained GloVe (Global Vectors for Word Representation) embeddings along with an LSTM (Long Short-Term Memory) network to perform text classification. The combination of these resources can significantly improve accuracy in text classification tasks, such as sentiment analysis or news classification, by effectively capturing the context and semantics of words in textual data.

## LSTM in text classification
The LSTM (Long Short-Term Memory) Network is a recurrent neural network architecture commonly used in natural language processing tasks, including text classification. Its key components include:

1. **Long-term memory**: LSTMs use state memory to retain temporal relationships and connections in the input data.
2. **Interconnected cells**: LSTMs consist of cells that can read, write, and erase information in their internal memory.
3. **Control gates**: Entry, forget, and exit gates regulate information flow within cells, determining what's stored or discarded.
4. **Sequence modeling**: LSTMs excel at handling sequential data, making them ideal for text classification tasks.
5. **Improved text classification**: LSTMs enhance context understanding and performance in text classification.

This project leverages PyTorch's LSTM implementation.

## About GloVe

GloVe (Global Vectors for Word Representation) is a word representation technique that maps words to a vector space where semantic relationships are reflected in the distance between word vectors. This technique is widely used in natural language processing for tasks such as text classification and text generation.

For more information about GloVe, visit the [GloVe GitHub](https://github.com/stanfordnlp/GloVe).

## Data information

#### Data Loading

The project uses the **AG's News Topic Classification Dataset** from Pytorch, which consists of news articles from various sources categorized into four topics: 
* World
* Sports
* Business
* Science/Technology. 

This dataset is of moderate size and serves the purpose of text classification, where the goal is to assign each news article to one of these predefined categories. 

## Objectives

The main objective of this project is to classify texts into four different categories using natural language processing and machine learning techniques. The project focuses on data preparation, implementing a text classification model, and evaluating the model's performance.

## Usage

To use this project, follow these steps:

1. Ensure that you have the following libraries installed: GloVe, PyTorch, and other dependencies mentioned in the code.

2. Run the provided code to prepare the data, create the model, and train the model on your data.

3. Use the evaluation functions to measure the model's performance on a test dataset.

## Required Libraries

Make sure to have the following libraries installed to run this project:
- GloVe
- PyTorch
- Scikit-learn
