# Create table

* The CREATE TABLE instruction allows you to create a new table in the database.
* When creating a new table you need to provide the table name along with its column names, column definition and constraints.
* The column definition refers to the column data type and properties.

Simple syntax:

```sql
-- Create a new table called '[TableName]' in schema '[dbo]'
-- Drop the table if it already exists
IF OBJECT_ID('[dbo].[TableName]', 'U') IS NOT NULL
DROP TABLE [dbo].[TableName]
GO
-- Create the table in the specified schema
CREATE TABLE [dbo].[TableName]
(
    [Id] INT NOT NULL PRIMARY KEY, -- Primary Key column
    [ColumnName2] NVARCHAR(50) NOT NULL,
    [ColumnName3] NVARCHAR(50) NOT NULL
    -- Specify more columns here
);
GO
```
