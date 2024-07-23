# Project-15-SQL-commands-PostgreSQL-
These are tasks given in Patika Java Intermediate course.

The database is the PostgreSQL's given dvdrental database.

* What is the average value of the rental_rate column in the film table?
* How many films in the film table start with the letter 'C'?
* What is the duration (length) of the longest film in the film table with a rental_rate of 0.99?
* How many distinct replacement_cost values are there for films in the film table that are longer than 150 minutes?

## Answers 
- 2.98
- 1000
- 184
- 21


The Queries :

``` 
-- Task1
SELECT AVG(rental_rate) FROM film ;


-- Task 2
SELECT COUNT(title LIKE 'C%') FROM film ;


-- Task 3
SELECT MAX(length) FROM film 
WHERE rental_rate = 0.99 ;

-- Task 4
SELECT COUNT(DISTINCT replacement_cost) FROM film 
WHERE length > 150 ;


```