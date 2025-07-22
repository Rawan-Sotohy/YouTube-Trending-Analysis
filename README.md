<img src="https://www.seotoolswep.com/components/storage/app/public/photos/1/youtube-trend.webp" width="100%" height="400" />


# 📊 YouTube Trending Videos Analysis - USA 🇺🇸


## 🔍 Project Overview
This notebook presents a comprehensive analysis of YouTube trending videos in the United States using the `USvideos.csv` dataset from Kaggle. The main goal is to uncover patterns behind viral content and identify actionable insights for content creators and marketers.

---

## 📦 Dataset
- **Source:** Kaggle (`USvideos.csv`)
- **Size:** ~40,000+ trending video entries
- **Period Covered:** Mostly from 2017–2018
- **Category Mapping:** Used external JSON file (`US_category_id.json`) to decode category IDs

---

## 🧱 Project Stages

### 1. Data Loading & Exploration
- Previewed data, checked datatypes, missing values
- Converted `publish_time` & `trending_date` to datetime

### 2. Data Cleaning
- Removed duplicates
- Handled missing descriptions
- Mapped category IDs to readable names

### 3.  Feature Engineering
- Created new columns: `like_ratio`, `comment_ratio`, `engagement_score`, `num_tags`, `title_length`
- Extracted temporal features: `publish_hour`, `publish_day`, `publish_month`

### 4.Text Preprocessing
- Cleaned video titles: lowercasing, removing punctuation, numbers, stopwords, and lemmatization
- Created `title_length` as numeric feature

### 5. Sentiment Analysis
- Used `TextBlob` to compute polarity scores for titles
- Labeled sentiment as Positive / Neutral / Negative

### 6. Exploratory Data Analysis (EDA)
- Distribution of views, likes, comments
- Top performing categories and channels
- Publishing hour/day analysis
- Correlation heatmaps between engagement features

### 7. Preparing for Power BI
- Selected key columns and exported a clean CSV
- Ready for dashboarding and storytelling

---

## 💡 Final Insights

- **Friday and Sunday** are the best days to publish videos based on average views.
- **Certain channels dominate** both by volume and total views, e.g. *ChildishGambinoVEVO*.
- **Category "Entertainment"** and **"Music"** have the highest engagement.
- **Longer titles or more tags don’t always equal higher views**, but moderate length seems effective.
- **Positive sentiments** are more common in top-viewed video titles.

---

## Author
**Prepared by:** Rawan Sotohy  
**Project:** Summer Internship @ National Telecommunication Institute (NTI)  
**Track:** Data Analysis & Visualization  
