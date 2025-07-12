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

