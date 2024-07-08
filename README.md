# ETL-Pipeline-with-Python-and-SQL

In this project, I designed and implemented an ETL pipeline to streamline the handling of loan application data. The pipeline involves extracting raw data from a CSV file, transforming it using Python and Pandas for data cleaning and preparation, and loading it into a PostgreSQL database.

Setting Up the Database:

I began by establishing a PostgreSQL database named myfirst on my local machine. This database served as the foundation for storing all loan application data.

Defining Data Tables:

Next, I defined the structure of the database by creating a table named accountinformation. This table included fields such as Loan ID, Gender, Marital Status, Income Details, and Loan Approval Status.

Data Extraction:

I utilized Pandas to read the finance data from a CSV file. This involved selecting relevant columns and ensuring data consistency for smooth processing.

Loading Data into PostgreSQL:

Using Python’s psycopg2 library, I programmatically inserted cleaned data into the PostgreSQL database. Each row of the Pandas DataFrame was mapped to corresponding fields in the database table.

Outcome and Learnings:

Through this project, I gained hands-on experience in database management, ETL pipelines, and data integrity practices.

It reinforced my skills in Python programming, SQL queries, and data manipulation with Pandas.

SQL Queries for Analysis:

Additionally, I executed SQL queries directly on PostgreSQL to perform data analysis tasks. 
