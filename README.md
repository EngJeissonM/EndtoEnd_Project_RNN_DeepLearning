# EndtoEnd_Project_RNN_DeepLearning

🎬 IMDB Movie Review Sentiment Analysis (RNN + Streamlit)

This project is an end-to-end Sentiment Analysis web application built using a Recurrent Neural Network (RNN) trained on the IMDB movie reviews dataset.
The app allows users to enter a movie review and classifies it as Positive or Negative using a pre-trained deep learning model.

The interface is built with Streamlit, making the model easy to interact with through a simple web UI.

🚀 Features

Deep Learning model based on Simple RNN

Trained on the IMDB movie reviews dataset

Real-time sentiment prediction

Clean and interactive Streamlit web interface

Displays both sentiment label and prediction confidence score

🧠 Model Overview

Architecture: Simple Recurrent Neural Network (RNN)

Activation Function: ReLU

Output: Binary classification (Positive / Negative)

Dataset: IMDB Movie Reviews (Keras built-in dataset)

Max sequence length: 500 tokens

The model was trained beforehand and saved as:

simple_rnn_imdb.h5

🛠️ Technologies Used

Python

TensorFlow / Keras

NumPy

Streamlit

IMDB Dataset (Keras)

📂 Project Structure
├── app.py                     # Streamlit application
├── simple_rnn_imdb.h5         # Pre-trained RNN model
├── README.md                  # Project documentation

⚙️ Installation & Setup

Clone the repository

git clone https://github.com/your-username/imdb-sentiment-rnn.git
cd imdb-sentiment-rnn


Create a virtual environment (optional but recommended)

python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate


Install dependencies

pip install tensorflow numpy streamlit

▶️ How to Run the App

Run the Streamlit application with:

streamlit run app.py


Then open the local URL shown in your terminal (usually http://localhost:8501).

🧪 How It Works

The user enters a movie review.

The text is:

Lowercased

Tokenized using the IMDB word index

Padded to a fixed length

The preprocessed input is passed to the RNN model.

The model outputs a probability score:

> 0.5 → Positive

≤ 0.5 → Negative

The sentiment and prediction score are displayed.

📊 Example Output
Sentiment: Positive
Prediction Score: 0.87

📌 Future Improvements

Replace Simple RNN with LSTM or GRU

Add word embeddings visualization

Improve text preprocessing (handling punctuation, OOV words)

Deploy the app on Streamlit Cloud or Hugging Face Spaces

👤 Author

Jeisson Morales
Industrial Engineer | Data Science & AI Enthusiast
🇨🇴 Colombia
