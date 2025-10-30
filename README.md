Social Media Analyzer (Instagram)

Technologies: Python · Jupyter Notebook · NumPy · Pandas · Matplotlib/Seaborn · (optional: scikit-learn, transformers)  
Author: Hrishikesh Shinde

Project overview
Social Media Analyzer is a project to extract, analyze, and visualize trends and user sentiment from Instagram-like social media data. The project demonstrates data ingestion, cleaning, exploratory data analysis (EDA), sentiment analysis using NLP (including GPT-assisted insight generation), and visualization in Jupyter notebooks.

This repository contains notebooks, modular Python code, and scripts to reproduce the analysis.

Features
- Data ingestion and cleaning utilities
- Exploratory data analysis with visualizations
- Sentiment analysis and topic insights
- Modular code (ingest, preprocess, analyze, visualize)
- Example Jupyter notebooks that walk through the full workflow

Repository structure
(See top-level README for full tree) — notebooks for interactive analysis are under `/notebooks`, reusable Python modules are in `/src`, and small sample datasets under `/data`.

Some Main Prompt while making these project are listed as follows
A. Project Setup & Structure
Prompt 1:
“Generate a complete Python project structure for a Social Media Analyzer that collects tweets using Tweepy, performs sentiment analysis with TextBlob, and visualizes data with Matplotlib.”
Prompt 2:
“Write a requirements.txt file for a Python project that uses pandas, numpy, tweepy, textblob, matplotlib, and streamlit.”
Prompt 3:
“Create a Streamlit-based dashboard layout for displaying social media analysis — include tabs for sentiment summary, trending hashtags, and engagement graphs.”

🌐 B. Data Collection (APIs / Scraping)
Prompt 4:
“Write Python code to fetch tweets containing a given hashtag using Tweepy and save them into a CSV file with columns: username, tweet_text, date, likes, retweets.”
Prompt 5:
“Generate a function using snscrape that collects recent posts about a keyword from Twitter and returns a pandas DataFrame.”
Prompt 6:
“Create a reusable Python module for fetching social media data from multiple sources (Twitter, Reddit, Instagram) and standardizing it into a unified format.”

🧠 C. Sentiment & Text Analysis
Prompt 7:
“Write a Python function that performs sentiment analysis using TextBlob and classifies tweets as Positive, Negative, or Neutral.”
Prompt 8:
“Implement sentiment analysis using a pre-trained Hugging Face transformer model for better accuracy and compare results with TextBlob.”
Prompt 9:
“Generate a word cloud visualization from collected tweets to highlight frequently used words.”

📈 D. Visualization & Reporting
Prompt 10:
“Create Python code that visualizes the sentiment distribution of tweets using Matplotlib or Plotly pie charts.”
Prompt 11:
“Generate a bar chart showing the top 10 hashtags used in the dataset using Seaborn.”
Prompt 12:
“Build a Streamlit page that dynamically updates charts when the user enters a new keyword or hashtag.”
Prompt 13:
“Write code to export sentiment analysis results into a PDF report using ReportLab or FPDF.”

⚙️ E. Advanced & Machine Learning Features
Prompt 14:
“Implement a machine learning model (Logistic Regression or Naive Bayes) to predict sentiment labels from tweet text using scikit-learn.”
Prompt 15:
“Create a time series visualization showing how sentiment about a topic changes over time.”

“Integrate keyword extraction and topic modeling (using spaCy or gensim) to identify trending themes in tweets.”

💬 F. Documentation & Deployment
Prompt 17:
“Generate a professional README.md for the Social Media Analyzer project including setup instructions, features, and screenshots.”
Prompt 18:
“Write a Dockerfile to containerize the Social Media Analyzer app with Python dependencies.”
Prompt 19:
“Prepare a short GitHub description and commit messages for uploading the Social Media Analyzer project.”
Prompt 20:
“Write Streamlit deployment instructions for hosting the Social Media Analyzer on Streamlit Cloud.”

Quick start
1. Clone the repo:
```bash
git clone https://github.com/<your-username>/social-media-analyzer-instagram.git
cd social-media-analyzer-instagram

2. Create environment and install dependencies:
python -m venv venv
source venv/bin/activate     # macOS/Linux
venv\Scripts\activate        # Windows
pip install -r requirements.txt

3. Open notebooks:
jupyter notebook notebooks/01_data_ingest_and_cleaning.ipynb

Usage
Add your dataset to data/ (or update the path in notebooks/ and src/ingest.py).
Run the notebooks in order:
01_data_ingest_and_cleaning.ipynb — load and clean data
02_eda_visualizations.ipynb — charts and patterns
03_sentiment_analysis_and_insights.ipynb — sentiment + GPT-assisted insights
Data

Place your data in data/. A sample schema:
post_id — unique id
user_id — user id or handle
timestamp — post datetime (ISO)
text — caption or comment text
likes — number of likes
comments — number of comments
impressions / reach — (optional)
Privacy note: Do not upload private or personally-identifiable data to GitHub. Remove or anonymize sensitive fields.

Notebooks & Code
notebooks/ — interactive analysis with narrative and figures
src/ — modular functions for ingestion, preprocessing, analysis, visualization
scripts/ — convenience runner to execute analysis steps programmatically

Dependencies
See requirements.txt. Example:
python >= 3.8
pandas, numpy, matplotlib, seaborn, jupyter, scikit-learn, nltk, transformers (optional), openai

git clone https://github.com/<your-username>/social-media-analyzer-instagram.git
cd social-media-analyzer-instagram
