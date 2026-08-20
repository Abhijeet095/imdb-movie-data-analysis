# IMDb Movies Data Analysis

An exploratory data analysis (EDA) project using a dataset of 10,000 IMDb movies.

## Project Overview

This project analyzes movie ratings, genres, release trends, Metascores, popularity, duration, directors, and certificates to identify patterns and relationships in the dataset.

The project follows a practical data-analysis workflow:

**Understand → Clean → Analyze → Visualize → Interpret**

## Objectives

- Understand the structure and quality of the IMDb movie dataset
- Clean relevant numerical and categorical fields
- Analyze the distribution of IMDb ratings
- Explore movie genres and their average ratings
- Analyze movie release trends over time
- Examine the relationship between IMDb ratings and Metascores
- Investigate the relationship between ratings and movie popularity
- Analyze movie duration in relation to IMDb ratings
- Compare directors based on average ratings
- Explore certificate categories and ratings

## Dataset

The dataset contains **10,000 movies** and **15 columns**, including:

- Title
- Year
- Certificate
- Duration (min)
- Genre
- Rating
- Metascore
- Director
- Cast
- Votes
- Description
- Review Count
- Review Title
- Review
- Poster

## Data Cleaning

The project handles important data-quality issues, including:

- Converting `Votes` from text containing commas into numeric values
- Converting numerical columns to appropriate numeric data types
- Handling missing certificate values using `Unknown`
- Retaining missing values where imputing them could introduce unsupported assumptions
- Creating filtered datasets for analyses that require specific fields

## Analysis Performed

### 1. IMDb Rating Distribution
Examines the overall distribution, average, median, minimum, and maximum IMDb ratings.

### 2. Genre Analysis
Analyzes common genre combinations and individual genres, including average ratings by genre.

### 3. Movie Release Trends
Examines the number of movies released by year and changes in average IMDb ratings over time.

### 4. IMDb Rating vs Metascore
Measures the relationship between IMDb user ratings and Metascore ratings using correlation and visualization.

### 5. IMDb Rating vs Number of Votes
Uses the number of IMDb votes as a rough indicator of popularity and examines its relationship with rating.

### 6. Movie Duration vs IMDb Rating
Investigates whether movie runtime is associated with IMDb rating.

### 7. Director Analysis
Compares directors using average ratings while requiring a minimum number of movies for more reliable comparisons.

### 8. Certificate Analysis
Examines certificate distribution and average IMDb ratings across certificate categories.

## Key Findings

- The average IMDb rating is approximately **6.44**, with a median of **6.50**.
- **Drama** is the most common individual genre in the dataset.
- Among genres with at least 10 movies, **Film-Noir** has the highest average IMDb rating in this dataset.
- IMDb Rating and Metascore show a **strong positive association** (correlation ≈ **0.73**).
- IMDb Rating and number of Votes show a **moderate positive association** (correlation ≈ **0.37**).
- IMDb Rating and movie Duration show a **moderate positive association** (correlation ≈ **0.36**).
- Among directors with at least three movies, **Charles Chaplin** has the highest average rating in this dataset.

These relationships represent **associations, not causation**.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Project Structure

```text
imdb-movie-data-analysis/
│
├── imdb_movie_analysis.ipynb
├── imdb-movies-dataset.csv
├── README.md
├── requirements.txt
└── .gitignore
```

## How to Run

1. Clone or download this repository.
2. Make sure Python is installed.
3. Install the dependencies:

```bash
pip install -r requirements.txt
```

4. Open the notebook:

```bash
jupyter notebook imdb_movie_analysis.ipynb
```

5. Run the notebook cells from top to bottom.

## Conclusion

This project demonstrates a complete exploratory data-analysis workflow using Python: understanding the dataset, cleaning relevant fields, analyzing relationships, visualizing patterns, and communicating data-driven findings.
