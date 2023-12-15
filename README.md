# SpaceX Launch Data Analysis Project

## Overview

This project aims to predict the success of Falcon 9 first-stage landings using SpaceX launch data. By determining if the first stage will land successfully, we can estimate the cost of a launch, which is crucial for competitive bidding in the space industry.

## Notebooks

1. **Spacex_Data_Collection_using_API:**
   - Request data from the SpaceX API.
   - Perform basic data wrangling and formatting.
   - Output: `dataset_part_1.csv`

2. **Webscraping_Falcon-9_&_Falcon_Heavy_Launches_Records_from_Wikipedia:**
   - Web scrape Falcon-9 launch records from Wikipedia.
   - Extract and parse HTML tables.
   - Output: `spacex_web_scraped.csv`

3. **Data_Wrangling:**
   - Explore Data Analysis (EDA) to find patterns.
   - Convert outcomes into training labels (1 for success, 0 for failure).
   - Input: `dataset_part_1.csv`, Output: `dataset_part_2.csv`

4. **SpaceX_EDA_using_SQL_&_SQLlite:**
   - Understand the SpaceX dataset.
   - Load the dataset into a Db2 database.
   - Execute SQL queries to answer questions.
   - Input: `Spacex.csv`

5. **SpaceX_EDA_using_DataVis:**
   - Perform EDA and feature engineering using Pandas and Matplotlib.
   - Input: `dataset_part_2.csv`, Output: `dataset_part_3.csv`

6. **Launch-Site_Location_Analysis_using_Folium:**
   - Mark all launch sites on a map.
   - Mark success/failed launches for each site on the map.
   - Calculate distances between a launch site and its proximities.
   - Input: `spacex_launch_geo.csv`

7. **SpaceX_Dash_Application:**
   - Build a Plotly Dash application for interactive visual analytics.
   - Input: `spacex_launch_dash.csv`

8. **SpaceX_Falcon-9_Landing_Prediction_using_ML:**
   - Create a machine learning pipeline to predict first-stage landings.
   - Standardize data, split into training and test data.
   - Find the best hyperparameters for SVM, Classification Trees, and Logistic Regression.
   - Determine the best-performing method using test data.
   - Input: `dataset_part_2.csv`

## Repository Structure

- `README.md`: Project overview and instructions.
- Notebooks: Contain Jupyter notebooks for each phase of the project.
- `spacex_dash_app.py`: Plotly Dash script for the interactive web application.
- `datasets/`: Folder containing CSV files generated during the project.

## How to Use

1. Clone the repository.
2. Explore the notebooks in numerical order for a step-by-step walkthrough.
3. Run the Dash application using `python spacex_dash_app.py`.
4. Check the `datasets/` folder for generated CSV files.

Feel free to reach out on **92.mohsin.muhammad@gmail.com** for any questions or clarifications.

