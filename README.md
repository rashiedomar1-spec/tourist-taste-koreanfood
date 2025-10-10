# 🍽️ Tourist Taste — Text Analytics on Korean Food

What do people say about **Korean food** online?  
This project analyzes discussions (e.g., Reddit) to surface popular **dishes, ingredients, and themes** using text preprocessing, simple visuals, and topic modeling.

> ✅ This repo contains: ready-to-view HTML exports of the notebooks, the raw & processed CSVs, and final visualizations (word cloud, LDA).

---

## 📂 Repository Structure

**CSV Files/**
- `korean_food_subreddit_raw.csv` - Raw scraped data
- `korean_food_subreddit_processed.csv` - Cleaned data

**Codes/**
- `analyzing_visualization.html` - Analysis and visualization notebook
- `preprocessing_step.html` - Data preprocessing notebook
- `reddit_crowling.html` - Reddit scraping notebook

**Results_including_PPT/**
- `A Tourist's Taste. O M A R M2024773.pdf` - Final report
- `lda_visualization_reddit_food_FINALL.html` - Interactive LDA visualization
- `output.png` - Bar/summary plot
- `Word cloud Output.png` - Word cloud visualization

> The original notebooks were exported to **HTML** so you can read the full workflow without setting up Python.

---

## 🔎 What’s inside

- **Data**  
  - `CSV Files/korean_food_subreddit_raw.csv` – combined text (titles, body, comments).  
  - `CSV Files/korean_food_subreddit_processed.csv` – cleaned/lemmatized tokens.

- **Process (see `Codes/*.html`)**  
  1) Cleaning: lowercase, remove URLs/punct/nums → tokenize → POS-filter (nouns/adjectives) → lemmatize → remove stopwords.  
  2) Exploration: frequency tables & **word cloud**.  
  3) Topics: **LDA** to group themes (dishes, ingredients, cooking, dining experience).

- **Results (see `Results_including_PPT/`)**  
  - `Word cloud Output.png` — high-frequency terms.  
  - `lda_visualization_reddit_food_FINAL.html` — interactive topic viz.  
  - `output.png` — summary plot.  
  - PDF report.

---
## 🧭 How to view quickly

You don’t need any environment to read the workflow:

- Double-click the HTML files in **Codes/** to read each step.  
- Open `Results_including_PPT/lda_visualization_reddit_food_FINAL.html` for the interactive topics.  
- View the word cloud (`Results_including_PPT/Word cloud Output.png`) and other figures.

---
## 🛠️ (Optional) Re-run with Python

If you want to reproduce the pipeline, set up a Python env (e.g., 3.10+) and install typical NLP libs:
pandas
numpy
nltk
scikit-learn
gensim
wordcloud
matplotlib
tqdm
Steps (high level):
1. Load `korean_food_subreddit_raw.csv`.  
2. Clean & lemmatize → export `korean_food_subreddit_processed.csv`.  
3. Generate word cloud / frequency plots.  
4. Fit LDA on processed tokens → export interactive HTML viz.

> The runnable notebooks can be added later; current repo prioritizes **readable outputs**.

---

## 📌 Notes
- Filenames with spaces are kept as-is (for traceability). You can rename them for cleaner links.
- Data is a snapshot and reflects the platforms & timeframe collected.

---

## 👤 Author
**Abdirashid Omar**  
GitHub: https://github.com/rashiedomar

Email: rashiidmatan@gmail.com
