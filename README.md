#  MarketGap Miner

**AI-driven analytics system to identify unmet market needs from customer reviews**

MarketGap Miner is an end-to-end NLP and analytics project that transforms unstructured customer reviews into actionable business insights. It helps companies detect high-impact product gaps by combining sentiment analysis, topic modeling, and strategic scoring.

---

##  Problem Statement

Companies receive thousands of customer reviews, but:

- Feedback is unstructured and difficult to analyze  
- Critical pain points are hidden in large volumes of text  
- Product teams struggle to prioritize improvements  
- Strategic opportunities are often missed  

**MarketGap Miner automates this process and highlights where the biggest opportunities lie.**

---

##  Solution Overview

This system:

- Ingests customer reviews from CSV files  
- Cleans and processes text using NLP  
- Performs sentiment analysis to detect negative feedback  
- Clusters complaints using topic modeling  
- Ranks opportunities using a Market Gap Score  
- Displays insights through an interactive Streamlit dashboard  

---

##  Methodology

### 1️⃣ Data Ingestion
Customer reviews are loaded from structured CSV files.

### 2️⃣ Text Pre-processing
- Lowercasing  
- Stopword removal  
- Lemmatization using spaCy  

### 3️⃣ Sentiment Analysis
- VADER sentiment analyzer  
- Focus on negative sentiment to capture customer pain points  

### 4️⃣ Topic Modeling
- BERTopic for semantic clustering of reviews  
- Groups similar complaints into meaningful themes  

### 5️⃣ Market Gap Scoring

Each topic is ranked using:

Gap Score = Frequency × Sentiment Severity × Competitor Spread

This ensures issues that are frequent, severe, and widespread are prioritised.

### 6️⃣ Visualization
- Interactive Streamlit dashboard  
- Bar charts of top market gaps  
- Table view of customer pain points  

---

##  Dashboard

The Streamlit dashboard allows decision-makers to:

- View top unmet market needs  
- Explore customer complaints  
- Support data-driven product decisions  

---

##  Tech Stack

- **Language:** Python  
- **Data Processing:** Pandas, NumPy  
- **NLP:** spaCy, NLTK  
- **Sentiment Analysis:** VADER  
- **Topic Modeling:** BERTopic  
- **Visualization:** Streamlit, Plotly  

---

##  Project Structure

MarketGap-Miner/
│
├── app/
│ └── app.py # Streamlit dashboard
│
├── data/
│ ├── gap_scores.csv # Market gap rankings
│ ├── pain_reviews.csv # Negative reviews
│ └── cleaned_master_reviews.csv
│
├── notebooks/
│ └── market_gap_analysis.ipynb # Full analysis workflow
│
├── README.md
├── requirements.txt
└── LICENSE

---

## ▶️ How to Run Locally

 1️⃣ Clone the repository
```bash
git clone https://github.com/jeevanshankar001/MarketGap-Miner.git
cd MarketGap-Miner

2️⃣ Install dependencies
pip install -r requirements.txt

3️⃣Run the Streamlit app
streamlit run app/app.py

## 📈 Outputs

- Ranked list of high-impact market opportunities  
- Clustered customer pain points  
- Interactive dashboard for decision-makers  

---

## 🔮 Future Enhancements

- Use real-world datasets (G2, Trustpilot, Amazon)  
- Add LLM-based review summarisation  
- Implement time-series analysis for emerging trends  
- Enable industry-specific market gap detection  

---

## 🎓 Use Cases

- Product strategy & roadmap planning  
- Business intelligence & analytics  
- Entrepreneurship & innovation research  
- Data Science & MBA portfolio projects  

---

## 👤 Author

**Jeevan**  
MBA (Entrepreneurship) | BSc (Hons) Data Science & Analytics  
