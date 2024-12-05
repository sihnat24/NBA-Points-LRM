# NBA-Points-LRM

This repository contains tools and scripts for building a linear regression model to predict NBA players' points scored in games, based on their performance metrics. The workflow involves data scraping, feature analysis, and dataset preparation. All data is provided by https://www.basketball-reference.com/.

### **1. `BBR_scraper.ipynb`**
- Reads a CSV file with player IDs for an entire NBA season.
- Filters out players who played fewer than 8 minutes in games.
- Scrapes player game logs using Beautiful Soup and stores the data for further analysis.

### **2. `prediction_model_v1.ipynb`**
- Analyzes features to determine their relevance in predicting points scored.
- Implements a linear regression model to predict points scored based on the selected features.

### **3. `pts_scrape_and_combine.ipynb`**
- (To be renamed) Combines game log data with seasonal averages to create custom CSV datasets.
- Allows customization of feature lists to generate CSVs containing only the desired features for modeling.

## Usage
1. Run `BBR_scraper.ipynb` to collect and preprocess the game log data.
2. Use `pts_scrape_and_combine.ipynb` to merge the game log data with seasonal averages and create feature-rich datasets.
3. Analyze and model the data in `prediction_model_v1.ipynb` to predict points scored.

## Requirements
- Python 3.x
- Jupyter Notebook
- Required Python libraries: `beautifulsoup4`, `pandas`, `numpy`, `scikit-learn`, and others listed in `requirements.txt`.

## Future Updates
- Rename `pts_scrape_and_combine.ipynb` for clarity.
- Expand prediction models to include additional machine learning techniques.
- Add visualization tools for feature importance and model performance.
- add `requirements.txt` containing all relevant packages

## Contributions
