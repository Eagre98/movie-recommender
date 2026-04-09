# Movie Recommender System

![Python](https://img.shields.io/badge/Python-3.11-blue)
![Pandas](https://img.shields.io/badge/Pandas-2.0-green)
![NumPy](https://img.shields.io/badge/NumPy-1.24-orange)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

## What this project is
A collaborative filtering recommendation engine. Type any movie title
and get 5 similar movies — based purely on rating patterns from real users,
no genre tags or descriptions needed.

## How it works
1. Load 100,836 ratings from 610 users across 9,742 movies
2. Build a user-item matrix — rows are users, columns are movies
3. Calculate Pearson correlation between every pair of movies
4. Return the top 5 most correlated movies for any input title

## Example results

**Input:** Toy Story (1995)
- Toy Story 2 (1999) — similarity: 0.70
- The Incredibles (2004) — similarity: 0.64
- Finding Nemo (2003) — similarity: 0.62

**Input:** Pulp Fiction (1994)
- Fight Club (1999) — similarity: 0.54
- Kill Bill: Vol. 1 (2003) — similarity: 0.50
- True Romance (1993) — similarity: 0.48

## What I learned
- Merging multiple datasets with Pandas
- Building user-item matrices with pivot_table
- Pearson correlation for similarity measurement
- Writing reusable Python functions
- How collaborative filtering works mathematically

## Tools used
| Tool | Purpose |
|------|---------|
| Python | Main language |
| Pandas | Data manipulation and pivot tables |
| NumPy | Numerical operations |
| Google Colab | Development environment |

## Dataset
[MovieLens Small Dataset](https://grouplens.org/datasets/movielens/)
— 100,836 ratings · 9,742 movies · 610 users

## How to run
1. Download MovieLens small dataset from grouplens.org
2. Upload movies.csv and ratings.csv to Google Colab
3. Open movie-recommender.ipynb and run all cells
4. Call recommend('Movie Title (Year)') with any movie
