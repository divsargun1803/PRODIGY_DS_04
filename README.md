# PRODIGY_DS_04 — Twitter Sentiment Analysis

> **Prodigy InfoTech Data Science Internship — Task 4**

Analyze and visualize sentiment patterns in social media data to understand public opinion and attitudes towards specific topics or brands.

---

## 📌 Objective

Perform end-to-end sentiment analysis on Twitter data to:
- Understand the distribution of sentiments (Positive, Negative, Neutral, Irrelevant)
- Identify which brands/entities generate the most positive or negative discussions
- Build a text classification model to predict tweet sentiment
- Extract key insights through rich visualizations

---

## 📦 Dataset

**Source:** [Prodigy InfoTech GitHub](https://github.com/Prodigy-InfoTech/data-science-datasets/tree/main/Task%204)

| Property | Value |
|---|---|
| File | `twitter_training.csv` |
| Rows | ~74,682 tweets |
| Columns | Tweet ID, Entity, Sentiment, Tweet Text |
| Sentiment Labels | Positive, Negative, Neutral, Irrelevant |

---

## 🛠️ Tech Stack

| Category | Tools |
|---|---|
| Language | Python 3 |
| Data Manipulation | pandas, numpy |
| NLP | NLTK (stopwords, lemmatization) |
| Visualization | matplotlib, seaborn, wordcloud |
| Machine Learning | scikit-learn (TF-IDF, Logistic Regression) |

---

## 📊 Analysis Highlights

### EDA & Visualizations
- **Sentiment Distribution** — Bar chart & pie chart of all 4 sentiment classes
- **Top 15 Entities** — Brands/topics with highest tweet volumes
- **Sentiment Breakdown per Entity** — Grouped bar chart for top 10 entities
- **Positivity Ratio** — Which brands attract the most positive tweets
- **Tweet Length Analysis** — Word count distribution and box plots by sentiment
- **Word Clouds** — Most frequent words for Positive, Negative, and Neutral tweets
- **Top Words per Sentiment** — Horizontal bar charts of most frequent terms
- **Sentiment Heatmap** — Entity vs. sentiment percentage matrix

### Machine Learning Model
- **Preprocessing:** URL removal, mention stripping, lemmatization, stopword removal
- **Vectorization:** TF-IDF (10,000 features, unigrams + bigrams)
- **Model:** Logistic Regression (3-class: Positive / Negative / Neutral)
- **Evaluation:** Confusion matrix, precision, recall, F1-score

---

## 🔑 Key Findings

1. **Negative tweets dominate** (~30% of all tweets) — users are more vocal about complaints
2. **Positive tweets** are the second most common (~28%), showing significant brand appreciation
3. **Microsoft, League of Legends, and Verizon** attract the highest tweet volumes
4. **Negative tweets** tend to be slightly longer on average
5. Positive tweets cluster around words like *love, great, amazing*; Negative around *worst, hate, bad*
6. The TF-IDF + Logistic Regression classifier achieves strong accuracy on 3-class sentiment prediction

---

## 📁 Repository Structure

```
PRODIGY_DS_04/
│
├── PRODIGY_DS_04.ipynb       # Main Jupyter Notebook
├── twitter_training.csv      # Dataset
└── README.md                 # Project documentation
```

---

## ▶️ How to Run

```bash
# 1. Clone the repository
git clone https://github.com/<your-username>/PRODIGY_DS_04.git
cd PRODIGY_DS_04

# 2. Install dependencies
pip install pandas numpy matplotlib seaborn wordcloud nltk scikit-learn

# 3. Launch the notebook
jupyter notebook PRODIGY_DS_04.ipynb
```

---

## Author
**Sargun (Divsargun Kaur)** — B.Tech, NIT Jalandhar (Batch 2029)  
[LinkedIn](https://linkedin.com/in/divsargunkaur) · [GitHub](https://github.com/divsargun1803)
