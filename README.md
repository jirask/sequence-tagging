# Sequence Tagging Project

## Overview

This repository contains the code and documentation for a sequence tagging project. The goal of this project is to implement and compare different sequence tagging models on a real-world dataset. The models include a Convolutional Neural Network (CNN), a Bidirectional Long Short-Term Memory (Bi-LSTM) network, and an LSTM network with dropout.

## Dataset

The dataset used in this project is sourced from the [Brown Corpus](https://en.wikipedia.org/wiki/Brown_Corpus). It is a real-world dataset with sequences of words and corresponding tags. The data is loaded, preprocessed, and split into training, validation, and test sets.

## Models

### LSTM with Dropout

The LSTM model with dropout is implemented to prevent overfitting. It consists of an embedding layer, a two-layer LSTM with dropout, and a linear layer for predictions.

### Bi-LSTM

The Bidirectional LSTM model aims to capture temporal dependencies in both forward and backward directions. It includes an embedding layer, a bidirectional LSTM layer, and a linear layer for predictions.

### CNN

The Convolutional Neural Network model utilizes convolutions to capture local patterns in the sequences. It comprises an embedding layer, convolutional layers with max-pooling, and a linear layer for predictions.

## Training

Each model is trained using the SGD optimizer and cross-entropy loss. The training process involves iterating through epochs and updating model parameters based on backpropagation.

## Evaluation

The performance of each model is evaluated on validation and test sets using accuracy metrics. The Bi-LSTM model demonstrated the highest accuracy, highlighting its effectiveness in capturing temporal dependencies.

## Future Work

Possible avenues for future work include:

- Fine-tuning hyperparameters for further optimization.
- Exploring different architectures or combinations of models.
- Experimenting with additional regularization techniques.
