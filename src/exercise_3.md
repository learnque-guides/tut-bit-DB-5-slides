# Exercise 3

* Alter table employees:
  * make employeeId column PRIMARY KEY, NOT NULL and IDENTITY.
* See what happens when you add two more entries in employees, this time without setting the employeeId manually:
  * 'Julie', 'Juliette', '1990-01-01', '0-800-900-111',  'julie@juliette.com', 5000
  * 'Sofie', 'Sophia', '1987-02-03', '0-800-900-222', 'sofie@sophia.com', 1700
* Create a new table departments, with columns:
  * departmentId - Integer, PRIMARY KEY, NOT NULL, IDENTITY
  * name - Varchar, NOT NULL
* Add two entries in table departments:
  * HR,
  * Finance.
* Connect the two tables together - employees should have a reference to departments:
  * add departmentId - Integer column to employees table,
  * assign John to HR and Julie to Finance.
* Delete entry HR from departments table:
  * Does this work?
  * Should we be able to delete it? If John is assigned to HR and we delete, is the data still correct?
* Create a foreign key in employees table to departments table:
  * departmentId column in employees should reference departmentId column in departments, remember the naming convention: fk_employees_departments.
* Now try to delete entry HR from departments table:
* Does this still work?
* Now try to add a new employee and set its departmentId to 10:
  * Does this work? Should it?
  * Try to add this new employee and set its departmentId to 1. Does this work?
* Try deleting the newly added employee:
  * Does it work? Should it?