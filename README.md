# SQL From Scratch - One Query at a time!
This repository is build for **curious minds who want to master SQL from the ground up** - whether you're a complete newbie or someone brushing up their skills. 

# SQL Basics/Meaning
SQL (Structured Query Language) is the standard language for managing and manipulating relational databases. It's an essential skill for 
anyone working with data. 

# How to run query or command using SQL Play Application

**The Query Editor**

You see a text box with **SELECT title from employees**. This is where you will type your SQL commands. 

**The Green Play/Send Button** 

In the bottom right, that green button is what you tap to **execute** the SQL command you've typed. 

![Image](https://github.com/user-attachments/assets/5d4afc0f-2aa1-48f5-b9ed-84a78aa3db2b)

## TIPS
(i) To make a text bold use **text**

(ii) To add image go to issues > drag and drop your image > a url will be created > from there copy the url > paste the url where you need to show image. 

# Understanding the **SELECT** Statement

![Image](https://github.com/user-attachments/assets/5d4afc0f-2aa1-48f5-b9ed-84a78aa3db2b)


The **SELECT** statement is the most fundamental and frequently used command in SQL. 
Its how you ask the database to give you data. 

The basic structure you just used in the screenshot above is:
**SELECT** column_name
**FROM** table_name;

- **SELECT**: This keyword tells the database you want to retrieve data.
- **column_name**: This is the name of the column you want to see. In our case, it was **title**
- **FROM**: This keyword specifies which table you want to get the data from.
- **table_name**: This is the name of the table. In our case, it was **employees**

## TIPS
(1) In order to use bullet points use "-" before your text.

# First Step: Selecting All Columns

Often you want to see all the data for each row in table, not just single column. 
For this, we use the asterisk (*) as a wildcard character. 

Steps to follow
(1) In your SQL Play app clear the current query in the editor area (delete **SELECT title from employees)**.
(2) Type the following command into the editor:
    SELECT *
    FROM employees;
(3) Tap the green play/send button in the bottom right corner. 

**What to expect**

You should now see all the columns and all the rows from the **employees** table. 
This will give us a better idea of what other columns (like **name**, **id**, **salary**, etc.) are available in this table. 

![Image](https://github.com/user-attachments/assets/1ac66c40-d9ee-4ff4-8d1d-6747d183ce71)

# Selecting Specific Columns (Practice 1)
(1) In your SQL Play app, clear the current query in the editor. 

(2) Type the following command to retrieve the first name, last name and email of all employees

**SELECT** FirstName, Lastname, Email

**FROM** employees;

(3) Tap the green play/send button. 

![Image](https://github.com/user-attachments/assets/b939c0f4-d24f-491e-9bb8-ae91b434ebf1)


# Lets Learn One concept At A Time

## Concept 1 : CREATE > INSERT > SELECT

# Concept 1.1: Create a small table
Using the following query you can create table which you could use to learn further:

![Image](https://github.com/user-attachments/assets/4e7c10f9-e62e-47f5-952d-ad441a0e90bd)

Lets try with one more query this time we add Products table
Use the following query to create Products table

![Image](https://github.com/user-attachments/assets/4ad1e855-8910-4473-8f7e-aac12522b143)

Once you have created a table you can simply follow the steps to display all the tables available

![Image](https://github.com/user-attachments/assets/647b5d82-047f-4030-983d-f4cc03d5d56b)

1. Once you open your SQL Play application on your android device you will be able to see 3 lines at top left
2. Click 3 lines at top left
3. Select List all tables
4. You will get a list of all tables available and created

# Concept 1.1.1: Understanding data available with you before moving ahead with advanced queries

The * means select all columns from a table. Think of it as “show me the whole table.”

1. Customers Table

SELECT * FROM customers;

shows all details available in the table

![Image](https://github.com/user-attachments/assets/79f68713-3148-4358-af94-a517a629650c)

2. Employees Table

SELECT * FROM employees;

shows all details available in employees table like Title, State, PostalCode, Phone, Last Name, First Name, Fax, Employee Id, Email, Address.

![Image](https://github.com/user-attachments/assets/72a6853f-3c57-4b9e-a82a-63b01686b171)

3. Albums Table

SELECT * FROM albums;

shows details available in table such as Title, Artistid, AlbumId

![Image](https://github.com/user-attachments/assets/d0573d43-d072-44a6-b12e-fdc7b1b26ef2)

4. Artists Table

SELECT * FROM artists;

shows details like Name & ArtistId

![Image](https://github.com/user-attachments/assets/8c1483d4-463f-4da7-be66-9212b8804dbe)

5. Tracks Table

SELECT * FROM tracks;

Shows all music tracks (TrackId, Name, AlbumId, MediaTypeId, GenreId, Composer, UnitPrice, etc.).

![Image](https://github.com/user-attachments/assets/7c5856ec-05b4-4d49-9174-631bc19b9554)

6. Students Table

SELECT * FROM students;

Shows the student data you inserted earlier

![Image](https://github.com/user-attachments/assets/d86cd748-f231-4538-bfd3-040672699520)

7. Products Table

SELECT * FROM Products;

Shows your products with name, price, stock, etc.

![Image](https://github.com/user-attachments/assets/9d8eb93f-049d-46dc-80ba-cb3923b10b4a)i


**PRACTISE** **FOR** **GETTING** **DATA** **BASED** **ON** **REQUIREMENT** **OR** **QUESTION** **ASKED**

Q1: What kind of columns or rows can I find in customers table?

A: SELECT * from customers;

![Image](https://github.com/user-attachments/assets/177578cd-e785-4dec-b5c7-6786f8b249c6)


Q2: Write me a query such that I get the data available in employees table

A: SELECT * FROM employees

![Image](https://github.com/user-attachments/assets/a74b21db-3188-4932-9ad2-0f95ec00a9d8)


Q3: Write me query one by one for showing data in albums, artists, tracks, students & Products

A: SELECT * FROM albums
A: SELECT * FROM artists
A: SELECT * FROM tracks
A: SELECT * FROM students
A: SELECT * FROM Products


**SELECTING** **SPECIFIC** **COLUMNS** **INSTEAD** **OF** **EVERYTHING** **IN** **THE** **TABLE**

When you run
SELECT * FROM students;
The * means “select all columns” from the table. But sometimes, you don’t need everything — maybe just name and city.

Query to use to get the data from specific columns
SELECT column1, column2, ...
FROM table_name;

For students table let run few queries to get data in specific column 

1. Select only name and city:

SELECT name, city
FROM students;

![Image](https://github.com/user-attachments/assets/2fa27951-446f-471d-bb4a-eceb398cf5e1)

2. Select only name and grade

SELECT name, grade
FROM students;

3. Select only age

SELECT age
FROM students;

4. Select name, age, city

SELECT name, age, city
FROM students;


# HOW TO RENAME COLUMNS

Using the following query you will be able to rename any column

SELECT column_name AS new_name
FROM table_name;

1. Rename one column from students table

SELECT name AS student_name
FROM students;

Output will show column heading as student_name instead of name.

![Image](https://github.com/user-attachments/assets/4b8b9c4c-7081-4436-a153-90d92e05b5bf)

2. Rename multiple column

SELECT name AS student_name, city AS hometown
FROM students;

Output will show headings student_name and hometown

![Image](https://github.com/user-attachments/assets/9bebe631-1f73-46d5-921c-b9e9ca654472)


# FILTERING RESULTS

In SQL filtering is done with the WHERE clause. It lets you return only the rows that meet certain conditions

Syntax to be used

SELECT column1, column2
FROM table_name
WHERE condition;

Example with students table

1. Filter by city

SELECT name, city
FROM students
WHERE city = 'Mumbai';

![Image](https://github.com/user-attachments/assets/378dbe60-90c2-46b7-8687-38fd80abee73)

2. Filter by age

SELECT name, age
FROM students
WHERE age > 12;

![Image](https://github.com/user-attachments/assets/1c2d054b-cbdf-476a-bd21-ac5d3611a486)

3. Fiter by multiple conditions

SELECT name, grade, city
FROM students
WHERE city = 'Mumbai' AND grade = 7;

![Image](https://github.com/user-attachments/assets/aba3ae00-b0ab-4da7-a323-52f262acd6e0)

4. Filter by OR

SELECT name, city
FROM students
WHERE city = 'Pune' OR city = 'Nashik';

![Image](https://github.com/user-attachments/assets/a98f9926-80ef-4337-82a0-4745fe77e4a8)

5. Filter with NOT

SELECT name, city
FROM students
WHERE NOT city = 'Mumbai';

![Image](https://github.com/user-attachments/assets/f4649d3e-c1f9-468b-9d90-a89fbba938d2)


## LIKE IN SQL

The LIKE keyword is used in WHERE clause to search for a specific pattern in a column. 

% - matches zero or more characters
_ - matches exactly one character

1. Name starting with "M"

SELECT name, city
FROM students
WHERE name LIKE 'M%';


