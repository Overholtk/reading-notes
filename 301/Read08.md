# SQL

SQL is a language designed to allow both technical and non-technical users to query, manipulate, and transform data from a relational database

## Relational Database:
- represents a collection of related (2d) tables.
- fixed number of named columns, and any number of rows of data

## SELECT queries:
- statement which declares what data we are looking for, where to find it, & how to transform it before it is returned
- Basic SELECT:
  `SELECT column, another_column, ... FROM myTable;`
- SELECT for all columns in the table:
  `SELECT * FROM mytable;`
- WHERE clause: checks specific column values to determine whether it sould be included in results or not
  `SELECT column, another_column, ... FROM mytable`
    `WHERE condition`
      `AND/OR another_condition`
- AND or OR can be used to join logical keywords
- makes data more manageable, and speeds up the query
- DISTINCT: discards rows with duplicate values
- ORDER BY: sorts results
- LIMIT: limits the number of rows to return
- OFFSET: specifies where to begin counting

## Inserting Rows
- Schema: describes the structure of each table, and the datatypes that each column can contain
- INSERT: inserts data into a database, declares which table to write to, the columns being filled, and one or more rows of data to insert
  `INSERT INTO mytable`
  `VALULES (value_or_expr, another_value_or_expr, ...),`
- Add incomplete data to tables by specifying what column the data will go into
  `INSERT INTO mytalbe`
  ` (column, another_column, ...)`
  `VALULES (value_or_expr, another_value_or_expr, ...),`
  
## Updating Existing Data
- UPDATE statement
- Specify which table, columns, and rows to upadate, and data has to match the existing datatypes
    `UPDATE mytable`
    `SET column = value_or_expr,`
    `other_column = another_value_or_expr,`
    `...`
    `WHERE condition;`
- To avoid updating the wrong rows: write the constraint first and test it in a SELECT

## Deleting Rows
- DELETE deletes all data, or, if paired with a WHERE statement, deletes an entire row of data
  `DELETE FROM mytable`
  `WHERE condition;`
 
## Creating Tables:
- CREATE TABLE creates a new table to store data
  `CREATE TABLE IF NOT EXISTS mytable{
  column DataType TableConstraint DEFAULT default_value,
  another_column DataType TableConstraint DEFAULT default_value
  ...
  );`
  

