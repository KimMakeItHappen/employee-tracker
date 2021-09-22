# employee-tracker

##### Table of Contents  

* [Description](#description)  
* [User Story](#userStory)
* [Acceptance Criteria](#acceptanceCriteria) 
* [Installation] (#Installation) 
* [Usage] (#Usage)
* [Mock-Up](#Mock-up)
* [Questions](#Questions)

# Description


Developers frequently have to create interfaces that allow non-developers to easily view and interact with information stored in databases. These interfaces are called content management systems (CMS). Your assignment this week is to build a command-line application from scratch to manage a company's employee database, using Node.js, Inquirer, and MySQL.
Because this application won’t be deployed, you’ll also need to create a walkthrough video that demonstrates its functionality and all of the following acceptance criteria being met. You’ll need to submit a link to the video and add it to the README of your project.

# User Story

AS A business owner
I WANT to be able to view and manage the departments, roles, and employees in my company
SO THAT I can organize and plan my business

# Acceptance Criteria

GIVEN a command-line application that accepts user input
WHEN I start the application
THEN I am presented with the following options: view all departments, view all roles, view all employees, add a department, add a role, add an employee, and update an employee role
WHEN I choose to view all departments
THEN I am presented with a formatted table showing department names and department ids
WHEN I choose to view all roles
THEN I am presented with the job title, role id, the department that role belongs to, and the salary for that role
WHEN I choose to view all employees
THEN I am presented with a formatted table showing employee data, including employee ids, first names, last names, job titles, departments, salaries, and managers that the employees report to
WHEN I choose to add a department
THEN I am prompted to enter the name of the department and that department is added to the database
WHEN I choose to add a role
THEN I am prompted to enter the name, salary, and department for the role and that role is added to the database
WHEN I choose to add an employee
THEN I am prompted to enter the employee’s first name, last name, role, and manager, and that employee is added to the database
WHEN I choose to update an employee role
THEN I am prompted to select an employee to update and their new role and this information is updated in the database 

# Installation
Install node.js, mysql, and npm. Then, clone this repo. Open the file called connection.js, which is located in the db folder. Create a .env file in the root directory with the following contents:

DB_USER='your username for mysql' DB_PASS='your password for mysql' DB_NAME='your database name'

You'll want to change the name of your database in the schema.sql file to match the name you choose for the .env file. Lastly, log into the mysql shell and type source schema.db. This will set up the database.

# Usage
Log into mysql in the terminal and type:

source ./db/schema.sql

This will set up the database. Then log out of mysql and type:

node index.js

This will open the application. To avoid errors, input your data in this order:

Add departments
Add roles
Add employees - start with managers before adding regular employees
If you need to update and employee role, choose "Update Employee Role". You can also choose to "View all Roles", "View all Departments", and "View all Employees".

# Mock-up
The following video shows an example of the application being used from the command line:
Screen Recording 2021-09-22 at 7.28.26 PM.mov