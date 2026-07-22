# 🤖 Intelligent Intent-Based Chatbot with Neural Networks

> **A Deep Learning-based Conversational AI built using TensorFlow, Natural Language Processing (NLP), and Intent Classification, with an experimental integration of Wikipedia for external knowledge retrieval.**

This repository demonstrates the development of an **intent-based chatbot** capable of understanding natural language queries and generating appropriate responses using a **feed-forward neural network** trained on a custom intent dataset.

The project follows the complete NLP pipeline—from text preprocessing and vocabulary creation to model training, intent prediction, and real-time conversation. It also includes experimental versions that explore additional features and external knowledge retrieval.

---

# 🚀 Project Highlights

- 🤖 Intent-based conversational chatbot
- 🧠 Deep Neural Network using TensorFlow/Keras
- 📚 Natural Language Processing (NLTK)
- 📝 Text preprocessing and lemmatization
- 🎯 Intent classification
- 💬 Interactive command-line conversation
- 📦 Vocabulary and model persistence
- 🌐 Experimental Wikipedia integration
- 📓 Beginner-friendly Google Colab implementation

---

# 📖 Project Overview

Unlike rule-based chatbots that rely solely on predefined conditions, this chatbot uses **Natural Language Processing** and a **Neural Network classifier** to identify the user's intent before selecting an appropriate response.

The chatbot learns from a custom **`intents.json`** dataset containing:

- User patterns
- Intent labels
- Multiple possible responses

During inference, the chatbot predicts the most probable intent and returns a suitable response from the corresponding intent category.

---

# 🎯 Objectives

The project aims to:

- Understand natural language user inputs.
- Train a neural network for intent classification.
- Build a reusable NLP preprocessing pipeline.
- Develop an interactive conversational chatbot.
- Demonstrate the complete machine learning workflow behind modern chatbots.
- Explore integration with external knowledge sources.

---

# 🔄 Project Workflow

```
User Message
      │
      ▼
Text Preprocessing
      │
      ▼
Tokenization
      │
      ▼
Lemmatization
      │
      ▼
Bag-of-Words Vector
      │
      ▼
Neural Network Prediction
      │
      ▼
Intent Classification
      │
      ▼
Response Selection
      │
      ▼
Bot Response
```

---

# 🧩 Project Structure

## 1. Import Required Libraries

- TensorFlow
- NumPy
- NLTK
- Pickle
- JSON
- Random

---

## 2. Dataset Loading

- Load custom `intents.json`
- Read user patterns
- Read chatbot responses

---

## 3. NLP Preprocessing

The preprocessing pipeline includes:

- Tokenization
- Lowercasing
- Lemmatization
- Removal of punctuation
- Vocabulary generation

---

## 4. Training Dataset Preparation

The chatbot converts text into numerical vectors using the **Bag-of-Words** approach.

The training pipeline includes:

- Vocabulary creation
- Intent encoding
- One-hot encoding
- Feature matrix generation

---

## 5. Neural Network Architecture

The chatbot uses a simple yet effective feed-forward neural network consisting of:

- Dense Layer (128 neurons)
- Dropout Layer
- Dense Layer (64 neurons)
- Dropout Layer
- Softmax Output Layer

The model is trained using:

- Categorical Crossentropy Loss
- SGD Optimizer
- Momentum
- Nesterov Acceleration

---

## 6. Model Training

- 200 Training Epochs
- Mini-batch learning
- Accuracy monitoring
- Model persistence

Generated files include:

- `chatbot_model.h5`
- `words.pkl`
- `classes.pkl`

---

## 7. Intent Prediction

The chatbot performs:

- Sentence preprocessing
- Bag-of-Words conversion
- Neural network inference
- Confidence threshold filtering
- Intent ranking

---

## 8. Response Generation

Once the predicted intent is identified, the chatbot:

- Finds the matching intent
- Selects a random response
- Returns it to the user

