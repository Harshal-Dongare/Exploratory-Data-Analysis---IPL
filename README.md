# Exploratory Data Analysis - IPL

## Project Overview

**IPLSync Analytics** is a Python-based exploratory data analysis (EDA) project focused on the Indian Premier League (IPL) cricket dataset. Conducted in a Jupyter Notebook (`Harshal-Dongare-eda-project.ipynb`), it analyzes match and ball-by-ball data to uncover insights into team performance and key metrics, such as the number of sixes hit per season. Leveraging Pandas, NumPy, Seaborn, and Matplotlib, the project delivers statistical summaries and visualizations, showcasing proficiency in data manipulation and sports analytics.

## Dataset Description

The project uses two CSV files:
- **`matches.csv`** (756 rows, 18 columns):
  - Contains match-level data, including `id`, `season`, `city`, `date`, `team1`, `team2`, `toss_winner`, `toss_decision`, `result`, `winner`, `win_by_runs`, `win_by_wickets`, `player_of_match`, `venue`, and umpire details.
  - Covers IPL seasons with details on match outcomes and conditions.
- **`deliveries.csv`** (179,078 rows, 21 columns):
  - Provides ball-by-ball data, including `match_id`, `inning`, `batting_team`, `bowling_team`, `over`, `ball`, `batsman`, `non_striker`, `bowler`, `batsman_runs`, `extra_runs`, `total_runs`, `player_dismissed`, and `dismissal_kind`.
  - Captures detailed in-game actions for performance analysis.

## Project Structure

The analysis is contained in a single Jupyter Notebook:
- **`Harshal-Dongare-eda-project.ipynb`**:
  - **Imports**: Loads required libraries (Pandas, NumPy, Seaborn, Matplotlib).
  - **Data Loading**: Reads `matches.csv` and `deliveries.csv` for analysis.
  - **EDA**: Explores dataset structures and metadata (e.g., column types, non-null counts).
  - **Analysis**: Calculates metrics like the number of sixes per season, merging `deliveries` with `matches` for season context.
  - **Visualization**: Generates a bar plot of sixes per season using Seaborn.

## Key Insights

- **Dataset Scope**: Covers IPL match and ball-by-ball data, enabling detailed performance analysis.
- **Sixes Analysis**: Identifies the number of sixes hit per season, visualized to highlight trends across years.
- **Data Quality**: Notes missing values in columns like `umpire3` (matches) and `player_dismissed` (deliveries), guiding future cleaning efforts.

## Conclusions

The **IPLSync Analytics** project reveals that the IPL dataset, comprising match-level data from `matches.csv` (756 matches across multiple seasons) and ball-by-ball data from `deliveries.csv` (179,078 records), provides a rich foundation for cricket performance analysis, with key metrics such as the number of sixes hit per season highlighting batting trends over time; the dataset’s structure, with detailed columns like `batsman_runs`, `dismissal_kind`, and `season`, enables granular insights into match dynamics, though missing values in columns like `umpire3` (637 nulls in `matches.csv`) and `player_dismissed` (170,244 nulls in `deliveries.csv`) suggest opportunities for data cleaning to enhance analysis accuracy; the visualization of sixes per season underscores varying batting aggression across IPL seasons, offering a starting point for deeper exploration of team and player performance metrics.

## How to Use

### Setup
- **Requirements**: Python 3.12, Jupyter Notebook, Pandas, NumPy, Seaborn, Matplotlib.
- Install dependencies:
  ```bash
  pip install pandas numpy seaborn matplotlib
- Place matches.csv and deliveries.csv in the project directory or update file paths in the notebook.

### Execution
- Open Harshal-Dongare-eda-project.ipynb in Jupyter Notebook or JupyterLab.
- Run all cells to load data, perform analysis, and generate visualizations.
- Outputs include printed metrics (e.g., sixes per season) and a bar plot.

### Execution
- Open Harshal-Dongare-eda-project.ipynb in Jupyter Notebook or JupyterLab.
- Run all cells to load data, perform analysis, and generate visualizations.
- Outputs include printed metrics (e.g., sixes per season) and a bar plot.

### Dependencies
- Python Libraries: Pandas, NumPy, Seaborn, Matplotlib.
- Tools: Jupyter Notebook or JupyterLab.
- Datasets: matches.csv, deliveries.csv (not included in repository; source externally or update paths).

### Conclusion
IPLSync Analytics demonstrates Python-based EDA skills through analysis and visualization of IPL cricket data. The project provides a foundation for deeper sports analytics, with potential for expanded metrics and interactive reporting.
