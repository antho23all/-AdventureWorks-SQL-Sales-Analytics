Developed SQL Server reports using the AdventureWorks database, creating SQL queries and views to analyze sales data, revenue trends, customer activity, and product performance.

## Database Download & Installation

This project uses Microsoft's AdventureWorks2022 OLTP sample database to practice SQL queries, database management, and sales analytics.

### Prerequisites
- SQL Server Express 2025
- SQL Server Management Studio (SSMS) 22
- AdventureWorks2022 backup file (`.bak`)

### Step 1: Download the AdventureWorks2022 Database

1. Visit Microsoft's official [AdventureWorks Sample Database documentation](https://learn.microsoft.com/en-us/sql/samples/adventureworks-install-configure).
2. Locate the **Download backup files** section.
3. Find the **OLTP** category.
4. Download `AdventureWorks2022.bak`.
5. Save the backup file to a folder on your computer.

### Step 2: Open SQL Server Management Studio

1. Launch SQL Server Management Studio (SSMS).
2. Connect to your SQL Server Express instance.
3. Verify that your connection is successful.
4. Locate **Databases** in Object Explorer.

### Step 3: Restore the AdventureWorks Database

1. Right-click **Databases** in Object Explorer.
2. Select **Restore Database...**
3. Under Source, select **Device**.
4. Click the three-dot button (`...`) to browse for the backup file.
5. Click **Add**.
6. Locate and select `AdventureWorks2022.bak`.
7. Click **OK** to confirm your backup selection.
8. Verify that the destination database name is `AdventureWorks2022`.
9. Review the Files section to confirm the database file locations.
10. Click **OK** to begin restoring the database.

### Step 4: Verify Database Restoration

1. Return to Object Explorer in SSMS.
2. Right-click **Databases**.
3. Select **Refresh**.
4. Locate `AdventureWorks2022` in the database list.
5. Expand the database to view its tables, views, and other database objects.

### Step 5: Verify Database Access

Open a new query window and execute:

```sql
USE AdventureWorks2022;
GO

SELECT TOP 10 *
FROM Sales.SalesOrderHeader;
GO
```

If the query executes successfully and returns results, the AdventureWorks2022 database has been successfully restored and is ready for analysis.

### Official Documentation
[Microsoft Learn – AdventureWorks Sample Databases](https://learn.microsoft.com/en-us/sql/samples/adventureworks-install-configure)

**Environment:** SQL Server Express 2025 | SSMS 22 | AdventureWorks2022
