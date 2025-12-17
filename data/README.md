# TweetLLM Data Analysis - Portfolio Deliverables

## Overview
This package contains a complete exploratory data analysis (EDA) of the TweetLLM dataset (305,432 tweets about LLMs from Nov 2022 - Feb 2023).

## Files Included

### 1. TweetLLM_DA.ipynb
Ready-to-run Jupyter notebook with:
- Data loading and preview
- Date/time parsing (Date, UserCreated)
- Numeric coercion (Retweets, Likes, UserFollowers, UserFriends)
- Language detection (langdetect)
- Quality checks (missing values, duplicates)
- EDA counts (by date, language, location)
- Visualizations (volume, word cloud, tweet length, top locations)
- Placeholders for next steps (sentiment, geo normalization, topics)

### 2. Figures (figures/)
High-resolution PNG exports:
- volume.png: Daily tweet volume over time
- wordcloud.png: Word cloud of overall corpus
- tweet_length.png: Distribution of tweet character lengths
- top_locations.png: Top 15 raw location strings

## Dataset Summary
- **Rows:** 305,432 tweets
- **Date range:** 2022-11-30 to 2023-02-24 (~3 months)
- **Languages:** 36 detected; 99.2% English
- **Locations:** 33,739 unique strings; 25% missing
- **Duplicates:** 5 exact duplicates, 30 duplicate URLs, 2,162 duplicate tweet texts

## Tools Used
- pandas: data wrangling
- numpy: numerics
- matplotlib: plotting
- wordcloud: corpus visualization
- langdetect: language inference
- tqdm: progress tracking
- nbformat: notebook generation

## Next Steps (Suggested)
1. Sentiment classification (VADER or transformer-based)
2. Location normalization (country/state/region mapping)
3. Time-series sentiment trends
4. Entity & topic extraction (NER, keyword extraction)
5. Interactive dashboard (Streamlit or Plotly Dash)

## How to Use
1. Ensure TweetLLM.csv is in the same directory
2. Install dependencies: pandas, numpy, matplotlib, wordcloud, langdetect, tqdm
3. Run TweetLLM_DA.ipynb cell-by-cell or all at once
4. Review figures/ for exported visuals


