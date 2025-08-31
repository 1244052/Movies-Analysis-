# Movies-Analysis-
# Re-run after environment reset to regenerate README.md file
readme_content = """
#  Microsoft Movie Studio Analysis

##  Overview
Microsoft is entering the competitive movie industry and needs to understand what kinds of films are most likely to succeed. This project uses data from IMDB and Box Office Mojo to analyze trends in genre, ratings, runtime, and box office performance to help Microsoft make informed decisions about film production.

## Business Understanding
The movie industry is highly competitive, with success often depending on genre selection, audience ratings, and timing. By using data to understand patterns in successful films, Microsoft can position its new studio to create commercially viable content.

##  Problem Statement
- What types of movies perform best at the box office?
- Which genres are most popular with audiences?
- How do runtime, release year, and audience ratings affect a movie’s success?
- What genres consistently generate the highest average box office revenue?

##  Objectives
- Identify film characteristics associated with higher box office revenue.
- Determine popular genres and how ratings impact success.
- Analyze how runtime and release year relate to financial performance.

## Data Sources
- `imdb.title.basics.csv.gz` – Title, genres, year, runtime.
- `imdb.title.ratings.csv.gz` – IMDB average rating and vote count.
- `bom.movie_gross.csv` – Domestic gross revenue.

##  Data Cleaning
- Removed missing values, duplicates, and extreme outliers.
- Merged IMDB and Box Office Mojo datasets.
- Converted data types and engineered new features (e.g., decade, genre count).
- Filtered movies with fewer than 1000 votes to ensure rating validity.

##  Exploratory Data Analysis
- **IMDB Ratings**: Most films have moderate scores (5.5–7.5). Few exceed 8.0.
- **Domestic Gross**: Skewed right; most movies earn under $100M.
- **Runtime**: Successful runtimes range from 90–130 minutes.
- **Genre Revenue**: Action, Adventure, and Sci-Fi have highest average gross.
- **Ratings vs Gross**: Higher ratings loosely correlate with higher revenue.

## Conclusions
- Action, Adventure, and Sci-Fi films consistently generate the highest box office returns.
- Higher audience ratings often lead to better financial performance.
- The optimal runtime for commercial success is between 90–130 minutes.

##  Recommendations
- Produce films in the Action, Adventure, and Sci-Fi genres.
- Target PG-13-rated content to maximize audience reach.
- Use audience ratings and early feedback to guide production.
- Avoid films that are very short or overly long.

##  Files Included
- `Microsoft_Movies_Analysis (1).ipynb`: Full project notebook (Colab)
- `presentation.pdf`: Non-technical stakeholder presentation (final slides)

## Author
Michelle Wangari Joan – Flatiron School, Phase 1 Project
"""

readme_path = "/mnt/data/README.md"
with open(readme_path, "w") as f:
    f.write(readme_content)

readme_path
