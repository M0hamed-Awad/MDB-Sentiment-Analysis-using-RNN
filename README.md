# IMDB Sentiment Analysis using RNN

This project performs Sentiment Analysis on IMDB movie reviews using a Recurrent Neural Network (RNN) implemented with TensorFlow/Keras. The goal is to classify each movie review as positive or negative based on its content.

---

## Overview

This project demonstrates how to build a simple RNN model for sentiment analysis using the IMDB movie reviews dataset. It includes model building, training, evaluation, and visualization of results.

---

## Model Architecture

- **Embedding Layer**: Converts words into dense vector representations.
- **Simple RNN Layer**: Captures the sequential relationships in the review text.
- **Dense Output Layer**: Single neuron with sigmoid activation for binary classification.

---

## Technologies Used

- Python 3
- TensorFlow / Keras
- Matplotlib (for visualization)
- Google Colab or Jupyter Notebook

---

## Dataset

- Dataset: IMDB movie reviews
- Automatically loaded using:
  ```python
  from tensorflow.keras.datasets import imdb
  ```
- Only the top 10,000 most frequent words are used:
  ```python
  num_words=10000
  ```

---

## How to Run

### Option 1: Run on Google Colab

1. Open the `.ipynb` notebook file in Google Colab.
2. To upload it to GitHub:
   - Click `File > Save a copy in GitHub`.
   - Choose the repository and filename, then click **OK**.

### Option 2: Download and Upload Manually

1. In Google Colab, click `File > Download > Download .ipynb`.
2. Go to your GitHub repository and upload the `.ipynb` file directly.

### Option 3: Run Locally (Optional)

If you convert the code to a Python script, you can run it locally:

```bash
pip install tensorflow matplotlib
python sentiment_rnn.py
```

---

## Output Example

- **Training & Validation Accuracy and Loss** are printed during training.
- **Accuracy and Loss charts** are displayed after training ends.

Tip: You can save the charts as an image using:

```python
plt.savefig('output.png')
```

and upload it to your repository.

---

## Results

- Accuracy may vary depending on model parameters.
- Example: **Test Accuracy ~85% after 5 epochs**.
