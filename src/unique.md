# Unique constraint

Unique constraint is used to ensure no duplicate values are entered in specific columns that do not participate in a primary key.

```sql
CREATE TABLE [dbo].[GrandChild]
(
    [Id] INT NOT NULL IDENTITY PRIMARY KEY, -- Primary Key column
    [ColumnName2] NVARCHAR(50) NOT NULL,
    [ColumnName3] NVARCHAR(50) NOT NULL,
    CONSTRAINT AK_ColumnName2 UNIQUE(ColumnName2)
    -- Specify more columns here
);
GO
```

You can alter UNIQUE constraint later after table already created

```sql
ALTER TABLE Person   
ADD CONSTRAINT AK_Password UNIQUE (PasswordHash, PasswordSalt);
```