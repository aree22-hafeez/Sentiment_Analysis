#🎬 IMDB Sentiment Analysis using LSTM

This project is a deep learning model that predicts whether a movie review is positive or negative.
It uses the IMDB dataset and builds a neural network with LSTM (Long Short-Term Memory) to understand text.

The goal is to learn how machine learning can analyze human language and classify sentiment.
--------------------------------------------------------------------
#🚀 Features
🧠 Deep Learning Model — Uses Bidirectional LSTM to capture context from both directions
🔤 Text Preprocessing — Converts text into sequences and pads them to a fixed length
📊 Word Embeddings — Learns semantic word representations using an embedding layer
📉 Overfitting Control — Uses Dropout layers and EarlyStopping
⚖️ Binary Classification — Predicts sentiment as Positive or Negative
📦 Vocabulary Filtering — Uses the top 10,000 most frequent words
⏱️ Fixed Input Size — Pads all reviews to 200 words
--------------------------------------------------------------------
# 🧠 Model Architecture

```bash
Input Layer (Tokenized review sequence)
        ↓
Embedding Layer (128-dimensional word vectors)
        ↓
Bidirectional LSTM (128 units)
        ↓
Dense Layer (64 neurons, ReLU activation)
        ↓
Dropout Layer (0.5)
        ↓
Output Layer (Sigmoid activation)
```bash
--------------------------------------------------------------------
##Training Setup
Loss function: Binary Crossentropy
Optimizer: Adam
Metric: Accuracy
Early Stopping:
- Monitors validation loss
- Stops training if no improvement for 3 epochs
- Restores best model weights
--------------------------------------------------------------------
##🛠️ Tech Stack

Python Ecosystem

NumPy
Matplotlib
Seaborn

Deep Learning

TensorFlow / Keras
LSTM (RNN)
Embedding Layer

Utilities
Scikit-learn (metrics: accuracy, classification report, confusion matrix)
------------------------------------------------------------------------------
#📈 How It Works
Movie review is given as input
Text is converted into numerical sequence
Embedding layer converts words into vectors
Bidirectional LSTM learns sentence context
Final dense layer predicts sentiment score
Output is classified as Positive or Negative
