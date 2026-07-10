# 📧 Email / SMS Spam Classifier

A machine learning web app that classifies messages as **Spam** or **Not Spam** using Natural Language Processing (NLP) and a trained Naive Bayes model. Built with **Streamlit**.

---

## 🚀 Demo

Enter any email or SMS message in the text box and click **Predict** to instantly find out if it's spam.

---

## 🧠 How It Works

1. **Text Preprocessing** — The input message is lowercased, tokenized, and cleaned (removes punctuation & stopwords).
2. **Stemming** — Words are reduced to their root form using Porter Stemmer.
3. **TF-IDF Vectorization** — The preprocessed text is converted into a numerical vector.
4. **Prediction** — A pre-trained machine learning model predicts whether the message is spam or not.

---

## 🗂️ Project Structure

```
ml project/
│
├── app.py              # Streamlit web application
├── main.ipynb          # Jupyter notebook (EDA, training & evaluation)
├── model.pkl           # Trained ML model (serialized)
├── vectorizer.pkl      # TF-IDF vectorizer (serialized)
├── spam.csv            # Dataset used for training
├── requirements.txt    # Python dependencies
└── README.md           # Project documentation
```

---

## 📦 Installation

### 1. Clone the repository

```bash
git clone https://github.com/sumitksr/Email-Spam-Classifier.git
cd Email-Spam-Classifier
```

### 2. Create a virtual environment (optional but recommended)

```bash
python -m venv venv
venv\Scripts\activate      # On Windows
# source venv/bin/activate  # On macOS/Linux
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Running the App

```bash
streamlit run app.py
```

The app will open automatically in your browser at `http://localhost:8501`.

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Python | Core programming language |
| Streamlit | Web application framework |
| scikit-learn | Machine learning model & TF-IDF |
| NLTK | Natural language processing |
| Pandas & NumPy | Data manipulation |
| Pickle | Model serialization |

---

## 📊 Dataset

The model was trained on the **SMS Spam Collection Dataset** (`spam.csv`), which contains labeled SMS messages tagged as either `ham` (not spam) or `spam`.

---

## 🤖 Model

- **Algorithm**: Naive Bayes (MultinomialNB)
- **Vectorizer**: TF-IDF (Term Frequency-Inverse Document Frequency)
- **Preprocessing**: Lowercasing → Tokenization → Stopword Removal → Porter Stemming

---

## 📝 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 🙋‍♂️ Author

**Sumit Kumar** — [@sumitksr](https://github.com/sumitksr)
