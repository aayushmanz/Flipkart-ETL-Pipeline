# Flipkart Mobile Data Analysis

This project demonstrates an end-to-end mini data pipeline for **Flipkart 5G mobile listings**:
- Web scraping product details with Selenium
- Cleaning and structuring the raw dataset with Pandas
- Running exploratory data analysis (EDA) to extract insights

## Repository Structure

- `/home/runner/work/Flipkart-Mobile-Data-Analysis/Flipkart-Mobile-Data-Analysis/Web Scrapping ( Selenium )/Web Scrapping From Flipkart.ipynb`  
  Scrapes mobile listing data and exports `flipkart_mobile.csv`.

- `/home/runner/work/Flipkart-Mobile-Data-Analysis/Flipkart-Mobile-Data-Analysis/Web Scrapping ( Selenium )/flipkart_mobile.csv`  
  Raw scraped dataset.

- `/home/runner/work/Flipkart-Mobile-Data-Analysis/Flipkart-Mobile-Data-Analysis/Data Cleaning ( Pandas )/Data Cleaning From Flipkart DataSet.ipynb`  
  Cleans and transforms raw data into analysis-ready features.

- `/home/runner/work/Flipkart-Mobile-Data-Analysis/Flipkart-Mobile-Data-Analysis/Data Cleaning ( Pandas )/Flipkart_cleaned_dataset.csv`  
  Cleaned dataset used for analysis.

- `/home/runner/work/Flipkart-Mobile-Data-Analysis/Flipkart-Mobile-Data-Analysis/Exploratory Data Analysis ( EDA )/EDA on Flipkart DataSet.ipynb`  
  Performs EDA and visualization on the cleaned dataset.

## Data Pipeline

1. Run the scraping notebook to collect product data from Flipkart.
2. Run the data cleaning notebook to parse product attributes (brand, storage, RAM, battery, etc.).
3. Run the EDA notebook to explore ratings, reviews, discount trends, and device specifications.

## Dataset Fields (Cleaned)

The cleaned dataset includes these core columns:
- `brand`
- `model name`
- `model color`
- `storage`
- `review`
- `rating`
- `star rating`
- `ram`
- `display_size`
- `battery`
- `discount`

## Requirements

- Python 3.x
- Jupyter Notebook
- Google Chrome + compatible ChromeDriver
- Python libraries:
  - selenium
  - pandas
  - numpy
  - matplotlib
  - seaborn

Install dependencies (example):

```bash
pip install selenium pandas numpy matplotlib seaborn notebook
```

## Notes

- Some notebook cells use local Windows-style file paths; update paths to match your local environment before running.
- Website structure changes can impact scraping selectors over time.
