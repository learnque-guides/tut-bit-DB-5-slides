# Foreign key

* A foreign key is a column or group of columns in a table that links to a column or group of columns in another table. The foreign key places constraints in the related tables, so database can maintain referential integrity.
* The table containing the foreign key is called the child table, and the referenced table is the parent table.
* Typically, the foreign key columns of the child table often refer to the primary key columns of the parent table.

```sql
CREATE TABLE [dbo].[Trailers] (
    [Id] INT IDENTITY(1,1) NOT NULL CONSTRAINT PK_Trailer_Id PRIMARY KEY NONCLUSTERED(Id),
    [Number] VARCHAR(50) NOT NULL,
    [CarId] INT CONSTRAINT FK_Car_Id FOREIGN KEY REFERENCES [dbo].[Cars](Id)
);
```

* A table can have more than one foreign key where each foreign key references to a primary key of the different parent tables.
* Once a foreign key constraint is in place, the foreign key columns from the child table must have the corresponding row in the parent key columns of the parent table or values in these foreign key columns must be NULL.
