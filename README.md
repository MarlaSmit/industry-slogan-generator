# Industry Slogan Generator & Classifier

An NLP project using LSTM neural networks to generate industry-specific marketing slogans and classify slogans by industry.

## Overview

This project explores two natural language processing tasks using TensorFlow and Long Short-Term Memory (LSTM) networks:

1. **Slogan Generation** – Generate new marketing slogans based on an industry prompt.
2. **Industry Classification** – Predict the industry associated with a given slogan.

The project demonstrates an end-to-end NLP workflow, including text preprocessing, tokenization, sequence padding, neural network modelling, text generation, and multi-class classification.

## Project Workflow

### 1. Data Preprocessing
- Cleaned and processed the slogan data.
- Removed unnecessary text and standardised the slogans.
- Prepared the industry labels for classification.

### 2. Slogan Generation

An LSTM-based language model was trained to predict the next word in a sequence.

The model uses:
- Word tokenization
- Sequence generation
- Padding
- An embedding layer
- Stacked LSTM layers
- A softmax output layer

The trained model can generate new slogans from an industry prompt.

### 3. Industry Classification

A second LSTM model was developed to predict the industry associated with a slogan.

The classifier:
- Tokenizes the slogan text.
- Converts words into numerical sequences.
- Pads the sequences to a consistent length.
- Uses an embedding layer and stacked LSTM layers.
- Predicts one of the industry categories in the dataset.

## Results

The industry classifier achieved approximately **20% test accuracy across 142 industry categories**.

While this performance is substantially above random guessing, classification remains challenging due to the large number of classes and similarities in vocabulary between different industries.

The slogan generator was able to produce industry-related language, although some generated sequences became less coherent as their length increased.

These results highlight both the potential and limitations of LSTM-based NLP models when working with a relatively small and diverse dataset.

## Technologies Used

- Python
- TensorFlow / Keras
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## Key Skills Demonstrated

- Natural Language Processing (NLP)
- Text preprocessing
- Tokenization
- Sequence modelling
- LSTM neural networks
- Text generation
- Multi-class classification
- Model evaluation
- Data preprocessing
- Python programming

## Future Improvements

Potential improvements to the project include:

- Training on a larger and more diverse dataset.
- Using pretrained word embeddings such as Word2Vec or GloVe.
- Experimenting with transformer-based models.
- Hyperparameter tuning.
- Improving the coherence of generated slogans.
- Addressing class imbalance and similarities between industry categories.
