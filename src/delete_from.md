# DELETE FROM

* To delete data from a table, you can use the DELETE FROM statement.
* Firstly, specify the table from which you delete data.
* Secondly, use a condition to specify which rows to delete in the WHERE clause. If the row matches the condition, it will be deleted. 
* Notice that the WHERE clause is optional. If you omit it, the DELETE statement will delete all rows in the table.
Besides deleting data from a table, the DELETE statement returns the number of rows deleted.

```sql
-- Delete rows from table '[TableName]' in schema '[dbo]'
DELETE FROM [dbo].[TableName]
WHERE /* add search conditions here */
GO
```