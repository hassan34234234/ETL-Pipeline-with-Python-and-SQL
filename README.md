
# ETL Pipeline with Python and SQL

## Project Overview

In this project, I designed and implemented an ETL (Extract, Transform, Load) pipeline to streamline the handling of loan application data. The pipeline involves:

- Extracting raw data from a CSV file.
- Transforming the data using Python and Pandas for data cleaning and preparation.
- Loading the cleaned data into a PostgreSQL database.

## Setting Up the Database

### Step 1: Establishing the PostgreSQL Database

I started by creating a PostgreSQL database named `myfirst` on my local machine. This database serves as the foundation for storing all loan application data.

### Step 2: Defining Data Tables

The structure of the database is defined by a table named `accountinformation`. This table includes the following fields:

- **Loan ID:** Unique identifier for each loan application.
- **Gender:** Applicant's gender.
- **Marital Status:** Applicant's marital status.
- **Income Details:** Applicant's income information.
- **Loan Approval Status:** Status of the loan application (approved/rejected).

## Data Extraction

Using Pandas, I read the finance data from a CSV file. This involved selecting relevant columns and ensuring data consistency for smooth processing.

## Data Transformation

The transformation process involved cleaning and preparing the data using Python and Pandas. This step included handling missing values, converting data types, and ensuring data integrity.

## Loading Data into PostgreSQL

Using Python’s `psycopg2` library, I programmatically inserted the cleaned data into the PostgreSQL database. Each row of the Pandas DataFrame was mapped to corresponding fields in the database table.

## SQL Queries for Analysis

Additionally, I executed SQL queries directly on PostgreSQL to perform data analysis tasks. This allowed me to derive insights from the cleaned data and validate the integrity of the ETL process.

## Outcome and Learnings

Through this project, I gained hands-on experience in database management, ETL pipelines, and data integrity practices. It reinforced my skills in Python programming, SQL queries, and data manipulation with Pandas.

## Project Structure

```plaintext
ETL-Pipeline-with-Python-and-SQL/
│
├── data/
│   └── loan_data.csv                # Raw data file
│
├── scripts/
│   ├── extract.py                   # Script for data extraction
│   ├── transform.py                 # Script for data transformation
│   └── load.py                      # Script for data loading
│
├── sql/
│   └── create_table.sql             # SQL script for creating the table
│
├── notebooks/
│   └── ETL_pipeline_demo.ipynb      # Jupyter notebook demonstrating the ETL process
│
├── README.md                        # Project description
│
└── requirements.txt                 # Python dependencies
