# SQL

## Querying data in the database 
A relational database represents a collection of related (two-dimensional) tables.

The database *schema* is what describes the structure of the table.  Having specific data types is what allows a database to efficiently store millions or billions of rows.

To retrieve data from a database, we need to write SELECT statements, which are referred to as *queries*.  Quieries are statements that declares what data we are looking for, where to find it in the database, and how to transform it before its returned. 

To select all columns from a table, you would use:
```
SELECT *
FROM mytable
```

To filter data, use the `WHERE` keyword:
```
SELECT column, another_column, …
FROM mytable
WHERE condition
    AND/OR another_condition
    AND/OR …;
```

You can sort using `ASCEND` or `DESCEND`, use the keyword `LIMIT` to reduce the number of rows returned, or use the keyword `OFFSET` to specify where to begin counting rows. 

```
SELECT column, another_column, …
FROM mytable
WHERE condition(s)
ORDER BY column ASC/DESC
LIMIT num_limit OFFSET num_offset;
```

Note: the keyword `DISTINCT` blindly removes duplicates 

## Inserting data into the database

To insert data into the database, use the `INSERT`:
```
INSERT INTO boxoffice
(movie_id, rating, sales_in_millions)
VALUES (1, 9.9, 283742034 / 1000000);
```
Update data using `UPDATE`:
```
UPDATE mytable
SET column = value_or_expr, 
    other_column = another_value_or_expr, 
    …
WHERE condition;
```

Delete data using `DELETE`:
```
DELETE FROM mytable
WHERE condition;
```
If you leave out the `WHERE` constraint, all rows are removed

Create table:
``` 
CREATE TABLE IF NOT EXISTS mytable (
    column DataType TableConstraint DEFAULT default_value,
    another_column DataType TableConstraint DEFAULT default_value,
);
```

Alter table:
```
ALTER TABLE mytable
ADD column DataType OptionalTableConstraint 
    DEFAULT default_value;
```