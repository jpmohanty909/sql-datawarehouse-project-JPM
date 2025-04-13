use master;
GO

--Drop and recreate the 'Datawarehouse_' database
--The below is checking if the database i.e Datawarehouse_ exists and drops it and recreates it
IF EXISTS (SELECT 1 FROM SYS.DATABASES WHERE NAME = 'Datawarehouse_')
BEGIN
	ALTER DATABASE Datawarehouse_ SET SINGLE_USER With ROLLBACK Immediate;
	DROP DATABASE Datawarehouse_;
END;
GO

--create the 'Datawarehouse_' Database
Create Database Datawarehouse_;
GO

Use Datawarehouse_;
GO

--Create Schemas
Create Schema bronze;
GO
Create Schema silver;
GO
Create Schema gold;
GO
---GO seprates batches when working with multiple SQL statements
---GO is basically used for executing the first command before going on to the next
