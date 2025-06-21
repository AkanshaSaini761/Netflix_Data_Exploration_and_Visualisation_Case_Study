# 🎬 Netflix Content Analysis Case Study
## 🏢 About Netflix
**Netflix** is one of the world’s most popular streaming platforms, hosting a vast collection of movies and TV shows. As of mid-2021, it boasts over **222 million global subscribers** and more than **10,000+ titles** across various genres, countries, and languages.

## 📌 Objective

Netflix, a global leader in video streaming, aims to better understand its content landscape across countries and time to make data-driven decisions. This project explores a dataset of over 8,000 titles, providing insights into what content is trending, which genres are growing, and what release strategies work best.

### 🔍 Business Goals

- Identify what type of shows/movies Netflix should produce more of.
- Suggest strategies to grow the platform’s global presence and engagement.
- Analyze viewing trends, genres, sentiments, and release behaviors.

## 📁 Dataset Overview
### 📥 Dataset: [netflix.csv](https://drive.google.com/file/d/1iRmihWqevBA_nEHWhWesVObj9gcA2u0a/view?usp=drive_link)
The dataset includes metadata on Netflix's catalog of Movies and TV Shows.

| Column         | Description                                               |
|----------------|-----------------------------------------------------------|
| `show_id`      | Unique ID for each title                                  |
| `type`         | Whether it's a Movie or a TV Show                         |
| `title`        | Title of the content                                       |
| `director`     | Director(s) of the content                                 |
| `cast`         | Main cast/actors                                           |
| `country`      | Country of origin                                          |
| `date_added`   | Date when content was added to Netflix                    |
| `release_year` | Year of initial release                                    |
| `rating`       | Age-based TV rating (e.g., PG-13, TV-MA)                   |
| `duration`     | Length in minutes or seasons                               |
| `listed_in`    | Genre(s)                                                   |
| `description`  | Content synopsis                                           |

## 🎯 Core Exploratory Goals

- What type of content is available in different countries?
- How has the number of movies/shows released changed over the last 20–30 years?
- Comparison of TV Shows vs. Movies
- What is the best time (week/month) to launch content?
- Who are the most active actors and directors?
- Has Netflix shown a growing preference for TV Shows over time?
- How can sentiment and genre analysis guide future content decisions?

## 📊 Key Analysis

### 1. 🔍 General & Preprocessing
- Dataset contains **8,807 titles** and **12 attributes**.
- Cleaned missing data in `director`, `cast`, `country`, and `date_added`.
- Columns like `cast`, `director`, and `country` were unnested for richer analysis.

### 2. 📊 Categorical Variables Analysis
- Counted and visualized all categorical variables.
- 2 main types: **Movies (~69.7%)** and **TV Shows (~30.3%)**.
- Over **198 countries**, **5121 directors**, and **39261 cast members** involved.

### 3. 🆚 TV Shows vs. Movies
- TV Shows and Movies analyzed by release trends and country of production.
- USA, India, and UK dominate content creation across both types.
- Significant rise in releases post-2010; peak around **2018**.

### 4. 📅 Best Release Time
- **Week 39 and 26** are peak weeks for releasing content.
- **July and December** are the best-performing months across both formats.

### 5. 🎭 Directors & Actors
- Top actors: **Anupam Kher, Shah Rukh Khan, Om Puri**
- Top directors: **Rajiv Chilaka, Martin Scorsese, Jan Suter**
- Suggests a diverse mix of global and regional influence.

### 6. 🎞️ Genre Analysis
- Top genres: **International Movies**, **Dramas**, **Comedies**, **International TV**, **Documentaries**
- WordCloud and year-wise genre popularity trends analyzed.
- Continued growth in International and Drama genres post-2015.

### 7. ⏱️ Time to Add on Netflix
- Median time to add new content after release: **334 days**
- Shorter intervals seen in recent years, indicating faster acquisition strategies.

### 8. 🔢 Rating Distribution
- Top rating: **TV-MA (36.4%)**, followed by **TV-14 (24.5%)**
- Skews toward content for mature audiences.

### 9. 💬 Sentiment Analysis
- Applied `TextBlob` to content descriptions.
- Most titles exhibit **positive sentiment**, followed by neutral, then negative.
- Peak content variety seen in **2018–2019**.

## 💡 Business Recommendations

1. **Diversify Content Portfolio**  
   Increase investment in **International Movies**, **Dramas**, and **Comedies** to appeal to broad audience bases.

2. **Strategic Release Timing**  
   Target **week 39** and **week 26**, and the months **July** and **December**, to optimize content engagement.

3. **Invest in Talent**  
   Leverage global acting and directing talent like **Anupam Kher**, **Martin Scorsese**, etc., to attract international viewers.

4. **Accelerate Content Acquisition**  
   Aim to shorten the **release-to-streaming** timeline below 334 days to maintain relevance.

5. **Target Mature Audiences**  
   Continue producing **TV-MA** content while maintaining a balance with family-friendly options.

6. **Emotionally Engaging Descriptions**  
   Emphasize **positive and engaging content descriptions** to boost initial click-through and retention.

7. **Explore Emerging Genres**  
   Track performance of niche genres like **action-adventure** and **crime thrillers** to identify breakout hits.

## 🛠️ Tools Used

- Python (Pandas, Seaborn, Matplotlib)
- NLTK & TextBlob for Sentiment Analysis
- Jupyter Notebook
- WordCloud, GroupBy, and Pivot for analysis

## 📄 Output Report

All visualizations, analysis code, and insights are documented in the PDF file:
📎 [netflix_case_study_akansha_saini.pdf](https://drive.google.com/file/d/18an1toFPFSjvsCm9jxsu8bkr4D0wuVq9/view?usp=drive_link)
