# 🧠 Mental Health Insights from Reddit

This project analyzes Reddit posts from mental health-related subreddits such as `r/depression` to uncover emotional trends, keyword themes, and shifts in sentiment over time using natural language processing (NLP) techniques. The insights are visualized to help identify patterns in mental distress, positivity, and support-seeking behavior.

---

## 📌 Project Objectives

- 🗣️ Analyze user-generated posts on mental health topics
- 📊 Perform sentiment analysis using VADER
- ⏳ Track emotional trends over time
- 🔍 Identify common keywords and dominant emotional themes
- 🧠 Apply topic modeling to uncover hidden topics in conversations

---

## 🗂️ Dataset

- **Source**: Scraped directly from Reddit using the `PRAW` API
- **Subreddit**: `r/depression` (expandable to others like `r/anxiety`, `r/mentalhealth`)
- **Features Collected**:
  - `title`, `selftext`, `created_utc`
  - `score`, `num_comments`
  - Derived features: `text`, `sentiment_score`, `sentiment_label`, `date`

---

## 🔬 Tools & Technologies

| Purpose                | Stack                                   |
|------------------------|-----------------------------------------|
| Data Collection        | Python, PRAW (Reddit API)               |
| Text Processing        | NLTK, re, pandas                        |
| Sentiment Analysis     | VADER (from nltk.sentiment.vader)       |
| Visualization          | Seaborn, Matplotlib                     |
| Topic Modeling         | Gensim (LDA), spaCy (optional)          |
| Dashboard (optional)   | Power BI or Streamlit                   |

---

## 🧪 NLP Tasks Performed

1. **Preprocessing**:
   - Cleaning text (punctuation, case, stopwords)
   - Combining title and body for full context

2. **Sentiment Analysis**:
   - VADER applied to compute compound score
   - Labeling posts as `Positive`, `Negative`, or `Neutral`

3. **Trend Analysis**:
   - Sentiment scores averaged per day
   - Trends visualized over time to track mental health shifts

4. **Keyword & Topic Mining**:
   - Most common keywords per sentiment label
   - Topic modeling with LDA to discover hidden themes

---

## 📊 Key Visualizations

- 📈 Sentiment trend line (daily)
- 📊 Top emotional keywords per sentiment
- ☁️ Word clouds by label
- 🔥 Topic frequency over time
- 🗓️ Weekly emotional activity heatmap (optional)

---

## 🧠 Insights Uncovered

- Peaks in negative sentiment around weekends and holidays
- Therapy and progress-related posts were generally positive
- Distress-heavy topics like isolation, insomnia, and family conflict dominated negative clusters
- Engagement (comments/upvotes) correlated with emotional depth

---

## 📁 Project Structure

 reddit-mental-health-nlp
├── scraped_data/
│ └── reddit_depression_posts.csv
├── notebooks/
│ ├── sentiment_analysis.ipynb
│ ├── trend_analysis.ipynb
│ └── topic_modeling.ipynb
├── visuals/
│ ├── sentiment_trend.png
│ └── wordcloud_negative.png
├── dashboard/
│ └── streamlit_app.py (optional)
├── README.md
└── requirements.txt

---

## 🚀 How to Run

1. Clone the repository
2. Install dependencies:

---

## 🤝 Contributions

This project is open for:
- Adding more subreddits and posts
- Deeper topic modeling with BERTopic
- Deploying an interactive web app for NGOs or universities

---

## ⚠️ Disclaimer

This project is for **educational and research purposes only**.  
It is **not a substitute for professional mental health care** or clinical tools.

---

## 🧑‍💻 Author

Afan Hafeez
_Data Analyst & NLP Explorer_  
[GitHub](https://github.com/) • [LinkedIn](https://linkedin.com/in/yourprofile)

---

## ⭐️ If you find this project insightful...

Don’t forget to **star** ⭐ it and share!  
Your support helps bring more awareness to mental health through data.

