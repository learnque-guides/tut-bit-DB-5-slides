# Alter table

The ALTER TABLE ADD statement allows you to add one or more columns to a table.

```sql
-- Add a new column '[NewColumnName]' to table '[TableName]' in schema '[dbo]'
ALTER TABLE [dbo].[TableName]
    ADD [NewColumnName] /*new_column_name*/ int /*new_column_datatype*/ NULL /*new_column_nullability*/
GO
```

The ALTER TABLE DROP statement allows you to remove one or more columns from a table.

```sql
-- Drop '[ColumnName]' from table '[TableName]' in schema '[dbo]'
ALTER TABLE [dbo].[TableName]
    DROP COLUMN [ColumnName]
GO
```

The ALTER TABLE ALTER COLUMN statement allows you to update one or more columns.

```sql
ALTER TABLE dbo.HelloWorld 
ADD Email varchar(255);

ALTER TABLE dbo.HelloWorld 
ALTER COLUMN Email varchar(300);
```