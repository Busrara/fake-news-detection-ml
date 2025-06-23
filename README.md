# fake-news-detection-ml

This project is a machine learning-based application that can predict whether a news article is **real** or **fake**. It has both a training pipeline and a user-friendly interface built with **Streamlit**.

## Features

- Trains and compares multiple models: **Naive Bayes**, **Logistic Regression**, and **Random Forest**.
- Automatically selects and saves the **best-performing model**.
- Uses **TF-IDF vectorization** to convert text into numerical features.
- A clean and interactive Streamlit app for users to test new articles.

## How it Works

1. **Data Loading:** Combines true and fake news datasets.
2. **Preprocessing:** Cleans text and extracts simple features.
3. **Training:** Tests 3 models and selects the best based on accuracy.
4. **Saving:** Stores the model, vectorizer, and model info as `.pkl` files.
5. **Prediction:** In the app, the model predicts using TF-IDF features.

** Ps: This app is not deployed. To test the app locally, run train-model.py first to train and save the models, then use st.py to launch the Streamlit interface. **

## 🛠️ Installation

```bash
git clone https://github.com/Busraracoban/fake-news-detection-ml.git
cd fake-news-detection-ml
pip install -r requirements.txt
