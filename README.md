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
