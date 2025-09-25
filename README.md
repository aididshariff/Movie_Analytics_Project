# Movie Analytics Project

## Overview
This project demonstrates a full **ETL pipeline** using Python, starting from **web scraping** (TMDb HTML), **API enrichment**, **data cleaning**, and **analysis** with **pandas**, followed by **visualization** (matplotlib, seaborn, Tableau), and ending with a **beginner machine learning step**.

The goal is to:
1. Practice Extract → Transform → Load (ETL) workflows.
2. Explore movie trends (genres, release years, runtime).
3. Build visualizations and dashboards for insights.
4. Experiment with basic ML models (cluster movies).

## Setup Instructions
Clone the repository:
git clone https://github.com/aididshariff/Movie_Analytics_Project.git
cd Movie_Analytics_Project

## Create & activate virtual environment
**Windows (PowerShell)**
python -m venv .venv
.venv\Scripts\activate

**macOS / Linux**
python3 -m venv .venv
source .venv/bin/activate

## Install dependencies
pip install -r requirements.txt

## Jupyter Notebook in VS Code
**.** Open the repo in VS Code.
**.** Install the Python and Jupyter extensions.
**.** Start a notebook (e.g., notebooks/01_scraping.ipynb) with the .venv kernel.


## Project Structure
## Project Structure

```text
Movie_Analytics_Project/
├── data/
│   ├── raw/          # Raw scraped data (not pushed to GitHub)
│   └── processed/    # Cleaned & enriched data
├── notebooks/
│   └── 01_scraping.ipynb   # Scraping + API enrichment
├── scripts/
│   ├── clean_data.py       # Data cleaning & transformation
│   ├── analysis.py         # Exploratory analysis
│   ├── visualize.py        # Matplotlib/Seaborn visualizations
│   └── ml_model.py         # Beginner ML model(s)
├── outputs/
│   ├── charts/             # Matplotlib/Seaborn charts
│   └── dashboards/         # Tableau exports or screenshots
├── README.md
└── requirements.txt


## Data
**1** Extraction (Scraping + API)
Scrape: TMDb Top Rated Movies
→ title, release year, rank.
**2** API Enrichment: TMDb API or OMDb API
→ rating, genres, runtime, director, plot.


## Project Idea
Analyze movie data scraped from websites and APIs.

## Tools
- Python (Pandas, requests, BeautifulSoup)
- Tableau

## Goals
1. Scrape movie data using requests + BeautifulSoup.
2. Clean and analyze the data with pandas.
3. Visualize insights using matplotlib, seaborn and Tableau.
4. Try simple ML models for predictions (scikit-learn).

## Transformation
Clean column names.
Handle missing values.
Convert data types (e.g., year → int, rating → float).

## Load
Save cleaned dataset into data/processed/movies_clean.csv.
Optionally load into a SQLite DB for practice.

👉**Note:** Raw data (data/raw/) is not pushed to GitHub.
If you want to recreate it, run:
jupyter notebook notebooks/01_scraping.ipynb
This will scrape the HTML and fetch API details again.

## Analysis & Visualization
Pandas → summary stats, top genres, movies per year.
Matplotlib/Seaborn → bar charts, scatter plots, distributions.
Tableau → interactive dashboard (optional).

## Beginner Machine Learning
Implemented with scikit-learn:
Regression: predict IMDb/TMDb rating based on year, runtime, genre.
Clustering: group movies by features (e.g., runtime, genre, rating).

## How to Run the Project
Run the scraping notebook → generates raw data.
Use cleaning scripts (scripts/clean_data.py) → creates processed dataset.
Perform EDA in scripts/analysis.py or Jupyter.
Generate visualizations with scripts/visualize.py.
Try out ML experiments with scripts/ml_model.py.

## Requirements
Python 3.9+
pandas
matplotlib
seaborn
requests
beautifulsoup4
scikit-learn
jupyter

## Install everything with:
pip install -r requirements.txt

## Notes
Raw data is ignored in GitHub (data/raw/).
You must re-run scraping to rebuild it.
The project is educational and not production-ready.

## Project status
In progress.

## Personal information
Name: **Aidid Alwi**.

Date: Sept 25, 2025.

[email](sharifaidid4@gmail.com)

[Tableau](https://public.tableau.com/app/profile/aidid.alwi)