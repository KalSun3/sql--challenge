# SQL Challenge: Employee Database Analysis

## Overview
This project involves analyzing employee data for a fictional company, **Pewlett Hackard**, focusing on employees from the 1980s and 1990s. The provided task consists of three major steps: Data Modeling, Data Engineering, and Data Analysis.

In this repository, you'll find SQL scripts for database schema creation, data importation, and queries to analyze the data. Additionally, the **analysis folder** contains corresponding PNG files for each SQL query that visually represents the results of the analysis.

## Project Structure

```plaintext
sql-challenge/       # Directory for the challenge project
data                 # Folder containing all CSV files
│   │   ├── departments.csv     
│   │   ├── dept_emp.csv
│   │   ├── dept_manager.csv     
│   │   ├── employees.csv
│   │   ├── salaries.csv     
│   │   ├── titles.csv     
data_analysis 
│   │── PGAdmin Screenshots / (PNG files)
│   │   ├── 1.png       # Visualization for Query 1
│   │   ├── 2.png       # Visualization for Query 2
│   │   ├── 3.png       # Visualization for Query 3
│   │   ├── 4.png       # Visualization for Query 4
│   │   ├── 5.png       # Visualization for Query 5
│   │   ├── 6.png       # Visualization for Query 6
│   │   ├── 7.png       # Visualization for Query 7
│   │   ├── 8.png       # Visualization for Query 8
│   ├── schema/         # Folder containing SQL schema files
│   │   ├── create_tables.sql
│   │   ├── insert_data.sql
│   ├── queries/       # Folder containing SQL analysis queries
│   │   ├── analysis_query.sql    # SQL for all 8 Queries
data_engineering  # Folder containing SQL schema files
│   │   ├── create_tables.sql
data_modeling  # Folder containing ERD from QuickDBD
│   ├── ERD.png           # Entity Relationship Diagram (ERD)
└── README.md             # This file

Steps
1. Data Modeling
In this phase, the structure of the data was analyzed, and an Entity Relationship Diagram (ERD) was created. The ERD outlines the relationships between different tables, such as Employees, Departments, Salaries, and Titles.

ERD: The Entity Relationship Diagram visualizes how the tables relate to each other through primary and foreign keys.
You can find the ERD in data_modeling/ERD.png.
2. Data Engineering
In this phase, the database schema was created and the data was imported from the provided CSV files into the SQL database. The following steps were carried out:

Tables Created:

Employees: Employee details (e.g., name, sex, hire date, salary).
Departments: Department names and numbers.
Salaries: Salary information tied to employees.
Titles: Job titles assigned to employees.
Dept_emp: Information about which employees belong to which departments.
Dept_manager: Information about which employees manage which departments.
SQL Scripts:

create_tables.sql: Contains SQL statements to create all necessary tables.
insert_data.sql: Contains SQL statements to import data from the CSV files into the tables.
You can find these SQL files in the data_analysis/schema/ directory.

3. Data Analysis
In this phase, SQL queries were written to answer a series of business questions. Each query provides insights about the employees, their departments, salaries, and other attributes.

The SQL queries are located in the data_analysis/queries/ folder in the analysis_query.sql file, which contains all eight queries.

For each query, there is a corresponding visualization of the results in the data_analysis/PGAdmin Screenshots/ folder. The visualizations are in PNG format and provide a visual representation of the results, as seen in the following example files:
1.png: Visualization for Query 1
2.png: Visualization for Query 2
3.png: Visualization for Query 3
4.png: Visualization for Query 4
5.png: Visualization for Query 5
6.png: Visualization for Query 6
7.png: Visualization for Query 7
8.png: Visualization for Query 8
Queries:
Each of the queries below was designed to answer a specific business question:

Employee Details: List employee number, last name, first name, sex, and salary.
Employees Hired in 1986: List first name, last name, and hire date for employees hired in 1986.
Department Managers: List the manager of each department along with department details.
Employee Department Details: List the department number for each employee along with their department name and employee details.
Employees Named Hercules: List first name, last name, and sex of employees whose first name is Hercules and whose last name starts with "B".
Sales Department Employees: List employees in the Sales department, including employee number, last name, and first name.
Employees in Sales and Development: List employees in both Sales and Development departments, including their department names.
Frequency of Last Names: List the frequency counts of employee last names, ordered by most common last name.

How to Run This Project
Clone this repository:

bash
Copy code
git clone https://github.com/KalSun3/sql--challenge.git
cd sql-challenge
Set up the SQL database:

Create a new database in your SQL server.
Run the data_engineering/create_tables.sql file to create the necessary tables.
Run the data_analysis/schema/insert_data.sql file to insert the data from the CSV files into the tables.
Run the Analysis Queries:

Execute the queries in data_analysis/queries/analysis_query.sql to get the results.
View the corresponding visualizations in the data_analysis/PGAdmin Screenshots/ folder. The PNG files represent the output of each query.
Check the Visualizations:

Each query result is visualized and saved as a PNG file in the PGAdmin Screenshots/ folder. Open the PNG files to see the query output.
Requirements
SQL Server: The project is compatible with any relational database that supports SQL (e.g., MySQL, PostgreSQL).
Data Visualization: PNG files are generated using external tools and are included for reference.
Acknowledgments
Special thanks to Pewlett Hackard for providing the fictional dataset.
License
This project is licensed under the MIT License - see the LICENSE file for details.


