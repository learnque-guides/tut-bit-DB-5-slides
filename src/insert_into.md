# INSERT INTO

* The INSERT INTO statement allows you to insert one or more rows into a table.
* First, specify the table name and a list of comma-separated column names inside parentheses after the INSERT INTO clause.
* Then, put a comma-separated list of values of the corresponding columns inside the parentheses following the VALUES keyword.

```sql
-- Insert rows into table 'TableName' in schema '[dbo]'
INSERT INTO [dbo].[TableName]
( -- Columns to insert data into
 [ColumnName1], [ColumnName2], [ColumnName3]
)
VALUES
( -- First row: values for the columns in the list above
 ColumnValue1, ColumnValue2, ColumnValue3
);
GO
```

It is possible to insert multiple rows

```sql
-- Insert rows into table 'TableName' in schema '[dbo]'
INSERT INTO [dbo].[TableName]
( -- Columns to insert data into
 [ColumnName1], [ColumnName2], [ColumnName3]
)
VALUES
( -- First row: values for the columns in the list above
 ColumnValue1, ColumnValue2, ColumnValue3
),
( -- Second row: values for the columns in the list above
 ColumnValue1, ColumnValue2, ColumnValue3
)
-- Add more rows here
GO
```