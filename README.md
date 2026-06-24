# 🎬 Netflix Titles EDA Analysis

**Tools used:** Python | Pandas | Matplotlib  

---

## 📌 Short Description

This project performs Exploratory Data Analysis on the Netflix Titles dataset from Kaggle. The goal was to go beyond just loading the data — I wanted to understand what kind of content Netflix actually has, which countries dominate, how content has grown over the years, and what the rating distribution looks like. This analysis is for anyone learning Python EDA or curious about how Netflix's content library is structured.

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| 🐍 Python | Core programming language for the analysis |
| 🐼 Pandas | Data loading, cleaning, and transformation |
| 📊 Matplotlib | Building all visualizations and charts |
| 📓 Jupyter Notebook | Interactive environment for writing and running the analysis |
| 📁 File Format | `.ipynb` for the notebook, `.png` for chart exports |

---

## 📁 Data Source

**Source:** [Kaggle — Netflix Movies and TV Shows](https://www.kaggle.com/datasets/shivamb/netflix-shows)

The dataset contains Netflix titles with the following key columns:
- `type` — Movie or TV Show
- `title` — Name of the content
- `country` — Country where the content was produced
- `release_year` — Year the title was released
- `rating` — Content rating (TV-MA, TV-14, PG-13, etc.)
- `duration` — Runtime in minutes (Movies) or number of seasons (TV Shows)

---

## 🔍 Features / Highlights

### 🔴 Business Problem

Netflix has thousands of titles across movies and TV shows. But just having the data does not tell you anything useful. I wanted to answer a few real questions:

- Is Netflix more of a movie platform or a TV show platform?
- Which countries are producing the most content?
- How has Netflix's content library grown over the years?
- What ratings dominate — is it mostly adult content or family-friendly?
- How long are most movies on Netflix?

---

### 🎯 Goal of the Analysis

To use Python and Matplotlib to explore the Netflix dataset and find patterns that are not visible just by looking at raw data. The focus was on cleaning the data properly first, then letting the visuals tell the story.

---

### 📊 Walkthrough of Key Visuals

**1. Movies vs TV Shows (Bar Chart)**
Compared the count of Movies vs TV Shows across the entire dataset. This was the first and most basic question — what does Netflix mostly have?

**2. Content Rating Distribution (Bar Chart)**
Plotted all content ratings by frequency. Wanted to see whether Netflix leans toward adult audiences or has a balanced mix across age groups.

**3. Movie Duration Distribution (Histogram)**
Filtered only movies, extracted the numeric duration, and plotted a histogram with 30 bins. This shows the typical runtime range most Netflix movies fall in.

**4. Titles Release Year Trend (Line Chart)**
Plotted how many titles were released each year across the full dataset. Shows when Netflix's content library started growing aggressively.

**5. Top 10 Countries by Number of Titles (Horizontal Bar Chart)**
Ranked the top 10 content-producing countries. Sorted before plotting so the chart is easier to read at a glance.

**6. Movies vs TV Shows — Year-wise Trend (Dual Line Chart)**
Grouped data by release year and type, then plotted both on the same chart. This shows whether Netflix has been investing more in movies or TV shows over time.

---

### 💡 Business Impact and Insights

- **Movies dominate** — Netflix has significantly more movies than TV shows in this dataset
- **USA leads by a large margin** — it produces far more content than any other country on the platform
- **Content growth spiked in the mid-2010s** — Netflix's aggressive original content push is clearly visible in the release year trend
- **TV-MA is the most common rating** — Netflix skews toward adult content, not family-friendly
- **Most movies are between 80 and 120 minutes** — the typical feature film length, no surprises there
- **TV Shows have been growing faster recently** — the year-wise trend shows TV Show production catching up to Movies in recent years

---
---

## 📂 Project Structure

```

├── Netflix_Analysis.ipynb       ← Main analysis notebook
├── netflix_titles.csv           ← Raw dataset from Kaggle
├── Charts/
│   ├── movies_vs_tvshows.png
│   ├── rating_distribution.png
│   ├── movie_duration_histogram.png
│   ├── release_year_trend.png
│   ├── top10_countries.png
│   └── yearly_type_trend.png
└── README.md
```

---

## 💡 What I Learned

- How to clean real-world messy data using Pandas — dropping nulls on specific columns instead of the whole dataset
- Extracting numeric values from string columns (like converting "90 min" to 90)
- Building different chart types in Matplotlib — bar, histogram, line, horizontal bar
- Grouping data with `groupby` and `unstack` to compare two categories over time
- Saving charts as `.png` files using `savefig`

---

## 🙋 Connect with Me

This is part of my ongoing data analytics learning journey. If you have feedback on the analysis or the code, I'd genuinely like to hear it.

- 🔗 LinkedIn: [linkedin.com/in/tarun-kumar-5b9280396](https://linkedin.com/in/tarun-kumar-5b9280396)
- 💻 GitHub: [github.com/tarunkumar7906](https://github.com/tarunkumar7906)

---

*Still learning. Open to feedback.*
