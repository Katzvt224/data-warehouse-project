
CREATE DATATBASE AND SCHEMAS

Script purpose:

This scripts creates a new Database named 'DataWareHouse' after checking it already exits.
If the database exits, it is dropped and recreated. Additionally, the scripts sets up 3 schemas within the database: bronze, silver, 

Use Master;
Go
--Drop and recreate the database 'DataWareHouse' database
```sql
IF EXISTS (SELECT 1 FROM sys.datatbase WHERE name = 'DataWareHouse')
BEGIN 
  ALTER DATABASE DataWareHouse SET SIINGER_USER WITH ROLLBACK IMMEDIATE;
  DROP DATABASE DataWhereHouse;
END;
GO

--Create the database DataWareHouse
CREATE DATABASE DataWareHouse;
GO

USE DataWarehouse;
GO

--Create Schemas

```