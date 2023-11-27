# LS180_database_foundations

## L1: INTRODUCTION

- [Introduction to the Course](https://github.com/SandyRodger/LS180_database_foundations/blob/main/01_introduction.md#introduction-to-the-course)
- [Welcome](https://github.com/SandyRodger/LS180_database_foundations/blob/main/01_introduction.md#welcome)
- [What this Course Covers](https://github.com/SandyRodger/LS180_database_foundations/blob/main/01_introduction.md#what-this-course-covers)
- [Setting Up Cloud Development Environments](https://github.com/SandyRodger/LS180_database_foundations/blob/main/01_introduction.md#setting-up-cloud-development-environments)
- [Read the Launch School SQL Book](https://github.com/SandyRodger/LS180_database_foundations/blob/main/01_introduction.md#read-the-launch-school-sql-book)
  - [Normalization](https://github.com/SandyRodger/LS180_database_foundations/blob/main/01_introduction.md#normalization)
  - [Keys](https://github.com/SandyRodger/LS180_database_foundations/blob/main/01_introduction.md#keys)
  - [Primary Keys](https://github.com/SandyRodger/LS180_database_foundations/blob/main/01_introduction.md#primary-keys)
  - [Foreign keys](https://github.com/SandyRodger/LS180_database_foundations/blob/main/01_introduction.md#foreign-keys)
  - [Referencial integrity](https://github.com/SandyRodger/LS180_database_foundations/blob/main/01_introduction.md#referencial-integrity)
  - [One to Many](https://github.com/SandyRodger/LS180_database_foundations/blob/main/01_introduction.md#one-to-many)
  - [Many to many](https://github.com/SandyRodger/LS180_database_foundations/blob/main/01_introduction.md#many-to-many)
  - [Database design](https://github.com/SandyRodger/LS180_database_foundations/blob/main/01_introduction.md#database-design)
  - [SQL joins](https://github.com/SandyRodger/LS180_database_foundations/blob/main/01_introduction.md#sql-joins)
  - [Types of joins](https://github.com/SandyRodger/LS180_database_foundations/blob/main/01_introduction.md#types-of-joins)
    - [Multiple joins](https://github.com/SandyRodger/LS180_database_foundations/blob/main/01_introduction.md#multiple-joins)
  - [Aliasing](https://github.com/SandyRodger/LS180_database_foundations/blob/main/01_introduction.md#aliasing)
  - [Subqueries](https://github.com/SandyRodger/LS180_database_foundations/blob/main/01_introduction.md#subqueries)
- [Reading PostgreSQL Documentation](https://github.com/SandyRodger/LS180_database_foundations/blob/main/01_introduction.md#reading-postgresql-documentation)
- [The PostgreSQL Command Line Interface](https://github.com/SandyRodger/LS180_database_foundations/blob/main/01_introduction.md#the-postgresql-command-line-interface)
- [Assignment: SQL Fundamentals - Easy 1](https://github.com/SandyRodger/LS180_database_foundations/blob/main/01_introduction.md#assignment-sql-fundamentals-easy-1)
- [Quiz Lesson 1](https://github.com/SandyRodger/LS180_database_foundations/blob/main/01_introduction.md#quiz-lesson-1)

## L2: SCHEMA, DATA AND SQL

- [Schema, data and SQL](https://github.com/SandyRodger/LS180_database_foundations/blob/main/02_schema_data_and_sql.md#schema-data-and-sql)
- [What to Focus On](https://github.com/SandyRodger/LS180_database_foundations/blob/main/02_schema_data_and_sql.md#what-to-focus-on)
- [The SQL Language](https://github.com/SandyRodger/LS180_database_foundations/blob/main/02_schema_data_and_sql.md#the-sql-language)
  - [Syntax](https://github.com/SandyRodger/LS180_database_foundations/blob/main/02_schema_data_and_sql.md#syntax)
  - [Practice problems: SQL Style Guide](https://github.com/SandyRodger/LS180_database_foundations/blob/main/02_schema_data_and_sql.md#practice-problems-sql-style-guide)
- [PostgreSQL Data Types](https://github.com/SandyRodger/LS180_database_foundations/blob/main/02_schema_data_and_sql.md#postgresql-data-types)
  - [NULL](https://github.com/SandyRodger/LS180_database_foundations/blob/main/02_schema_data_and_sql.md#null)
  - [Practice problems: Working with a Single Table](https://github.com/SandyRodger/LS180_database_foundations/blob/main/02_schema_data_and_sql.md#practice-problems-working-with-a-single-table)
- [More Single Table Queries](https://github.com/SandyRodger/LS180_database_foundations/blob/main/02_schema_data_and_sql.md#more-single-table-queries)
- [NOT NULL and Default Values](https://github.com/SandyRodger/LS180_database_foundations/blob/main/02_schema_data_and_sql.md#not-null-and-default-values)
  - [Practice problems: More Constraints](https://github.com/SandyRodger/LS180_database_foundations/blob/main/02_schema_data_and_sql.md#practice-problems-more-constraints)
- [Using Keys](https://github.com/SandyRodger/LS180_database_foundations/blob/main/02_schema_data_and_sql.md#using-keys)
  - [Natural Keys](https://github.com/SandyRodger/LS180_database_foundations/blob/main/02_schema_data_and_sql.md#natural-keys)
  - [Surrogate Keys](https://github.com/SandyRodger/LS180_database_foundations/blob/main/02_schema_data_and_sql.md#surrogate-keys)
    - [Sequences](https://github.com/SandyRodger/LS180_database_foundations/blob/main/02_schema_data_and_sql.md#sequences)
  - [Enforcing uniqueness](https://github.com/SandyRodger/LS180_database_foundations/blob/main/02_schema_data_and_sql.md#enforcing-uniqueness)
  - [Primary keys](https://github.com/SandyRodger/LS180_database_foundations/blob/main/02_schema_data_and_sql.md#primary-keys)
    - [UUIDs](https://github.com/SandyRodger/LS180_database_foundations/blob/main/02_schema_data_and_sql.md#uuids)
  - [Practice problems](https://github.com/SandyRodger/LS180_database_foundations/blob/main/02_schema_data_and_sql.md#practice-problems)
- [GROUP BY and Aggregate Functions](https://github.com/SandyRodger/LS180_database_foundations/blob/main/02_schema_data_and_sql.md#group-by-and-aggregate-functions)
- [How PostgreSQL Executes Queries](https://github.com/SandyRodger/LS180_database_foundations/blob/main/02_schema_data_and_sql.md#how-postgresql-executes-queries)
- [Table and Column Aliases](https://github.com/SandyRodger/LS180_database_foundations/blob/main/02_schema_data_and_sql.md#table-and-column-aliases)
- [Summary](https://github.com/SandyRodger/LS180_database_foundations/blob/main/02_schema_data_and_sql.md#summary)
- [Quiz Lesson 2](https://github.com/SandyRodger/LS180_database_foundations/blob/main/02_schema_data_and_sql.md#quiz-lesson-2)

## L3: RELATIONAL DATA AND JOINS

- [Relational Data and Joins](https://github.com/SandyRodger/LS180_database_foundations/blob/main/03_relational_data_and_joins.md#relational-data-and-joins)
- [What to Focus On](https://github.com/SandyRodger/LS180_database_foundations/blob/main/03_relational_data_and_joins.md#what-to-focus-on)
- [What is Relational Data?](https://github.com/SandyRodger/LS180_database_foundations/blob/main/03_relational_data_and_joins.md#what-is-relational-data)
- [Database Diagrams: Levels of Schema](https://github.com/SandyRodger/LS180_database_foundations/blob/main/03_relational_data_and_joins.md#database-diagrams-levels-of-schema)
- [Database Diagrams: Cardinality and Modality](https://github.com/SandyRodger/LS180_database_foundations/blob/main/03_relational_data_and_joins.md#database-diagrams-cardinality-and-modality)
- [A Review of JOINs](https://github.com/SandyRodger/LS180_database_foundations/blob/main/03_relational_data_and_joins.md#a-review-of-joins)
- [Working with Multiple Tables](https://github.com/SandyRodger/LS180_database_foundations/blob/main/03_relational_data_and_joins.md#working-with-multiple-tables)
- [Using Foreign Keys](https://github.com/SandyRodger/LS180_database_foundations/blob/main/03_relational_data_and_joins.md#using-foreign-keys)
- [One-to-Many Relationships](https://github.com/SandyRodger/LS180_database_foundations/blob/main/03_relational_data_and_joins.md#one-to-many-relationships)
- [Extracting a 1:M Relationship From Existing Data](https://github.com/SandyRodger/LS180_database_foundations/blob/main/03_relational_data_and_joins.md#extracting-a-1m-relationship-from-existing-data)
- [Assignment: SQL Fundamentals - DDL (Data Definition Language)](https://github.com/SandyRodger/LS180_database_foundations/blob/main/03_relational_data_and_joins.md#assignment-sql-fundamentals---ddl-data-definition-language)
- [Assignment: SQL Fundamentals - DML (Data Manipulation Language)](https://github.com/SandyRodger/LS180_database_foundations/blob/main/03_relational_data_and_joins.md#assignment-sql-fundamentals---dml-data-manipulation-language)
- [Many-to-Many Relationships](https://github.com/SandyRodger/LS180_database_foundations/blob/main/03_relational_data_and_joins.md#many-to-many-relationships)
- [Converting a 1:M Relationship to a M:M Relationship](https://github.com/SandyRodger/LS180_database_foundations/blob/main/03_relational_data_and_joins.md#converting-a-1m-relationship-to-a-mm-relationship)
- [Assignment: SQL Fundamentals - Many to Many](https://github.com/SandyRodger/LS180_database_foundations/blob/main/03_relational_data_and_joins.md#assignment-sql-fundamentals---many-to-many)
- [Summary](https://github.com/SandyRodger/LS180_database_foundations/blob/main/03_relational_data_and_joins.md#summary)
- [Quiz Lesson 3](https://github.com/SandyRodger/LS180_database_foundations/blob/main/03_relational_data_and_joins.md#quiz-lesson-3)

## L4: OPTIMISING SQL QUERIES

- [Optimizing SQL Queries](https://github.com/SandyRodger/LS180_database_foundations/blob/main/04_optimising_SQL_queries.md#optimizing-sql-queries)
- [What to Focus On](https://github.com/SandyRodger/LS180_database_foundations/blob/main/04_optimising_SQL_queries.md#what-to-focus-on)
- [Indexes](https://github.com/SandyRodger/LS180_database_foundations/blob/main/04_optimising_SQL_queries.md#indexes)
- [Comparing SQL Statements](https://github.com/SandyRodger/LS180_database_foundations/blob/main/04_optimising_SQL_queries.md#comparing-sql-statements)
- [Subqueries](https://github.com/SandyRodger/LS180_database_foundations/blob/main/04_optimising_SQL_queries.md#subqueries)
- [Assignment: SQL Fundamentals - Subqueries and More](https://github.com/SandyRodger/LS180_database_foundations/blob/main/04_optimising_SQL_queries.md#assignment-sql-fundamentals---subqueries-and-more)
- [Summary](https://github.com/SandyRodger/LS180_database_foundations/blob/main/04_optimising_SQL_queries.md#summary)
- [Quiz Lesson 4](https://github.com/SandyRodger/LS180_database_foundations/blob/main/04_optimising_SQL_queries.md#quiz-lesson-4)
- [Course LS180 Feedback](https://github.com/SandyRodger/LS180_database_foundations/blob/main/04_optimising_SQL_queries.md#course-ls180-feedback)

## Quizes

|  | Once | Twice | Thrice |
| :--- | :---: | :---: | :---: |
| L1 |  10/15 (66.67%) |
| L2 | 8/10 (80.0%) |
| L3 | 8/9 (88.89%) |
| L4 | 2/2 (100.0%) |

## [Introduction to SQL](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md)
- [GETTING STARTED](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#getting-started)
  - [1. Introduction](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#1-introduction)
    - [The importance of data](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#the-importance-of-data)
    - [Structured Data](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#structured-data)
    - [Spreadsheet as Database](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#spreadsheet-as-database)
    - [Relational Database Management Systems](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#relational-database-management-systems)
    - [SQL](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#sql)
    - [Why learn SQL?](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#why-learn-sql)
    - [Summary](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#summary)
  - [2. Preparations](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#2-preparations)
    - [Vocabulary](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#vocabulary)
    - [Installing PostgreSQL](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#installing-postgresql)
    - [Summary](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#summary-1)
  - [3. Interacting With PostgreSQL](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#3-interacting-with-postgresql)
    - [Interacting with a database](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#interacting-with-a-database)
    - [PostgreSQL Client Applications](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#postgresql-client-applications)
    - [The psql console](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#the-psql-console)
    - [SQL Sub-languages](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#sql-sub-languages)
    - [Summary](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#summary-2)
  - [4. SQL Basics Tutorial](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#4-sql-basics-tutorial)
    - [Set Up](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#set-up)
    - [Connect](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#connect)
    - [Select all](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#select-all)
    - [Selecting columns](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#selecting-columns)
    - [Selecting rows](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#selecting-rows)
    - [Selecting columns and rows](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#selecting-columns-and-rows)
    - [Data vs Schema](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#data-vs-schema)
    - [Summary](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#summary-3)
    - [Exercises](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#exercises)
- [YOUR FIRST DATABASE: SCHEMA](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#your-first-database-schema)
  - [5. Create and View Databases](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#5-create-and-view-databases)
    - [Create a database](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#create-a-database)
      - [Using a SQL statement](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#using-a-sql-statement)
      - [Database naming](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#database-naming)
    - [Connecting to a Database](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#connecting-to-a-database)
    - [Delete the Database](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#delete-the-database)
      - [Using dropdb](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#using-dropdb)
    - [Summary](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#summary-4)
    - [Exercises](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#exercises-1)
  - [6. Create and View Tables](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#6-create-and-view-tables)
    - [Table Creation Syntax](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#table-creation-syntax)
      - [Creating a users table](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#creating-a-users-table)
    - [Data Types](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#data-types)
    - [Keys and Constraints](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#keys-and-constraints)
    - [View the Table](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#view-the-table)
    - [Schema and DCL](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#schema-and-dcl)
    - [Summary](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#summary-5)
    - [Exercises](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#exercises-2)
  - [7. Alter a Table](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#7-alter-a-table)
    - [Alter Table Syntax](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#alter-table-syntax)
    - [Renaming a Table](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#renaming-a-table)
    - [Renaming a Column](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#renaming-a-column)
    - [Changing a Column's Datatype](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#changing-a-columns-datatype)
    - [Adding a Constraint](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#adding-a-constraint)
    - [Removing a Constraint](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#removing-a-constraint)
    - [Adding a Column](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#adding-a-column)
    - [Removing a Column](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#removing-a-column)
    - [Dropping Tables](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#dropping-tables)
    - [Summary](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#summary-6)
    - [Exercises](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#exercises-3)
- [YOUR FIRST DATABASE: DATA](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#your-first-database-data)
  - [8. Add Data with INSERT](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#8-add-data-with-insert)
    - [Data and DML](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#data-and-dml)
      - [A bit about CRUD](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#a-bit-about-crud)
    - [Setup](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#setup)
        - [Insertion Statement Syntax](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#insertion-statement-syntax)
    - [Adding Rows of Data](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#adding-rows-of-data)
      - [Rows](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#rows)
      - [Adding a single row](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#adding-a-single-row)
      - [Adding multiple rows](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#adding-multiple-rows)
    - [Constraints and Adding Data](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#constraints-and-adding-data)
      - [Default values](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#default-values)
      - [NOT NULL constraints](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#not-null-constraints)
      - [Unique constraints](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#unique-constraints)
      - [CHECK constraints](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#check-constraints)
      - [Quote marks](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#quote-marks)
    - [Summary](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#summary-7)
    - [Exercises](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#exercises-4)
  - [9. Select Queries](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#9-select-queries)
    - [Select Query Syntax](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#select-query-syntax)
      - [Identifiers and key words](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#identifiers-and-key-words)
    - [ORDER BY](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#order-by)
    - [Operators](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#operators)
      - [Comparison operators](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#comparison-operators)
      - [Logical operators](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#logical-operators)
      - [String matching operators](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#string-matching-operators)
    - [Summary](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#summary-8)
    - [Exercises](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#exercises-5)
  - [10. More on Select](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#10-more-on-select)
    - [LIMIT and OFFSET](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#limit-and-offset)
      - [Pagination](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#pagination)
    - [DISTINCT](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#distinct)
    - [Functions](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#functions)
      - [String Functions](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#string-functions)
      - [Data/time functions](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#datetime-functions)
      - [Aggregate functions](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#aggregate-functions)
    - [GROUP BY](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#group-by)
      - [Ian Austin article](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#ian-austin-article)
    - [Summary](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#summary-9)
    - [Exercises](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#exercises-6)
  - [11. Update Data in a Table](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#11-update-data-in-a-table)
    - [Updating Data](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#updating-data)
    - [Update all rows](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#update-all-rows)
    - [Update specific rows](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#update-specific-rows)
  - [Deleting Data](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#deleting-data)
    - [Delete specific rows](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#delete-specific-rows)
  - [Delete all rows](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#delete-all-rows)
  - [Update vs Delete](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#update-vs-delete)
  - [Use Caution](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#use-caution)
  - [Summary](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#summary-10)
  - [Exercises](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#exercises-7)
- [WORKING WITH MULTIPLE TABLES](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#working-with-multiple-tables)
  - [12. Create Multiple Tables](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#12-create-multiple-tables)
    - [Normalization](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#normalization)
    - [Database Design](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#database-design)
      - [Entities](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#entities)
      - [Relationships](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#relationships)
    - [Keys](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#keys)
      - [Primary keys](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#primary-keys)
      - [Foreign keys](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#foreign-keys)
    - [One-to-One](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#one-to-one)
    - [Referential Integrity](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#referential-integrity)
      - [The ON DELETE clause](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#the-on-delete-clause)
    - [One-to-Many](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#one-to-many)
    - [Many-to-Many](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#many-to-many)
    - [Summary](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#summary-11)
    - [Exercises](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#exercises-8)
  - [13. SQL Joins](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#13-sql-joins)
    - [Join Syntax](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#join-syntax)
      - [Transient tables](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#transient-tables)
    - [Types of Joins](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#types-of-joins)
      - [INNER JOIN](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#inner-join)
      - [LEFT JOIN](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#left-join)
      - [RIGHT JOIN](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#right-join)
      - [FULL JOIN](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#full-join)
      - [CROSS JOIN](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#cross-join)
    - [Multiple Joins](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#multiple-joins)
    - [Aliasing](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#aliasing)
      - [Column aliasing](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#column-aliasing)
    - [Subqueries](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#subqueries)
      - [Subquery expressions](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#subquery-expressions)
    - [Summary](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#summary-12)
    - [Exercises](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#exercises-9)
  - [CONCLUSION](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#conclusion)
  - [14. Summary and Additional Resources](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#14-summary-and-additional-resources)
    - [Summary](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#summary-13)
    - [Next Steps](https://github.com/SandyRodger/launch_school_books/blob/main/introduction_to_sql.md#next-steps)
