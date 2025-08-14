# Next-Word-Prediction-Model-using-LSTM-Neural-Networks

## Project Overview
This project implements a **Next Word Prediction model** using **LSTM (Long Short-Term Memory) networks** in TensorFlow/Keras. The model is trained on a cleaned version of Franz Kafka's *Metamorphosis* to predict the next word given a seed word. It demonstrates **sequence modeling**, **tokenization**, and **text generation** using deep learning.

**Key Features:**
- Text preprocessing including punctuation removal and duplicate word filtering.
- Tokenization using `Tokenizer` to convert words to integer sequences.
- Sequence creation for next-word prediction.
- LSTM-based neural network with an embedding layer.
- One-hot encoding of target words using `to_categorical`.
- Callbacks for **model checkpointing**, **learning rate reduction**, and **TensorBoard visualization**.
- Generation of text sequences using a trained model.

---

## Dataset
- Source: [Project Gutenberg - Metamorphosis](http://www.gutenberg.org/cache/epub/5200/pg5200.txt)
- The file `metamorphosis_clean.txt` is a cleaned version with unnecessary text removed.
- Lines are concatenated into a single string, punctuation is replaced with spaces, and duplicate words are removed to create a unique word sequence dataset.

---

## Setup & Installation
```bash
git clone https://github.com/your-username/next-word-prediction.git
cd next-word-prediction
pip install tensorflow numpy pickle5
