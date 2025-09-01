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

