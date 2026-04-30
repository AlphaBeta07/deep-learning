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

| Lab | Topic | Dataset | Key Concepts | File Location |
| :---: | :--- | :--- | :--- | :--- |
| **Lab 1** | **Introduction to Neural Networks** | MNIST | Implementing foundational Multilayer Perceptron (MLP) architectures using TensorFlow/Keras. Covers data flattening, building sequential dense models, compiling with optimizers, and evaluating classification accuracy. | [`dl_lab1.ipynb`](./dl_lab1.ipynb) |
| **Lab 2** | **Regularization & Optimization** | MNIST | Addressing model overfitting through advanced techniques: applying Dropout layers, implementing Batch Normalization to stabilize learning, and utilizing L2 Regularization to constrain model weights. | [`dl_lab2.ipynb`](./dl_lab2.ipynb) |
| **Lab 3** | **Advanced Training Techniques** | MNIST | Enhancing training loops using Custom Callbacks to dynamically monitor performance, and implementing Learning Rate Scheduling to adjust step sizes across epochs for optimal convergence. | [`dl_lab3.ipynb`](./dl_lab3.ipynb) |
| **Lab 4** | **Convolutional Neural Networks (CNN)** | CIFAR-10 | Constructing CNNs for spatial feature extraction. Concepts include 2D Convolutions, MaxPooling for downsampling, flatten operations, and plotting training graphs for loss and accuracy. | [`dl_lab4.ipynb`](./dl_lab4.ipynb) |
| **Lab 5** | **Transfer Learning with VGG16** | CIFAR-10 | Utilizing a pre-trained VGG16 model. Covers freezing base layers for rapid feature extraction, replacing the classifier head, and fine-tuning by unfreezing final layers with a reduced learning rate. | [`dl_lab5.ipynb`](./dl_lab5.ipynb) |
| **Lab 6** | **Natural Language Processing (NLP)** | IMDb Reviews | Text classification for sentiment analysis. Includes tokenization, sequence padding for uniform length, word embeddings, and training sequential models using Recurrent Neural Networks (LSTM/RNN). | [`dl_lab6.ipynb`](./dl_lab6.ipynb) |
| **Lab 7** | **AI Assistant App (AskAI)** | N/A | Developing an interactive chatbot using Streamlit. Features LangChain integration with Google's Gemini 2.5 Flash Lite API, state management for session history, and real-time streaming text responses. | [`dl_lab7/`](./dl_lab7/) |
| **Lab 8** | **Explainable AI (XAI) using LIME** | Custom | Transitioning to PyTorch to build neural networks and applying Local Interpretable Model-agnostic Explanations (LIME) to demystify "black-box" model predictions using image superpixels. | [`dl_lab8.ipynb`](./dl_lab8.ipynb) |

---

## Tech Stack

- **Languages:** Python
- **Deep Learning Frameworks:** TensorFlow, Keras, PyTorch
- **Web App Framework:** Streamlit
- **Generative AI:** LangChain, Google Gemini API
- **Data Science Libraries:** NumPy, Matplotlib, JSON
- **Environment:** Google Colab, Jupyter Notebooks (`.ipynb`)

---

## Getting Started

These labs were developed and executed using **Google Colab**, which provides free access to GPUs for training deep learning models.

### Running on Google Colab (Recommended)

1. Navigate to [Google Colab](https://colab.research.google.com/).
2. Click on **File > Upload notebook**.
3. Upload the desired `.ipynb` file from this repository.
4. If a lab requires a GPU (like CNNs or VGG16), go to **Runtime > Change runtime type** and select **T4 GPU**.
5. Run the cells!

### Running Locally

#### Prerequisites
Make sure you have Python 3.8+ installed along with `pip` and `jupyter`. 

#### Installation

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
   *(Note: Core deep learning libraries are pre-installed on Colab. Install these only if you are setting up a local environment for Lab 7 or local execution).*
   ```bash
   pip install tensorflow torch torchvision numpy matplotlib streamlit langchain-google-genai python-dotenv
   ```

4. **View and Run the Labs:**
   Instead of launching a local Jupyter server, simply upload the `.ipynb` files to [Google Colab](https://colab.research.google.com/) to utilize their cloud environment and free GPUs.

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