This creates more natural conversations by avoiding repetitive replies.

---

## 9. Interactive Chat

The notebook provides a real-time command-line chatbot where users can interact continuously until termination.

---

## 10. Experimental Wikipedia Integration

One experimental component demonstrates how the chatbot can retrieve factual information directly from **Wikipedia** using the `wikipedia-api` package.

This opens the possibility of extending the chatbot beyond predefined responses into a knowledge-assisted conversational system.

---

# 🧠 Machine Learning & NLP Concepts Covered

This project introduces several important concepts, including:

- Natural Language Processing (NLP)
- Intent Classification
- Text Tokenization
- Lemmatization
- Bag-of-Words Representation
- One-Hot Encoding
- Feed-Forward Neural Networks
- Softmax Classification
- Model Persistence
- Conversational AI

---

# 📊 Model Pipeline

The chatbot follows a complete machine learning workflow:

```
Dataset
    │
    ▼
Preprocessing
    │
    ▼
Vocabulary Building
    │
    ▼
Feature Engineering
    │
    ▼
Neural Network Training
    │
    ▼
Model Saving
    │
    ▼
Intent Prediction
    │
    ▼
Chat Interface
```

---

# 🛠️ Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- NLTK
- Pickle
- JSON
- Wikipedia API
- Google Colab

---

# 💬 Example Conversation

```
You : Hello

Bot : Hi! How can I help you today?

-------------------------------------

You : Tell me about Albert Einstein

Bot : Albert Einstein was a German-born theoretical physicist...
```

---

# 📂 Repository Structure

```
.
├── Chatbot3.ipynb
├── Chatbot3 (1).ipynb
├── Chatbot5 (working).ipynb
├── intents.json
├── chatbot_model.h5
├── words.pkl
├── classes.pkl
└── README.md
```

---

# 📌 Notebook Versions

This repository contains multiple development versions that document the evolution of the chatbot.

### 🔹 Chatbot3.ipynb

The initial implementation of the chatbot, covering the complete NLP preprocessing pipeline, intent classification, neural network training, and interactive conversation.

---

### 🔹 Chatbot3 (1).ipynb

An intermediate development version that includes refinements to preprocessing, training workflow, and chatbot behavior while serving as an experimental checkpoint during development.

---

### 🔹 Chatbot5 (working).ipynb ⭐

The latest and fully functional implementation.

Additional features include:

- Improved training pipeline
- Cleaner prediction workflow
- Better response handling
- Saved model loading
- Experimental Wikipedia integration for external knowledge retrieval

This notebook represents the recommended version for running the chatbot.

---

# 🎯 Applications

The techniques demonstrated in this project can be extended to build:

- Customer Support Chatbots
- Educational Assistants
- FAQ Bots
- College Help Desks
- Healthcare Assistants
- Banking Chatbots
- Retail Support Systems
- Personal AI Assistants

---

# 🎓 Learning Outcomes

After completing this project, readers will understand:

- How conversational AI systems process language.
- How NLP transforms text into numerical features.
- How intent classification works.
- How neural networks power chatbots.
- How chatbot models are trained and deployed.
- How external knowledge sources can enhance conversational systems.

---

# 📌 Future Improvements

Potential enhancements include:

- Transformer-based models (BERT, RoBERTa)
- Retrieval-Augmented Generation (RAG)
- Large Language Model (LLM) integration
- Voice-based interaction
- Streamlit web application
- Context-aware conversations
- Conversation history memory
- Multilingual support
- Sentiment-aware responses
- Vector database integration (FAISS/ChromaDB)

---

# 🤝 Contributions

Contributions are welcome! Feel free to fork this repository, improve the chatbot, or submit pull requests.

---

# ⭐ Support the Project

If you found this repository useful for learning **Natural Language Processing**, **Deep Learning**, or **Conversational AI**, consider giving it a **⭐ Star** to support the project.
