A deep learning-based sentiment analysis project that uses a Simple Recurrent Neural Network (RNN) to classify IMDB movie reviews as Positive or Negative.


## Project Overview

This project uses the IMDB movie review dataset provided by TensorFlow/Keras. The reviews are converted into integer sequences using the IMDB word index, padded to a fixed length, and passed through an RNN model for binary sentiment classification.

The trained model is deployed as an interactive Streamlit web application, allowing users to enter their own movie review and receive a sentiment prediction with a confidence score.

## Model Architecture

The model consists of:

Embedding Layer — Converts word indices into dense vector representations.
SimpleRNN Layer — Learns sequential patterns in the review text.
Dense Layer with Sigmoid Activation — Produces the final binary classification probability.


## Architecture
Input Review
     ↓
IMDB Word Index
     ↓
Sequence of Integers
     ↓
Padding (500 tokens)
     ↓
Embedding (128 dimensions)
     ↓
SimpleRNN (128 units)
     ↓
Dense (1, Sigmoid)
     ↓
Positive / Negative
Dataset

## The project uses the IMDB Movie Reviews Dataset available through TensorFlow/Keras.

25,000 training reviews
25,000 testing reviews
Binary labels:
0 → Negative
1 → Positive
Vocabulary size: 10,000
Maximum sequence length: 500
Model Performance

## The trained model achieved approximately:

Training Accuracy	84.72%
Validation Accuracy	77.38%
Training Loss	0.3544
Validation Loss	0.5877


## Technologies Used
Python
TensorFlow
Keras
NumPy
Streamlit
Jupyter Notebook
Simple RNN
Natural Language Processing (NLP)
