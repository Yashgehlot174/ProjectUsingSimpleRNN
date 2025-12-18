# IMDB Movie Review Sentiment Analysis (Simple RNN)

This project implements a **movie review sentiment analysis system** using a **Simple Recurrent Neural Network (RNN)** trained on the **IMDB dataset**. The model classifies user-provided movie reviews as **Positive** or **Negative** and is deployed using **Streamlit** for an interactive web interface.

---

## 📌 Project Overview

- Uses the IMDB movie review dataset from Keras
- Implements a Simple RNN-based deep learning model
- Performs text preprocessing, tokenization, and padding
- Loads a pre-trained model (`.h5`) for inference
- Provides a user-friendly Streamlit web app

---

## 🧠 Model Details

- **Model type:** Simple RNN
- **Framework:** TensorFlow / Keras
- **Activation:** ReLU (hidden layers)
- **Output:** Binary classification (Positive / Negative)
- **Max sequence length:** 500 words

The model predicts a **sentiment score between 0 and 1**:
- `> 0.5` → Positive Review
- `≤ 0.5` → Negative Review

---

## 📂 Project Structure

```
├── main.py                 # Streamlit application
├── simple_rnn_imdb.h5      # Pre-trained RNN model
├── requirements.txt        # Project dependencies
├── simplernn.ipynb         # Model training notebook
├── embedding.ipynb         # Word embedding exploration
├── prediction.ipynb        # Prediction and evaluation notebook
├── LICENSE                 # License file
├── README.md               # Project documentation
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the repository
```bash
git clone https://github.com/Yashgehlot174/ProjectUsingSimpleRNN.git
```

### 2️⃣ Create a virtual environment (optional but recommended)
```bash
python -m venv venv
source venv/bin/activate   # On Windows: venv\\Scripts\\activate
```

### 3️⃣ Install dependencies
```bash
pip install -r requirements.txt
```

---

## ▶️ Running the Application

Launch the Streamlit app using:
```bash
streamlit run main.py
```

Then open the provided local URL in your browser.

---

## 📝 How It Works

1. User enters a movie review in text form
2. Text is converted into word indices using IMDB word index
3. The sequence is padded to a fixed length
4. The pre-trained Simple RNN model predicts sentiment
5. The result (Positive/Negative) and confidence score are displayed

---

## 📊 Example Output

- **Input:** "The movie was amazing with great performances"
- **Sentiment:** Positive
- **Prediction Score:** 0.91

---

## 🚀 Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Streamlit
- Jupyter Notebook

---

## 📌 Future Improvements

- Use LSTM / GRU for better long-term dependency learning
- Add word embedding visualization
- Improve UI with sentiment probability graphs
- Deploy on cloud platforms (Streamlit Cloud / AWS / GCP)

---

## 👤 Author

**Yash Gehlot**  
IIT Roorkee  

---

## 📜 License

This project is licensed under the terms of the license provided in the `LICENSE` file.

---

⭐ If you find this project useful, feel free to star the repository!

