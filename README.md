# Workshop #1 Candidate Data Analysis

 This project was developed as part of a data engineer challenge and serves as a portfolio piece showcasing my skills in data extraction, transformation, loading, and visualization. I built this project from scratch to simulate a real job interview exercise, where I received a CSV file containing 50k rows of randomly generated candidate data.

## Project Overview

In this project, my main goal was to:
- **Extract** data from a CSV file containing candidate information.
- **Transform and load** the data into a relational database in PostgreSQL.
- **Analyze** the data using Jupyter Notebooks.
- **Visualize** the results in Power BI, creating several key charts.

## Tools and Technologies

For this project, I used the following tools:
- **Python** – For data manipulation and processing.
- **Jupyter Notebooks** – To perform the extraction, transformation, and analysis.
- **PostgreSQL** –  to store and query the candidate data.
- **Power BI Desktop** – To build interactive dashboards.
- **Additional Libraries:**
  - Pandas
  - NumPy
  - Matplotlib
  - Seaborn
  - psycopg2-binary
  - SQLAlchemy
  - python-dotenv
  - SQLAlchemy-Utils

All the exact versions of the libraries can be found in the `requirements.txt` file.

## About the data
This dataset has 50k rows of data about candidates. The column names and their respective data types before data transformation are:

First Name: Object
Last Name: Object
Email: Object
Application Date: Object
Country: Object
YOE (Years of Experience): Integer
Seniority: Object
Technology: Object
Code Challenge Score: Integer
Technical Interview Score: Integer

## Repository Organization

### data: 
This folder contains the CSV file candidates.csv used as the source data for the analysis.
### notebooks: 
This folder contains all the Jupyter notebooks:
001_extraction_and_load.ipynb: Responsible for data extraction and loading, and for creating the raw_candidates table.
002_Candidates_EDA.ipynb: Used for exploratory data analysis (EDA) on the dataset.
003_DataCleanAndLload.ipynb: Handles data cleaning and transformation, ultimately creating a new PostgreSQL table called cadidates_hired.
### SRC: 
This folder holds supporting code and resources such as the powerBI_candidates.pdf dashboard guide and the requirements.txt file for installing necessary dependencies.

## Installation and Setup

Follow these steps to set up the project on your local machine:

1. **Clone the Repository:**

    ```bash
    git clone https://github.com/Juanjoslo2/WorkShop-1.git
    ```

2. **Navigate to the Project Directory:**

    ```bash
    cd WorkShop-1
    ```

3. **Create a Virtual Environment:**

    ```bash
    python -m venv venv
    ```

4. **Activate the Virtual Environment:**
    
      ```bash
      venv\Scripts\activate
      ```

5. **Install Dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

6. **Create Database in postgreSQL**

## Running the Project

1. **Data Extraction and Load:**
   - Open and run the `001_extraction_and_load.ipynb` notebook to load the CSV data into your database.

2. **Exploratory Data Analysis (EDA):**
   - Execute the `002_Candidates_EDA.ipynb` notebook to explore the dataset and understand its characteristics.

3. **Data Cleaning and Transformation:**
   - Run the `003_DataCleanAndLload.ipynb` notebook to clean the data and apply the necessary transformations (including the "HIRED" logic).


