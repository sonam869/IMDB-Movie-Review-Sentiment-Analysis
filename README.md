# 🎬 IMDB Movie Review Sentiment Analysis

A Streamlit-based web application that uses a Simple RNN model built with TensorFlow/Keras to classify movie reviews as **positive** or **negative**.

## 🚀 Features

* ✅ Real-time sentiment prediction
* ✅ Pre-trained SimpleRNN model
* ✅ Interactive web interface using Streamlit
* ✅ Confidence score for each prediction
* ✅ Text preprocessing with tokenization and padding
* ✅ Binary classification (Positive / Negative)

---

---

## 📂 Project Structure

```text
simple_rnn_imdb/
├── main.py                      # Streamlit application
├── simple_rnn_imdb.keras        # Trained SimpleRNN model
├── embedding.ipynb              # Embedding layer experiments
├── simplernn.ipynb              # Model training notebook
├── prediction.ipynb             # Prediction examples
├── requirements.txt             # Dependencies
├── README.md                    # Project documentation
└── assets/
    └── demo.png                 # Application screenshot
```

---

## 🛠️ Tech Stack

* Python 3.11
* TensorFlow 2.15
* Keras
* Streamlit
* NumPy
* Jupyter Notebook

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/sonam869/IMDB-Movie-Review-Sentiment-Analysis.git

cd IMDB-Movie-Review-Sentiment-Analysis
```

### 2. Create a virtual environment

```bash
py -3.11 -m venv venv

venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install --upgrade pip

pip install -r requirements.txt
```

---

## ▶️ Run the Application

```bash
streamlit run main.py
```

Open your browser and visit:

```text
http://localhost:8501
```

---

## 🧠 Model Information

| Parameter               | Value                 |
| ----------------------- | --------------------- |
| Model Type              | SimpleRNN             |
| Dataset                 | IMDB Movie Reviews    |
| Training Samples        | 25,000                |
| Vocabulary Size         | 10,000 words          |
| Maximum Sequence Length | 500                   |
| Output Layer            | Sigmoid               |
| Task                    | Binary Classification |

---

## 📝 Example

### Input

> "This movie was absolutely amazing! Great plot and excellent acting."

### Output

```text
Sentiment: Positive
Confidence Score: 0.92
```

---

## 📋 Requirements

* Python 3.11 (recommended)
* TensorFlow 2.15.0
* Streamlit
* NumPy

Install all dependencies with:

```bash
pip install -r requirements.txt
```

Example `requirements.txt`:

```text
tensorflow==2.15.0
streamlit>=1.35.0
numpy>=1.26.0
```

---

## ⚠️ Compatibility Note

The model was trained using **TensorFlow 2.15** and may not load correctly with **Keras 3** or **Python 3.13**.

For best compatibility, use:

* Python 3.11
* TensorFlow 2.15.0

Load the model using:

```python
from tensorflow.keras.models import load_model

model = load_model("simple_rnn_imdb.keras")
```

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome.

Feel free to fork this repository and submit a pull request.

---

## 👤 Author

GitHub: [@sonam869](https://github.com/sonam869)

---

## 📄 License

This project is licensed under the MIT License.
