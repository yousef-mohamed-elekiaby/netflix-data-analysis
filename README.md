# Netflix Data Science Project
### Decodelabs Internship

---

## Project Overview
This project analyzes the Netflix Movies and TV Shows dataset.
It covers all 5 Data Science tasks: data collection, cleaning, analysis, visualization, and building a machine learning model.

---

## Dataset
- **Name:** Netflix Movies and TV Shows
- **File:** `netflix_titles.csv`
- **Rows:** 8,807 titles
- **Columns:** 12 columns

| Column | Description |
|--------|-------------|
| show_id | Unique ID for each title |
| type | Movie or TV Show |
| title | Name of the movie or show |
| director | Director name |
| cast | Actors |
| country | Country of production |
| date_added | Date added to Netflix |
| release_year | Year of release |
| rating | Age rating (TV-MA, PG-13, etc.) |
| duration | Length in minutes or seasons |
| listed_in | Genre (Action, Comedy, etc.) |
| description | Short summary |

---

## Tasks

### Task 1: Data Collection & Understanding
- Loaded the dataset using pandas
- Explored the shape, columns, and data types
- Described what each column represents

### Task 2: Data Cleaning & Preprocessing
- Filled missing values in `director`, `cast`, and `country` with `'Unknown'`
- Removed rows with missing `rating`, `duration`, and `date_added`
- Removed duplicate rows
- Extracted `year_added` from `date_added`
- Extracted `duration_mins` from `duration`

### Task 3: Exploratory Data Analysis (EDA)
- Movies (6,126) are more than TV Shows (2,664)
- United States is the top content-producing country
- Most common rating is TV-MA
- 2019 had the highest number of titles added to Netflix
- Average movie length is about 100 minutes

### Task 4: Data Visualization
- Pie chart: Movies vs TV Shows
- Bar chart: Top 10 countries by content
- Line chart: Content added per year
- Histogram: Movie duration distribution
- Bar chart: Content by age rating
- Heatmap: Model confusion matrix

### Task 5: Predictive Model
- **Model:** Logistic Regression
- **Goal:** Predict if content is a Movie or TV Show
- **Features used:** release year, year added, age rating
- **Accuracy:** ~70%

---

## Charts

| Chart | File |
|-------|------|
| Movies vs TV Shows | `chart1_movies_vs_tvshows.png` |
| Top 10 Countries | `chart2_top_countries.png` |
| Content Per Year | `chart3_content_per_year.png` |
| Movie Duration | `chart4_movie_duration.png` |
| Age Rating | `chart5_age_rating.png` |
| Confusion Matrix | `chart6_confusion_matrix.png` |

---

## How to Run
1. Install the required libraries:
```
pip install -r requirements.txt
```
2. Make sure `netflix_titles.csv` is in the same folder as the notebook
3. Open `netflix_beginner.ipynb` in Jupyter or Google Colab
4. Run all cells from top to bottom

---

## Project Structure
```
├── netflix_beginner.ipynb       # Main notebook with all 5 tasks
├── netflix_titles.csv           # Dataset
├── requirements.txt             # Required libraries
├── README.md                    # Project description
├── chart1_movies_vs_tvshows.png
├── chart2_top_countries.png
├── chart3_content_per_year.png
├── chart4_movie_duration.png
├── chart5_age_rating.png
└── chart6_confusion_matrix.png
```
