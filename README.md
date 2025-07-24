🚀 Falcon 9 First Stage Landing Prediction
This project focuses on predicting the success of Falcon 9 first-stage landings, a critical aspect of SpaceX's mission to reduce space launch costs. Utilizing historical launch data, this project employs various data science and machine learning techniques, culminating in an interactive dashboard for analysis.

✨ Project Overview
The project follows a typical data science pipeline, from data collection and cleaning to exploratory data analysis, machine learning model building, and interactive visualization. The primary goal is to build models that can accurately predict whether a Falcon 9 booster will successfully land.

📋 Key Stages & Notebooks
This repository contains a series of Jupyter Notebooks and supporting files that detail each stage of the project:

webscraping.ipynb:

Purpose: Collects initial historical Falcon 9 launch data from Wikipedia using web scraping techniques.

Output: spacex_web_scraped.csv

SpaceX_API.ipynb:

Purpose: Fetches additional launch details from the SpaceX API and performs initial data processing to create a foundational dataset.

Output: dataset_part_1.csv.

Data_wrangling.ipynb:

Purpose: Cleans, preprocesses, and transforms the raw collected data. This includes handling missing values, converting data types, and preparing features for analysis.

Input: dataset_part_1.csv.

Output: dataset_part_2.csv.

EDA_SQL.ipynb:

Purpose: Performs Exploratory Data Analysis (EDA) using SQL queries to uncover patterns, relationships, and insights within the cleaned launch data.

EDA_VIZ.ipynb:

Purpose: Conducts further EDA using various visualization libraries (e.g., Matplotlib, Seaborn, Plotly) to visually explore the data and identify trends related to landing success. This notebook also performs final feature engineering.

Input: dataset_part_2.csv.

Output: dataset_part_3.csv (the final prepared dataset for machine learning).

Folium.ipynb:

Purpose: Focuses on geospatial analysis, visualizing launch sites and landing outcomes on interactive maps using the Folium library.

Input: spacex_launch_geo.csv.

Output: (No new CSV output specified, typically generates HTML maps).

SpaceX_Machine Learning Prediction.ipynb:

Purpose: Builds and evaluates various classification models (e.g., Logistic Regression, SVM, Decision Tree, KNN) to predict landing success. Includes hyperparameter tuning (e.g., GridSearchCV) and model evaluation metrics.

Input: dataset_part_3.csv.

my_dash.py:

Purpose: An interactive web dashboard built with Plotly Dash, allowing users to explore launch data.

Input: spacex_launch_dash.csv.

📊 Datasets
The project utilizes and generates several CSV files, following a clear data flow:

spacex_web_scraped.csv: Raw data from web scraping (webscraping.ipynb).

dataset_part_1.csv: Initial processed data from SpaceX API calls (SpaceX_API.ipynb).

dataset_part_2.csv: Cleaned and preprocessed data from data wrangling (Data_wrangling.ipynb).

dataset_part_3.csv: Final prepared dataset for machine learning, resulting from further EDA and feature engineering (EDA_VIZ.ipynb).

spacex_launch_geo.csv: Data specifically prepared for Folium mapping (Folium.ipynb).

spacex_launch_dash.csv: Data specifically prepared for the Plotly Dash application (my_dash.py).

🛠️ Technologies Used
Programming Language: Python 3.x

Data Manipulation: Pandas, NumPy

Web Scraping: Requests, BeautifulSoup

API Interaction: Requests

Database Interaction: SQLite (implicitly via data wrangling)

Machine Learning: Scikit-learn

Data Visualization: Matplotlib, Seaborn, Plotly, Folium

Interactive Dashboard: Plotly Dash

Environment Management: requirements.txt

🚀 Setup and Run
To set up and run this project locally, follow these steps:

1. Prerequisites
Python 3.9 or newer installed on your system.

Git installed.

2. Clone the Repository
Open your terminal or command prompt and clone this repository:

git clone https://github.com/tousifT5/Coursera_project.git 

3. Install Dependencies
All required Python libraries are listed in requirements.txt. Install them using pip:

pip install -r requirements.txt

4. Run the Jupyter Notebooks
You can explore the data analysis and model building process by running the Jupyter Notebooks in the specified order to ensure data flow:

jupyter notebook

This will open a browser window where you can navigate to and open each .ipynb file in sequence:

webscraping.ipynb

SpaceX_API.ipynb

Data_wrangling.ipynb

EDA_SQL.ipynb

EDA_VIZ.ipynb

Folium.ipynb

SpaceX_Machine Learning Prediction.ipynb

5. Run the Interactive Dashboard
To launch the Plotly Dash application:

python my_dash.py

After running, open your web browser and go to the address displayed in your terminal (usually http://127.0.0.1:8050/).

📂 Project Files
.gitignore: Specifies files and directories that Git should ignore (e.g., __pycache__, .ipynb_checkpoints, potentially large datasets if not intended for version control).

Data_wrangling.ipynb: Jupyter Notebook for data cleaning and preparation.

EDA_SQL.ipynb: Jupyter Notebook for Exploratory Data Analysis using SQL.

EDA_VIZ.ipynb: Jupyter Notebook for Exploratory Data Analysis using visualizations.

Folium.ipynb: Jupyter Notebook for geographical data visualization.

README.md: This project's README file.

SpaceX_API.ipynb: Jupyter Notebook for data collection via SpaceX API.

SpaceX_Machine Learning Prediction.ipynb: Jupyter Notebook for building and evaluating ML models.

dataset_part_1.csv: Intermediate dataset.

dataset_part_2.csv: Intermediate dataset.

dataset_part_3.csv: Intermediate dataset.

my_dash.py: Python script for the interactive Plotly Dash application.

requirements.txt: List of Python dependencies.

spacex_launch_dash.csv: Dataset specifically prepared for the Dash app.

spacex_launch_geo.csv: Dataset specifically prepared for Folium.

spacex_web_scraped.csv: Raw data obtained from web scraping.

webscraping.ipynb: Jupyter Notebook for web scraping.