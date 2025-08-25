# Steam 200K Dataset Analysis
## Overview
This project analyzes the **Steam 200K** dataset, which contains user interaction logs from the Steam gaming platform. The dataset includes information about game purchases and playtime across thousands of users.
The main notebook (`Project 2.ipynb`) is implemented in **PySpark** on **Databricks** and demonstrates:
- Data loading into Spark
- Exploratory Data Analysis (EDA) with SQL & PySpark
- Data cleaning and preparation
- Feature engineering (unique game IDs, structured tables)
## Requirements
This project is designed for **Databricks** (or any Spark environment).
**Main dependencies:**
- PySpark
- MLflow (for experiment tracking)
- Databricks utilities (`dbutils`)
- Jupyter Notebook (if running locally)
If running locally with Spark installed, install dependencies with:
```bash
pip install pyspark mlflow
```
## How to Run
1. **Upload the dataset** `steam-200k.csv` into your Databricks FileStore:
   - `/FileStore/tables/steam_200k.csv`
2. **Import the notebook** `Project 2.ipynb` into Databricks.
3. **Run the notebook cells step by step.**
   - The dataset is read into a Spark DataFrame.
   - SQL queries explore the dataset (purchase counts, play hours, etc.).
   - Feature engineering creates unique numeric IDs for games.
## Project Structure
```
├── Project 2.ipynb        # Main notebook
├── data/
│   └── steam-200k.csv     # Dataset (user-game interactions)
├── output/                # Any processed data or results
└── README.md              # Project documentation
```
## Results
- Successfully loaded `steam-200k.csv` into Spark.
- Performed exploratory analysis with SQL (e.g., top games by playtime, purchase frequency).
- Created unique `GameId` identifiers and joined them with the dataset.
- Prepared cleaned and structured data for further analysis or ML tasks.
## Notes
- This notebook is built for Databricks, but can be adapted to local Spark setups.
- Ensure `steam-200k.csv` is uploaded to the correct path.
- MLflow is enabled for experiment tracking, though not all runs may log results unless extended with ML models.
# python-project-
