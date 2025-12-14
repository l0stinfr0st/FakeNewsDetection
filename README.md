# Fake News Detection – EDA & Modeling

This repository contains an end-to-end **fake news detection** project, including exploratory data analysis (EDA), text preprocessing, feature extraction, and machine learning model implementation. The project uses two well-known datasets (**ISOT** and **LIAR**) and follows a clean, reproducible research structure.

---

## 📂 Repository Structure

```
.
├── notebooks/
│   ├── ISOT_EDA.ipynb
│   ├── LIAR_EDA_.ipynb
│   └── Model_Implementation_Notebook.ipynb
│
├── requirements.txt
├── README.md
```

---

## 📊 Datasets

### 1. ISOT Fake News Dataset
- Contains labeled real and fake news articles.
- Features include news **title**, **text**, and **label**.
- Primarily used for binary fake/real classification.

### 2. LIAR Dataset
- Short political statements labeled across multiple truthfulness levels.
- Includes metadata such as speaker, subject, and context.
- Used to analyze linguistic patterns in deceptive statements.

---

## 🔍 Exploratory Data Analysis (EDA)

EDA is performed separately for each dataset:

### ISOT_EDA.ipynb
- Dataset inspection and class distribution
- Text length and word count analysis
- Missing value handling
- Basic text cleaning (lowercasing, punctuation removal)

### LIAR_EDA_.ipynb
- Label distribution analysis
- Statement length statistics
- Cleaning and normalization
- Comparison between truthful vs deceptive statements

---

## 🧠 Feature Extraction

Before modeling, textual data is transformed into numerical representations:

- **TF-IDF Vectorization**
  - Converts cleaned text into weighted term-frequency features
  - Reduces the impact of common but uninformative words

Feature extraction is applied consistently across datasets to ensure fair model comparison.

---

## 🤖 Modeling

Implemented in `Model_Implementation_Notebook.ipynb`:

- Train-test split
- TF-IDF feature matrix construction
- Machine learning classifiers (Decision Trees, and Random Forests)
- Model training and evaluation
- Performance metrics:
  - Accuracy
  - Precision
  - Recall
  - F1-score

The notebook focuses on clarity and reproducibility rather than heavy hyperparameter tuning, but it also uses GridSearchCV for the hyperparameter tuning.

---

## ▶️ Usage

1. **Clone the repository**
```bash
git clone <https://github.com/l0stinfr0st/FakeNewsDetection/>
cd fake-news-detection
```

2. **Install dependencies**
```bash
pip install -r requirements.txt
```

3. **Run notebooks**
```bash
jupyter notebook
```
Open the notebooks in the following order:
1. `ISOT_EDA.ipynb`
2. `LIAR_EDA_.ipynb`
3. `Model_Implementation_Notebook.ipynb`

---

## 📦 requirements.txt (Example)

```
numpy
pandas
matplotlib
seaborn
scikit-learn
nltk
jupyter
```

---

## 🎯 Project Goals

- Understand linguistic differences between fake and real news
- Apply classical NLP feature extraction techniques
- Build and evaluate baseline ML models for fake news detection
- Maintain a clean and reproducible research workflow

---

## 📌 Notes

- All preprocessing and modeling steps are fully documented inside the notebooks.
- The repository is structured to meet academic project and reproducibility requirements.

---

## 👤 Author

Ahmad El Ghazi

