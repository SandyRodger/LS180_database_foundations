# [Schema, data and SQL](https://launchschool.com/lessons/a1779fd2/assignments)

## [What to Focus On](https://launchschool.com/lessons/a1779fd2/assignments/71713836)

- 

## [The SQL Language](https://launchschool.com/lessons/a1779fd2/assignments/7673d9a9)

- SQL is declarative. It says what it means.
- As with most languages the implementation of an SQL search query is hidden from the user. But if you know a little about it you can tweak for optimisaton.
- SQL is 3 sub-languages:
  - Data Definition Language: create and modify schema, ie
    - `CREATE TABLE`
    - `ALTER TABLE`
    - `ADD COLUMN`
  - Data Manipulation Language: retrieve and modify data, ie
    - `SELECT`
    - `INSERT`
    - `UPDATE`
    - `DELETE`
  - Data Control Language: controls the rights and "access roles" of the user. We don't go into this much on this course. Usually it just means being granted 'read-only' access and only being able to use `SELECT` statements.
 
### Syntax

- ` SELECT (1 + 4) * 6;`

### Practice problems:

1. Declarative.
   - Their answer: Special purpose language. The special purpose is interacting with relational databases.
2. DDL, DML, DCL.
3. 
```
'canoe'
'a long road' 
'weren''t'
'"No way!"'
```
4. ||
5. `lower('InPut')`
6. `t` `f`
7. `SELECT round((4 * 3.14159265359) * (26.3 * 26.3));` (8692)
  - Their answer: `SELECT trunc(4 * pi() * 26.3 ^ 2);`

