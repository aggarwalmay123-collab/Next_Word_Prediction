# 🚀 Next Word Prediction Using LSTM and RNN

A Deep Learning based Next Word Prediction System built using TensorFlow, Keras, RNN, and LSTM. The application predicts the next word based on the text entered by the user and provides an interactive interface using Streamlit.

---

## 📌 Project Description

The goal of this project is to predict the next word in a sequence of text using Natural Language Processing (NLP) and Deep Learning techniques.

The model is trained on a dataset of quotes and learns word patterns to generate meaningful predictions. Both Recurrent Neural Network (RNN) and Long Short-Term Memory (LSTM) architectures were implemented and compared, with LSTM selected as the final model due to its better performance.

---

## ✨ Features

- Text preprocessing and cleaning
- Tokenization using TensorFlow/Keras
- One-Hot Encoding for output labels
- Sequence generation for training
- Sequence padding
- RNN implementation
- LSTM implementation
- Next word prediction
- Interactive Streamlit web application
- Saved model and tokenizer for deployment

---

## 🛠️ Technologies Used

### Languages
- Python

### Libraries
- TensorFlow
- Keras
- NumPy
- Pandas
- Streamlit
- Pickle
- Matplotlib

### Deep Learning Models
- Recurrent Neural Network (RNN)
- Long Short-Term Memory (LSTM)

---

## 📂 Project Structure

```bash
Next-Word-Prediction/
│
├── app.py                  # Streamlit User Interface
├── model_training.py       # Training Script
├── lstm_model.h5           # Trained LSTM Model
├── tokenizer.pkl           # Saved Tokenizer
├── max_len.pkl             # Maximum Sequence Length
├── dataset.csv             # Training Dataset
├── requirements.txt        # Project Dependencies
└── README.md               # Project Documentation
```

---

## ⚙️ How It Works

### Step 1: Data Preprocessing

- Convert text to lowercase
- Remove punctuation
- Tokenize text
- Create vocabulary
- Generate input-output sequences

### Step 2: One-Hot Encoding

The target word is converted into a one-hot encoded vector for multi-class classification.

### Step 3: Sequence Padding

Input sequences are padded to ensure equal length before training.

### Step 4: Model Training

#### RNN Architecture

```text
Embedding Layer
      ↓
Simple RNN Layer
      ↓
Dense Layer
```

#### LSTM Architecture

```text
Embedding Layer
      ↓
LSTM Layer
      ↓
Dense Layer
```

### Step 5: Prediction

The trained model predicts the most probable next word based on the user's input sequence.

---

## 🧠 Model Architecture

```python
Embedding(input_dim=10000, output_dim=50)
LSTM(128)
Dense(10000, activation='softmax')
```


## 💻 Usage

1. Open the Streamlit application.
2. Enter a text sequence.
3. Click the Predict button.
4. View the predicted next word.

### Example

Input:

```text
What are you
```

Output:

```text
worrying
```

---

## 📊 Key Concepts Used

- Natural Language Processing (NLP)
- Tokenization
- Vocabulary Building
- Sequence Modeling
- One-Hot Encoding
- Word Embeddings
- RNN
- LSTM
- Deep Learning
- Streamlit Deployment

