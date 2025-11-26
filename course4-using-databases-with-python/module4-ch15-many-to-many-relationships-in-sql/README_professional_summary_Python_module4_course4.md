📦 Module 4: Many-to-Many Relationships in SQL

Course: Using Databases with Python
Specialization: Python for Everybody
Platform: Coursera – University of Michigan
Module: Chapter 15 – Many-to-Many Relationships in SQL
Date Completed: ✅ 
Directory: module4-ch15-many-to-many-relationships-in-sql

🎯 Module Objective

This module explored how to model complex relational data structures, focusing on many-to-many relationships — where a single student may be enrolled in multiple courses and each course may have many students. I used Python to read and parse JSON data and created SQL tables that reflected real-world enrollment data through primary and foreign key relationships.

The goal was to build a normalized database schema that supports efficient querying and updates, then populate and query that structure using Python scripts and SQL.

📁 Folder Contents

many-to-many-relationships-and-python.txt:
My notes and code breakdown for the "Many-to-Many Relationships and Python" assignment.

Many Students in Many Courses_Answer.txt:
My solution for the second graded app item, including the output and observations.

Many Students in Many Courses_Instructions.png:
Screenshot of the problem prompt for the multi-table assignment.

roster/:
A subfolder containing all files related to the roster.py exercise:

roster_data.json – Source data to be parsed and inserted into the database

roster_data.py – Python script to process and populate the database

rosterdb.sql – SQL schema file defining User, Course, and Member tables

rosterdb.sqlite – Final SQLite database after running the script

rosterdb.sqbpro – Optional database viewer file for inspection

✅ Assignments Completed

Many-to-Many Relationships and Python
Graded Assignment — Score: 100%

Many Students in Many Courses
Graded App Item — Score: 100%

🔍 Key Concepts Practiced

Designing and normalizing many-to-many relationships using SQL JOIN tables

Writing Python scripts to parse JSON data and execute SQL INSERT/SELECT operations

Safeguarding against data duplication using INSERT OR IGNORE

Using executescript() to define multiple table schemas in one transaction

Verifying results by inspecting final .sqlite databases

💬 Reflection

This module made me feel more confident working with real-world relational database patterns, especially how to translate abstract relationships (students ↔ courses) into normalized table structures. Building the roster database from scratch and manipulating it with SQL queries through Python helped me understand the power of multi-table relationships and JOIN operations.

I now feel ready to design more complex schemas that involve intermediary tables, and I’ve begun thinking of database architecture not just in terms of code, but as part of overall system design.