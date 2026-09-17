#Instruction

Working with ETL/SSIS

1. Open Microsoft SQL Server Manager
create database in our case financial_transactions
create tables and fill them


2. Create csv and Excel data sheet samples

3. Open Visual studio
create new project
pick type Integration Services Project
if this is not available open VS go to extensions In the search bar on the top-right, type SQL Server Integration Services Projects.
Download it, close VS and install the extension
Name the project for example Finacial Data Warehouse
On the right side on solution explorer pay attention to Connection Manager, SSIS Packages, Project PArameters and Package PArts
On the left side is SSIS toolbox
Open Control Flow (building  ETL flow) grab Data flow task from the SSIS toolbox, name it logical name like Customer Transactions. When you click double on it it takes you to Data Flow.
That's where we move data.
We need to connect to sources of data, for start to SQL source
grab OLEDB Source from Other sources on menu on the left, double click and create connection
click New, new again, then pick provider. Since it's MS SQL server pick Microsoft OLE DB Driver for SQL server.
In server name put server name like localhost
in Initial catalog pick database like our Financial_transactions. Now we have connection. Pick table like financial_transactions, and click ok
rename this source like financial transactions to know what it is

Now go to SQL server again and create datawarehouse database, for example financial_data_warehouse
create table financial_analysis
that will be our result!
