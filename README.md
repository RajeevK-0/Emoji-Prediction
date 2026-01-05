# 🎭 Text-to-Emoji Predictor with LSTM

A Deep Learning project that classifies text sentences and predicts the most appropriate emoji to represent the sentiment or context. Built using Python, Keras/TensorFlow, and GloVe word embeddings.

## 🚀 Project Overview
This project solves a multi-class classification problem in Natural Language Processing (NLP). By analyzing the semantic meaning of input sentences, the model predicts one of 5 target emojis (❤️, ⚾, 😄, 😓, 🍴). 

It utilizes **Long Short-Term Memory (LSTM)** networks to handle sequential data and **GloVe (Global Vectors)** for pre-trained word embeddings to understand word relationships.

## 🛠️ Tech Stack
* **Language:** Python 3.x
* **Deep Learning:** Keras (TensorFlow backend)
* **Data Manipulation:** Pandas, NumPy
* **NLP Tools:** GloVe Word Embeddings (50d), Emoji library

## 📂 Dataset
The model relies on three key data files:
1.  **`train_emoji.csv`**: Training dataset containing sentences and labels.
2.  **`test_emoji.csv`**: Testing dataset for validation.
3.  **`glove.6B.50d.txt`**: Pre-trained word vectors (Stanford NLP) to map words to 50-dimensional geometric vectors.

## 🧠 Model Architecture
The model is built using a Sequential API with the following layers:
1.  **Input Layer:** Processes sequences of text (padded/truncated to fixed length).
2.  **LSTM Layer (32 units):** Returns sequences to capture high-level context.
3.  **LSTM Layer (16 units):** Captures temporal dependencies in the text.
4.  **Dropout (0.3):** Regularization layer to prevent overfitting.
5.  **Dense Layer (Softmax):** Output layer with 5 units for multi-class probability distribution.

## 🔧 Installation & Usage

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/YOUR-USERNAME/emoji-predictor.git](https://github.com/YOUR-USERNAME/emoji-predictor.git)
   cd emoji-predictor
