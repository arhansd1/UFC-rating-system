# MMA Fighter Rating System

This project calculates and analyzes MMA fighters' performance over time. Using fight data, it creates a **dynamic record** for each fighter, tracking both their **current** and **peak scores** (highest career score). The project considers opponent quality, win/loss outcomes, and victory methods.

## Project Overview
- Used UFC official website for webscraping all data 
http://ufcstats.com/statistics/fighters
http://ufcstats.com/statistics/events/completed

- **Load Data**: Collects fighter data from a CSV and scrapes additional stats.
- **Calculate Scores**: Adjusts scores based on:
  - **Opponent Quality**: Higher scores for wins over strong opponents.
  - **Victory Method**: Knockouts or submissions score higher than decisions.
  - **Win/Loss History**: Tracks career-high scores and records downward trends.
- **Output**: Saves scores to a CSV file for easy analysis.

## Requirements

- Python 3 and virtual environment setup
- Install dependencies with `pip install -r requirements.txt`

## Instructions to Run

1. **Set Up Environment**:
   - Open terminal in the project folder.
   - Create and activate a virtual environment:
     ```bash
     python3 -m venv myenv
     source myenv/bin/activate
     ```
   - Install dependencies:
     ```bash
     pip install -r requirements.txt
     ```

2. **Run the Code**:
   - Open Jupyter Notebook:
     ```bash
     jupyter notebook
     ```
   - Run `dynamic record.ipynb` and `static record.ipynb` to calculate and export scores.

## Project Files

- **`static_data.csv`**: Base fighter data with quality factors. Final result
- **`dynamic record.ipynb`** & **`static record.ipynb`**: Main scripts to process data and output final scores.
- **`requirements.txt`**: Required Python packages.
