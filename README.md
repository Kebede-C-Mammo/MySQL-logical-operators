# MySQL-logical-operators

Reading exercise: Filtering data examples

Based in Tucson, Arizona, Lucky Shrub is a medium-sized company specializing in garden design, creation, maintenance and landscaping. The company also runs a small nursery that sells indoor and outdoor plants. Lucky Shrub has seven employees who work in six different departments.

Instructions
To complete this exercise, use MySQL on your own machine.

Prerequisites

You can use the below SQL scripts to set up the luckyshrub_db in your local environment.

CREATE DATABASE luckyshrub_db;

USE luckyshrub_db;

CREATE TABLE employees (
EmployeeID int NOT NULL,
EmployeeName varchar(150) DEFAULT NULL,
Department varchar(150) DEFAULT NULL,
ContactNo varchar(12) DEFAULT NULL,
Email varchar(100) DEFAULT NULL,
AnnualSalary int DEFAULT NULL,
PRIMARY KEY (EmployeeID)
);

INSERT INTO employees VALUES
(1,'Seamus Hogan', 'Recruitment', '351478025', 'Seamus.h@luckyshrub.com',50000),
(2,'Thomas Eriksson', 'Legal', '351475058', 'Thomas.e@ luckyshrub.com',75000),
(3,'Simon Tolo', 'Marketing', '351930582','Simon.t@ luckyshrub.com',40000),
(4,'Francesca Soffia', 'Finance', '351258569','Francesca.s@ luckyshrub.com',45000),
(5,'Emily Sierra', 'Customer Service', '351083098','Emily.s@ luckyshrub.com',35000),
(6,'Maria Carter', 'Human Resources', '351022508','Maria.c@ luckyshrub.com',55000),
(7,'Rick Griffin', 'Marketing', '351478458','Rick.G@luckyshrub.com',50000);

TODOs:
Lucky Shrub management needs to generate reports based on this employee data by completing the following tasks:

Task 1: Use the AND operator to find employees who earn an annual salary of $50,000 or more attached to the Marketing department.

Task 2: Use the NOT operator to find employees not earning over $50,000 across all departments.

Task 3: Use the IN operator to find Marketing, Finance, and Legal employees whose annual salary is below $50,000.

Task 4: Use the BETWEEN operator to find employees who earn annual salaries between $10,000 and $50,000.

Task 5: Use the LIKE operator to find employees whose names start with ‘S’ and are at least 4 characters in length.
