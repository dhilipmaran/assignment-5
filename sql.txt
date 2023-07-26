
CREATE DATABASE Student;
CREATE DATABASE Employee;
CREATE DATABASE Bank;
CREATE DATABASE Library;
CREATE DATABASE Family;
USE Student;

CREATE TABLE student_details (
  id INT PRIMARY KEY,
  name VARCHAR(50),
  age INT,
  course VARCHAR(50),
  address VARCHAR(100)
);
USE Employee;

CREATE TABLE employee_details (
  id INT PRIMARY KEY,
  name VARCHAR(50),
  age INT,
  department VARCHAR(50),
  salary DECIMAL(10, 2)
);
USE Bank;

CREATE TABLE banki_nfo (
  id INT PRIMARY KEY,
  account_number VARCHAR(20),
  account_holder VARCHAR(50),
  balance DECIMAL(10, 2),
  branch VARCHAR(100)
);
USE Library;

CREATE TABLE book_details (
  id INT PRIMARY KEY,
  title VARCHAR(100),
  author VARCHAR(50),
  publication_year INT
);
USE Family;

CREATE TABLE family_tree (
  id INT PRIMARY KEY,
  name VARCHAR(50),
  age INT,
  relationship VARCHAR(50),
  occupation VARCHAR(50)
);
INSERT INTO Student.student_details (id,name, age, course, address)
VALUES
  (1,'James', 25, 'IT', 'CHENNAI'),
  (2,'Kavya', 20, 'AIML', 'TRICHY');
  SELECT * FROM Student.student_details;
  INSERT INTO Employee.employee_details (id,name, age, department, salary)
VALUES
  (1,'RAM', 35, 'DATA SCIENTIST', 45000),
  (2,'ED', 30, 'DEVELOPER', 55000);
  SELECT * FROM Employee.employee_details;
  INSERT INTO Bank.bank_info (id,account_number, account_holder, balance, branch)
VALUES
  (1,'123456', 'PYTHON', 50790, 'CHENNAI'),
  (2,'962672', 'JAVA', 17280, 'COIMBATORE');
  SELECT * FROM Bank.bank_info;
  INSERT INTO Library.book_details (id,title, author, publication_year)
VALUES
  (1,'Cyber security', 'kumar', 1925),
  (2,'Machine Learning', 'P. Ramanujam', 2004);
  SELECT * FROM Library.book_details;
  INSERT INTO Family.family_tree (id,name, age, relationship, occupation)
VALUES
  (1,'Sam', 50, 'Father', 'Mechanic'),
  (2,'Rajan', 70, 'Grandfather','Farmer'),
  (3,'Emily', 45,'Mother','Home maker') ;
SELECT * FROM Family.family_tree;
