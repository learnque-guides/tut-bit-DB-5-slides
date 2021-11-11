# UPDATE


* The UPDATE statement modifies existing data in a table.
* Firstly, specify the name of the table that you want to update data after the UPDATE keyword.
* Secondly, specify which column you want to update and the new value in the SET clause.
* Thirdly, specify which rows to be updated using a condition in the WHERE clause. The WHERE clause is optional. If you omit it, the UPDATE statement will update all rows in the table.


```sql
-- Update rows in table '[TableName]' in schema '[dbo]'
UPDATE [dbo].[TableName]
SET
    [ColumnName1] = ColumnValue1,
    [ColumnName2] = ColumnValue2
    -- Add more columns and values here
WHERE /* add search conditions here */
GO
```