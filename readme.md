# Deep Learning Lab Works 

Welcome to the **Deep Learning Lab Works** repository! This repository contains a series of practical, hands-on laboratory exercises focusing on various Deep Learning concepts. The labs cover everything from basic neural networks to advanced architectures, transfer learning, natural language processing, and explainable AI.

---

## Table of Contents

- [Overview](#-overview)
- [Lab Breakdown](#-lab-breakdown)
- [Tech Stack](#-tech-stack)
- [Getting Started](#-getting-started)
- [Running the Streamlit App (Lab 7)](#-running-the-streamlit-app-lab-7)

---

## Overview

This repository serves as a structured learning path for Deep Learning. It transitions from fundamental concepts like artificial neural networks (ANNs) using MNIST, to convolutional neural networks (CNNs), recurrent neural networks (RNNs) for NLP, transfer learning with VGG16, and interpretability using LIME. It also features an AI Assistant web application integrated with the Gemini API.

---

## Lab Breakdown

| Lab | Topic | Dataset | Key Concepts |
| :---: | :--- | :--- | :--- |
| **Lab 1** | **Introduction to Neural Networks** | MNIST | Basics of TensorFlow/Keras, Multilayer Perceptrons (MLP), Image Classification. |
| **Lab 2** | **Regularization & Optimization** | MNIST | Dropout, Batch Normalization, L2 Regularization, preventing overfitting. |
| **Lab 3** | **Advanced Training Techniques** | MNIST | Custom Callbacks, Learning Rate Scheduling, model optimization. |
| **Lab 4** | **Convolutional Neural Networks (CNN)** | CIFAR-10 / Custom | Building CNNs, Convolution layers, Pooling, Feature extraction. |
| **Lab 5** | **Transfer Learning with VGG16** | CIFAR-10 | Pre-trained models, Feature Extraction (Frozen Base), Fine-Tuning. |
| **Lab 6** | **Natural Language Processing (NLP)** | IMDb Reviews | Text processing, Sequence Padding, Recurrent Neural Networks (RNN/LSTM). |
| **Lab 7** | **AI Assistant App (AskAI)** | N/A | Generative AI, Streamlit, LangChain, Google Gemini 2.5 Flash Lite API. |
| **Lab 8** | **Explainable AI (XAI) using LIME** | MNIST / Custom | PyTorch basics, Local Interpretable Model-agnostic Explanations (LIME). |

---

## Tech Stack

- **Languages:** Python
- **Deep Learning Frameworks:** TensorFlow, Keras, PyTorch
- **Web App Framework:** Streamlit
- **Generative AI:** LangChain, Google Gemini API
- **Data Science Libraries:** NumPy, Matplotlib, JSON
- **Environment:** Jupyter Notebooks (`.ipynb`)

---

## Getting Started

### Prerequisites

Make sure you have Python 3.8+ installed along with `pip` and `jupyter`. 

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/deep-learning-labs.git
   cd deep-learning-labs
   ```

2. **Create a virtual environment (optional but recommended):**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install the required dependencies:**
   *(A `requirements.txt` might be needed. If not, you can install the core packages manually)*
   ```bash
   pip install tensorflow torch torchvision numpy matplotlib jupyter streamlit langchain-google-genai python-dotenv
   ```

4. **Launch Jupyter Notebook to view the labs:**
   ```bash
   jupyter notebook
   ```

---

## Running the Streamlit App (Lab 7)

Lab 7 contains a functional AI Assistant Chatbot built with Streamlit and LangChain.

1. Navigate to the `dl_lab7` directory:
   ```bash
   cd dl_lab7
   ```

2. Set up your environment variables:
   - Create a `.env` file in the `dl_lab7` directory.
   - Add your Google Gemini API key:
     ```env
     GOOGLE_API_KEY=your_api_key_here
     ```

3. Run the Streamlit app:
   ```bash
   streamlit run app.py
   ```

---