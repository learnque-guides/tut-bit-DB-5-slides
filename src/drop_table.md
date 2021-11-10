# Drop table

The DROP TABLE statement removes a table and its data permanently from the database.

In MySQL, you can also remove multiple tables using a single DROP TABLE statement, each table is separated by a comma, but not sure if it possible to do in T-SQL

```sql 
DROP TABLE [ IF EXISTS ] { database_name.schema_name.table_name | schema_name.table_name | table_name } [ ,...n ]  
[ ; ] 
```

Example

```sql
CREATE TABLE T1 (Col1 INT);  
GO  
DROP TABLE IF EXISTS T1;  
GO
```
