# ME204 Final Project: Brewery Characteristics Across the United States

| GitHub username | LSE ID |
|-----------------|--------|
| jtwinterle | 250086299 |

## Overview

This project investigates how brewery characteristics vary across the United States using data collected from the Open Brewery DB API. The project follows a complete data pipeline consisting of data collection, data preparation, data analysis, and communication through a public website.

The research question is:

**How do brewery characteristics vary across the United States?**

The analysis explores three key areas:

- The distribution of brewery types.
- The distribution of breweries across U.S. states.
- The geographic clustering of breweries throughout the United States.

## Data Sources

The project uses the Open Brewery DB API as its primary data source.

The API provides information including:

- Brewery name
- Brewery type
- City
- State
- Country
- Latitude
- Longitude
- Website URL
- Contact information

The raw API responses were collected in JSON format and stored in the `data/raw` folder before being cleaned and transformed into CSV files in the `data/processed` folder.

## Project Structure

```text
final-project/
│
├── README.md
├── .gitignore
├── .env.example
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
│   ├── NB01-Data-Collection.ipynb
│   ├── NB02-Data-Transformation.ipynb
│   └── NB03-jtwinterle-Data-Analysis.ipynb
├── docs/
│   ├── jtwinterle.md
│   ├── brewery.png
│   ├── states.png
│   └── geographic.png
```

## Notebook Summary

### NB01 – Data Collection

- Connected to the Open Brewery DB API.
- Downloaded brewery data.
- Stored the raw API responses as JSON files.
- Saved the raw data in the `data/raw` folder.

### NB02 – Data Transformation

- Loaded the raw JSON data.
- Examined missing values and duplicate records.
- Removed unnecessary variables.
- Prepared cleaned datasets for analysis.
- Saved processed CSV files in the `data/processed` folder.

### NB03 – Data Analysis

The analysis focused on answering the research question through three main findings:

1. Micro breweries are the most common brewery type.
2. Brewery activity is concentrated in a relatively small number of U.S. states.
3. Breweries form clear regional clusters across the United States.

Interactive Plotly visualisations were created to support each finding.

## Public Website

The public website is located in the `docs` folder. It presents the project's research question and summarizes the three strongest findings developed in NB03 using charts and explanations written for a general audience.

## Software Requirements

The project was completed using Python and the following libraries:

- pandas
- plotly
- pathlib

## How to Reproduce

To reproduce the project, run the notebooks in the following order:

1. `NB01-Data-Collection.ipynb`
2. `NB02-Data-Transformation.ipynb`
3. `NB03-jtwinterle-Data-Analysis.ipynb`

NB01 collects the brewery data from the Open Brewery DB API.

NB02 cleans and prepares the datasets for analysis.

NB03 loads the processed data, performs the analysis, and creates the visualisations used in the public website.

## Use of AI

Generative AI tools were used during the development of this project to assist with debugging Python code and improving the wording on my markdowns