[Assignment: SQL Fundamentals - DML, DDL, and DCL](https://launchschool.com/exercise_sets/eac14e3d)

1. The other 2 sublanguages are
- DDL, ie
  - CREATE TABLE
  - ALTER TABLE
- DML ie
  - INSERT
  - UPDATE

2. DML because it is selecting the information, but not changing it.
3. CREATE TABLE is DDL
4. DDL
5. DML
6. DML
7. None. Trick question.
8. DML
9. DDL
10. DDL

## [SQL Style Guide](https://launchschool.com/lessons/a1779fd2/assignments/dc780258)

- We don't bother with this here, but [here it is](https://www.sqlstyle.guide).

## [PostgreSQL Data Types](https://launchschool.com/lessons/a1779fd2/assignments/834815910)

- There are a whole bunch of data types, from moneys and geometric shapes, but we look at these guys:
  - varchar
  - text
  - integer
  - real
  - decimal
  - timestamp
  - date
  - boolean
 
### NULL

- When you ask SQL if NULL is NULL, it says, 'NULL', not 'true'
- That's why we have `IS NULL` and `IS NOT NULL`.

### Practice problems:

1. `text` is unlimited, where `varchar` takes an argument that limits how long it can be.
2. `integer` is a whole number, `decimal` takes an argument saying how precise it should be, `real` is like unlimited `decimal`
3. between -2147483648 and +2147483647.
4. `timestamp` = date and time, `date` is only date.
5. No, but you can with `timestamp with time zone` or `timestamptz`

## [Working with a Single Table](https://launchschool.com/lessons/a1779fd2/assignments/4f4df8a4)

1.
```
CREATE TABLE people (
  name varchar(50),
  age integer,
  occupation varchar(50)
);

2.

INSERT INTO people (name, age, occupation) VALUES 
('Abby', 34, 'biologist'), 
('Mu''nisah', 26, NULL), 
('Mirabelle', 40, 'contractor');
```

3.

```
SELECT * FROM people WHERE occupation IS NULL;
SELECT * FROM people WHERE age < 27;
SELECT name, age, occupation FROM people WHERE name LIKE '%sah%';
```

4.

```
CREATE TABLE birds (
  name varchar(50),
  length decimal(3,1),
  wingspan decimal(3,1),
  family varchar(30)
  extinct boolean
);
```

5.
```
INSERT INTO birds VALUES 
('Spotted Towhee',	21.6,	26.7,	'Emberizidae',	false),
('American Robin',	25.5,	36.0,	'Turdidae',	false),
('Greater Koa Finch',	19.0,	24.0,	'Fringillidae',	true),
('Carolina Parakeet',	33.0,	55.8,	'Psittacidae',	true),
('Common Kestrel', 35.5, 73.5, 'Falconidae', false);
```
6.
```
SELECT name, family FROM birds WHERE extinct = false ORDER BY length DESC;
```

7.
```
SELECT avg(wingspan), min(wingspan), max(wingspan) FROM birds;
```
8.
```
CREATE TABLE menu_items (
  item varchar(50),
  prep_time integer,
  ingredient_cost decimal(3,2),
  sales integer,
  menu_price decimal(4,2)
);
```

9.
```
INSERT INTO menu_items VALUES 
('omelette',	10,	1.50,	182,	7.99),
('tacos',	5,	2.00,	254,	8.99),
('oatmeal',	1,	0.50,	79,	5.99);
```

10. I peaked
```
SELECT item, menu_price - ingredient_cost AS profit FROM menu_items ORDER BY profit DESC LIMIT 1;
```

11.
```
SELECT item, menu_price, ingredient_cost, 
round((13.00/60 * prep_time),2) AS labor, 
round((menu_price - ingredient_cost) - (13.00/60 * prep_time), 2) AS profit
FROM menu_items ORDER BY profit DESC;
```

[Loading Database Dumps](https://launchschool.com/lessons/a1779fd2/assignments/fa05a889)

1.
- The file deletes any existing `film` table, then creates one and adds three entries.
- The output looks like this:
```
NOTICE:  table "films" does not exist, skipping
DROP TABLE
CREATE TABLE
INSERT 0 1
INSERT 0 1
INSERT 0 1
```
2. `SELECT * FROM films;`
3. 'SELECT * FROM films WHERE length(title) > 12;'
4. 
```
ALTER TABLE films ADD COLUMN director varchar(255);
ALTER TABLE films ADD COLUMN duration integer;
```

5. 
```
UPDATE films SET director = 'John McTiernan', duration = 132 WHERE title = 'Die Hard';
UPDATE films SET director = 'Michael Curtiz', duration = 102 WHERE title = 'Casablanca';
UPDATE films SET director = 'Francis Ford Coppola', duration = 113 WHERE title = 'The Conversation';
```

6. 
```
INSERT INTO films(title, year, genre, director, duration) VALUES 
('1984', 1956,	'scifi',	'Michael Anderson',	90),
('Tinker Tailor Soldier Spy',	2011,	'espionage',	'Tomas Alfredson',	127),
('The Birdcage',	1996,	'comedy',	'Mike Nichols',	118);
```

7.
```
SELECT title, 2023 - year AS age FROM films ORDER BY age ASC;
```

8.
```
SELECT title, duration FROM films WHERE duration > 120 ORDER BY duration DESC;
```

9. `SELECT title FROM films ORDER BY duration DESC LIMIT 1;`

## [More Single Table Queries](https://launchschool.com/lessons/a1779fd2/assignments/e5d34504)

1. `createdb residents`
2. `psql -d residents < residents_with_data.sql`
3. `SELECT state, COUNT(id) FROM people GROUP BY state ORDER BY count DESC LIMIT 10;`  (I peaked)
4.   (I peaked)

```
SELECT substr(email, strpos(email, '@') + 1) as domain,
         COUNT(id)
  FROM people
  GROUP BY domain
  ORDER BY count DESC;
```

5. `DELETE FROM people WHERE id = 3399;`
6. 'DELETE FROM people WHERE state = 'CA';'
7. 


9	NOT NULL and Default Values	Not completed
10	More Constraints	Not completed
11	Using Keys	Not completed
12	GROUP BY and Aggregate Functions	Not completed
13	How PostgreSQL Executes Queries	Not completed
14	Table and Column Aliases	Not completed
15	Summary	Not completed
16	Quiz Lesson 2
