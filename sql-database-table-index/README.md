# An SQL Database Table Index

We all know filtering a table with `WHERE` condition can be significantly optimized and speeded up by defining suitable
indicies on a given table. E.g. we have a table `order` with a column `price` and we want to select all rerods/rows with
the `price` bigger than 1000 (i.e. `SELECT * FROM order WHERE price > 1000`). If the table `order` contains tousands or even
millions of records, this query can be greatly optimized by defining an index on the row `price`. The question is how is this 
index used if we are selecting not from one table but from multiple tables joined by a condition.

