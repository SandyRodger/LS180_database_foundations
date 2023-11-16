# [Relational Data and Joins](https://launchschool.com/lessons/5ae760fa/assignments)

## [What to Focus On](https://launchschool.com/lessons/5ae760fa/assignments/28d79a9d)
## [What is Relational Data?](https://launchschool.com/lessons/5ae760fa/assignments/074f64a8)
## [Database Diagrams: Levels of Schema](https://launchschool.com/lessons/5ae760fa/assignments/2f3bc8f7)
## [Database Diagrams: Cardinality and Modality](https://launchschool.com/lessons/5ae760fa/assignments/46053e3b)
## [A Review of JOINs](https://launchschool.com/lessons/5ae760fa/assignments/0391f663)
## [Working with Multiple Tables](https://launchschool.com/lessons/5ae760fa/assignments/285d837e)

2. `SELECT COUNT(*) FROM tickets;`
3. `SELECT count(distinct customer_id) FROM tickets;`
4. Wrong

```
SELECT round(count(DISTINCT customer_id)/count(DISTINCT tickets.event_id)::decimal, 2) AS percentage FROM customers INNER JOIN tickets ON customers.id = tickets.customer_id;`
```

LS answer:

```
SELECT round( COUNT(DISTINCT tickets.customer_id)
            / COUNT(DISTINCT customers.id)::decimal * 100,
            2)
       AS percent
  FROM customers
  LEFT OUTER JOIN tickets
    ON tickets.customer_id = customers.id;
```

5. Write a query that returns the name of each event and how many tickets were sold for it, in order from most popular to least popular.

```
SELECT events.name, count(tickets.id) AS popularity FROM events
LEFT OUTER JOIN tickets
ON events.id = tickets.event_id
GROUP BY events.name ORDER BY popularity DESC
;
```

I CAN DO THIS

6. Write a query that returns the user id, email address, and number of events for all customers that have purchased tickets to three events.

Almost, but not quite:

```
SELECT c.id, c.email, COUNT(t.customer_id) AS count FROM customers AS c
LEFT OUTER JOIN tickets AS t
ON c.id = t.customer_id
GROUP BY
c.id
HAVING
count(t.event_id) = 3;
;
```

LS solution:
```
SELECT customers.id, customers.email, COUNT(DISTINCT tickets.event_id)
  FROM customers
  INNER JOIN tickets
    on tickets.customer_id = customers.id
  GROUP BY customers.id
  HAVING COUNT(DISTINCT tickets.event_id) = 3;
```


## [Using Foreign Keys]()
## [One-to-Many Relationships]()
## [Extracting a 1:M Relationship From Existing Data]()
## [Assignment: SQL Fundamentals - DDL (Data Definition Language)]()
## [Assignment: SQL Fundamentals - DML (Data Manipulation Language)]()
## [Many-to-Many Relationships]()
## [Converting a 1:M Relationship to a M:M Relationship]()
## [Assignment: SQL Fundamentals - Many to Many]()
## [Summary]()
## [Quiz Lesson 3]()
