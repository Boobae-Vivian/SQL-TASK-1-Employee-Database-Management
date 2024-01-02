# Employee-Database-Management

## INTRODUCTION

In this database management task, the goal is to create a database named 'Staff' to efficiently manage information about employees. Two tables, 'Employee_Info' and 'Employee_Salary,' are designed with appropriate constraints to organize data related to staff details and their salary information. These constraints ensure data accuracy, consistency, and reliability. The task involves inserting ten rows of information into both tables, and then crafting SQL queries to retrieve specific data. Additionally, table and column renaming, along with changes to data types and the addition of a new column, are performed to enhance the structure and functionality of the database. This task encompasses various aspects of database administration, including schema design, data insertion, querying, and schema modification, contributing to the effective management of employee information within the 'Staff' database.

## PROBLEM STATEMENT

1. Create a comprehensive database named 'Staff'. Within this database, create two tables, 'Staff_Info' and 'Staff_Salary', with specific constraints to ensure data integrity and accuracy. The structure of the tables should include the following columns:
   - 'Staff_Info' (ID, Name, Age, DOE, Contract_Duration)
   - 'Staff_Salary' (ID, Salary, Yearly_Increment)
2. Insert into 'staff_info' and 'staff_salary', ten (10) rows of informations
3. Construct SQL queries to extract specific details:
   - The Name and Age from the 'Staff_Info' table.
   - The ID and Salary from the 'Staff_Salary' table.
5. Rename the existing tables to 'Employee_Info' and 'Employee_Salary,'
6. Change the 'ID' columns in both table to 'Employee_ID.'
7. Alter the 'Employee_ID' columns data types to 'Text' data types
8. Create a new column named 'Department' in the 'Employee_Salary' table
9. For Employees with the following IDs, update their Departments with the specified:
   - IDs 1, 3, 7 = IT
   - IDs 2, 5, 9 = Advertising
   - IDs 4, 6, 8, 10 = Communications
10. Execute a query to retrieve the Month, Year, and Day of each employee's entry into the company
11. Execute and update a query to add 10 years to the entry year of each employee as their 'Year_of_Exit'
12. Replace the department ‘Communications’ with ‘Stakeholders’
13. Modify the 'Name' column to ensure that all values are in UPPER CASE
14. Execute a query to display the Employees' Names and Date of Entry (DOE) in a single column named 'Employee's Brief'.

## SKILLS AND CONCEPTS DEMOSTRATED

The task involves various skills and concepts related to database management and SQL. Here are the possible skills and concepts to be demonstrated:
1. Database Design:
   - Understanding of how to design a database schema, including defining tables, primary keys, and relationships.
2. Constraints:
   - Application of constraints such as primary key constraints, not null constraints, unique constraints, default constraints and foreign key constraints to ensure data integrity.
3. Data Insertion:
   - Knowledge of inserting data into tables, including handling constraints and ensuring data consistency.
4. SQL Queries:
   - Writing SQL queries to retrieve specific information from the database, including SELECT statements with various conditions.
5. Data Modification:
   - Ability to modify the structure of the database, including renaming tables, columns, and changing data types.
6. Data Types:
   - Understanding and handling data types, including converting data types to meet specific requirements.
7. Column Addition:
   - Adding new columns to existing tables to accommodate additional information.
8. Table Renaming:
   - Renaming tables to adhere to standardized naming conventions and improve table clarity.
9. Data Transformation:
   - Transforming data during retrieval, such as displaying concatenated values in a single column.
10. SQL Execution:
    - Executing SQL queries and modification statements using a database management system.
      
By completing the task successfully, one can demonstrate proficiency in these skills and concepts, showcasing a comprehensive understanding of database administration and SQL manipulation.

## RESULTS AND DISCUSSIONS

### 1. Create a comprehensive database named 'Staff'. Within this database, create two tables, 'Staff_Info' and 'Staff_Salary':

To initiate the creation of a database named 'staff' and simultaneously establish two tables, namely 'staff_info' and 'staff_salary' within the database, the initial set of commands to be employed are as follows:

```sql
CREATE DATABASE Staff;


USE Staff
CREATE TABLE Staff_Info
(ID INT NOT NULL,
Name VARCHAR(50) NOT NULL,
Age INT DEFAULT "25",
DOE DATE DEFAULT "2022-06-30",
Contract_Duration VARCHAR(50) DEFAULT "Three months");


USE Staff;
CREATE TABLE Staff_Salary
(ID INT UNIQUE,
Salary INT NOT NULL,
Yearly_Increment VARCHAR(50) DEFAULT "Three months");


To execute these commands, initiate the analysis by clicking the fourth icon within the workbench interface.
Subsequently, the 'staff' database, along with the 'staff_info' and 'staff_salary' tables, will be created.

````

Staff and Staff_Info        | Staff_Salary
:-----------------:|:------------------:
![](TASK1a.png)    |![](TASK1b.png)


    












