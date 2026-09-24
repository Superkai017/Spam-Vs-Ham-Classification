# Spam vs Ham Classifier

A machine learning project that classifies text messages/emails as **spam** or **ham** (legitimate) using natural language processing and classical machine learning algorithms.

## 📋 Overview

This project builds a binary text classification pipeline that preprocesses raw message text and predicts whether a message is spam or ham, using classical ML algorithms trained on labeled data.

## ✨ Features

- Text preprocessing (lowercasing, punctuation removal, tokenization, stopword removal, stemming/lemmatization)
- Feature extraction using **Bag of Words** / **TF-IDF**
- Model training with **Naive Bayes**, **Logistic Regression**, and **SVM**
- Model comparison and selection based on performance metrics
- Model evaluation (accuracy, precision, recall, F1-score, confusion matrix)
- (Optional) Deployment via Flask/Streamlit for live predictions

## 🛠️ Tech Stack

- Python 3.x
- scikit-learn
- pandas / numpy
- NLTK
- matplotlib / seaborn

## 📂 Project Structure

```
spam-vs-ham-classifier/
│
├── data/
│   └── spam.csv
├── notebooks/
│   └── spam_ham_classification.ipynb
├── src/
│   ├── preprocessing.py
│   ├── train.py
│   └── predict.py
├── models/
│   └── best_model.pkl
├── requirements.txt
└── README.md
```

## 📊 Dataset

Trained on the [SMS Spam Collection Dataset](https://archive.ics.uci.edu/dataset/228/sms+spam+collection), containing labeled SMS messages as spam or ham.

## ⚙️ Installation

```bash
git clone https://github.com/yourusername/spam-vs-ham-classifier.git
cd spam-vs-ham-classifier
pip install -r requirements.txt
```

## 🚀 Usage

**Train the model:**
```bash
python src/train.py
```

**Make a prediction:**
```bash
python src/predict.py --text "Congratulations! You've won a free prize, click here"
```

## 🔎 Methodology

1. **Data Cleaning** — remove null values, duplicates, and irrelevant columns
2. **Text Preprocessing** — lowercase, remove punctuation/numbers, tokenize, remove stopwords, apply stemming/lemmatization
3. **Feature Extraction** — convert text to numerical vectors using TF-IDF
4. **Model Training** — train and compare Naive Bayes, Logistic Regression, and SVM
5. **Evaluation** — assess models using accuracy, precision, recall, and F1-score

## 📈 Results

| Model | Accuracy | Precision | Recall | F1-Score |
|-------|----------|-----------|--------|----------|
| Naive Bayes | XX% | XX% | XX% | XX% |
| Logistic Regression | XX% | XX% | XX% | XX% |
| SVM | XX% | XX% | XX% | XX% |

Best performing model: **[Model Name]** with **XX% accuracy**.

## 📌 Future Improvements

- Experiment with deep learning approaches (LSTM, BiLSTM)
- Deploy as a web app for real-time classification
- Expand dataset for better generalization

## 📝 License

This project is licensed under the MIT License.

## 🙋 Author

**[Your Name]**  
[GitHub](https://github.com/yourusername) | [LinkedIn](https://linkedin.com/in/yourusername)
