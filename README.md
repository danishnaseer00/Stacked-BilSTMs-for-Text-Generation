# Stacked BiLSTMs for Text Generation

This project implements a **Stacked Bidirectional LSTM (BiLSTM)** model for **character-level text generation** using the famous **Tiny Shakespeare** dataset.  
It demonstrates how deep recurrent neural networks can learn sequential dependencies and generate new text in the style of the training data.

## 📜 Project Overview

- **Dataset**: [Tiny Shakespeare](https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt)  
- **Approach**: Character-level modeling using Stacked Bidirectional LSTMs  
- **Framework**: TensorFlow/Keras  
- **Goal**: Generate Shakespeare-like text from scratch by training on character sequences.

## 🚀 Features

- Data preprocessing and character encoding  
- Vocabulary creation and sequence preparation  
- Stacked **BiLSTM** architecture with dropout for regularization  
- Model checkpointing and early stopping  
- Training history visualization (loss & accuracy curves)  
- Text generation from trained model

## 📊 Model Architecture

- Embedding Layer – Maps characters to dense vectors
- BiLSTM Layer 1 – 512 units, return sequences, dropout & recurrent dropout
- BiLSTM Layer 2 – 512 units, dropout & recurrent dropout
- Dense Layer – Softmax activation for character prediction
