
# Relational Data and Joins

## [What to Focus On](https://launchschool.com/lessons/5ae760fa/assignments/28d79a9d)

- How to work with multiple tables using `JOIN`
- SQL optional keywords
- How schemas change over time
- Make sure you spend some time with the Summary at the end of this lesson.

## [What is Relational Data?](https://launchschool.com/lessons/5ae760fa/assignments/074f64a8)

- This page explains about what is a 'relations' and what is a 'relationship'. I feel confident that I know this.

## [Database Diagrams: Levels of Schema](https://launchschool.com/lessons/5ae760fa/assignments/2f3bc8f7)

- video 

## [Database Diagrams: Cardinality and Modality](https://launchschool.com/lessons/5ae760fa/assignments/46053e3b)
## [A Review of JOINs](https://launchschool.com/lessons/5ae760fa/assignments/0391f663)
## [Working with Multiple Tables](https://launchschool.com/lessons/5ae760fa/assignments/285d837e)


2. `SELECT COUNT(*) FROM tickets;`
3. `SELECT count(distinct customer_id) FROM tickets;`
4. Write a query that determines what percentage of the customers in the database have purchased a ticket to one or more of the events. (First day I failed, second day I got it)

```
SELECT round(count(DISTINCT t.customer_id) / count(DISTINCT c.id)::decimal * 100, 2)
AS percent FROM customers AS c
LEFT OUTER JOIN tickets AS t
ON c.id = t.customer_id
;
```

5.

```
SELECT e.name, count(t.id) AS popularity FROM events AS e
LEFT OUTER JOIN tickets as t
ON t.event_id = e.id
GROUP BY e.name
ORDER BY popularity DESC;
```

6.

```
SELECT c.id, c.email, count(DISTINCT t.event_id) AS count 
FROM tickets AS t
RIGHT OUTER JOIN customers AS c
ON c.id = t.customer_id
GROUP BY c.id
HAVING count(DISTINCT t.event_id) = 3
;
```

7. This ate up a lot of my time, I got this far, which joins all the tables, but with incorrect output

```
SELECT e.name AS event, e.starts_at, sec.name, s.row, s.number AS seat
FROM events AS e
LEFT OUTER JOIN tickets AS t
ON t.event_id = t.id
LEFT OUTER JOIN seats AS s
ON s.id = t.seat_id
LEFT OUTER JOIN sections AS sec
ON s.section_id = sec.id
LEFT OUTER JOIN customers AS c
ON c.id = t.customer_id
;
```
LS solution:

```
SELECT events.name AS event,
       events.starts_at,
       sections.name AS section,
       seats.row,
       seats.number AS seat
  FROM tickets
  INNER JOIN events
    ON tickets.event_id = events.id
  INNER JOIN customers
    ON tickets.customer_id = customers.id
  INNER JOIN seats
    ON tickets.seat_id = seats.id
  INNER JOIN sections
    ON seats.section_id = sections.id
  WHERE customers.email = 'gennaro.rath@mcdermott.co';
```

The problem is, I don't know why my solution didn't work.


## [Using Foreign Keys](https://launchschool.com/lessons/5ae760fa/assignments/bb4f3ba2)

2. Update the orders table so that referential integrity will be preserved for the data between orders and products.   CORRECT

`ALTER TABLE orders ADD CONSTRAINT orders_product_id_fkey FOREIGN KEY (product_id) REFERENCES products(id);`

3. & 4. My solution (which fit the criteria and is correct):   CORRECT
```
INSERT INTO products(name) VALUES 
('small bolt'),
('small bolt'),
('large bolt');

INSERT INTO orders(product_id, quantity) VALUES
(1, 10),
(1, 25),
(3, 15);

SELECT o.quantity, p.name AS product FROM orders AS o
INNER JOIN products AS p
ON o.product_id = p.id
;
```

LS solution:

```
foreign-keys=# INSERT INTO products (name) VALUES ('small bolt');
INSERT 0 1
foreign-keys=# INSERT INTO products (name) VALUES ('large bolt');
INSERT 0 1
foreign-keys=# SELECT * FROM products;
 id |    name
----+------------
  1 | small bolt
  2 | large bolt
(2 rows)

foreign-keys=# INSERT INTO orders (product_id, quantity) VALUES (1, 10);
INSERT 0 1
foreign-keys=# INSERT INTO orders (product_id, quantity) VALUES (1, 25);
INSERT 0 1
foreign-keys=# INSERT INTO orders (product_id, quantity) VALUES (2, 15);
INSERT 0 1

SELECT quantity, name FROM orders INNER JOIN products ON orders.product_id = products.id;
```

5. Yes, it is possible, but it shouldn't be:   CORRECT

`INSERT INTO orders(quantity) VALUES (10);`

6. CORRECT

```
ALTER TABLE orders
      ALTER COLUMN product_id
      SET NOT NULL;
```

causes this error message:

`ERROR:  column "product_id" of relation "orders" contains null values`

7. `DELETE FROM orders WHERE product_id IS NULL;`  CORRECT 
## [One-to-Many Relationships]()
## [Extracting a 1:M Relationship From Existing Data]()
## [Assignment: SQL Fundamentals - DDL (Data Definition Language)]()
## [Assignment: SQL Fundamentals - DML (Data Manipulation Language)]()
## [Many-to-Many Relationships]()
## [Converting a 1:M Relationship to a M:M Relationship]()
## [Assignment: SQL Fundamentals - Many to Many]()
## [Summary]()
## [Quiz Lesson 3]()
