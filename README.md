# AWP
**AdventureWorks DW Project**

## Data flow diagram:

<img src="Documentation/img/flow.png">

### Load data from flat files to staging DB:<br />
Products<br />
<img src="Documentation/img/PackageProducts.png"><img src="Documentation/img/DFT_Products.png"><br />
<br />
Customers<br />
<img src="Documentation/img/PackageCustomers.png"><img src="Documentation/img/DFT_Customers.png"><br />
<br />
Calendar<br />
<img src="Documentation/img/PackageCalendar.png"><img src="Documentation/img/DFT_Calendar.png"><br />
<br />
Sales<br />
<img src="Documentation/img/PackageSales.png"><img src="Documentation/img/DFT_Sales.png"><br />
<br />
<img src="Documentation/img/LoadRAWDataToStagingDB.png"><br />
<br />
Logging inserted rows:<br />
<img src="Documentation/img/SQL_logging.png"><br />
<img src="Documentation/img/SQL_LoggingPara.png"><br />
<img src="Documentation/img/LogsTableStagingDB.png"><br />
<br />
Load dimensions and facts tables from staging DB to DW:<br />
<img src="Documentation/img/LoadDimensions.png"><img src="Documentation/img/LoadFacts.png"><br />
<br />
Slowly changing dimesion Categories:<br />
<img src="Documentation/img/DFT_SCDCategories.png"><br />
<br />
Data cleansing in T-SQL:<br />
<img src="Documentation/img/DataCleansingStagingToDB.png"><br />
<br />

### Data from DW is processed to OLAP database ([AWPOLAP Project](https://github.com/maciejsss/AWPOLAP)):<br />
<img src="Documentation/img/OLAPdb.png"><br />
<br />
Sales cube:<br />
<img src="Documentation/img/SalesCube.png"><br />
<br />

### All previous stages combined in one SQL job:<br />
<img src="Documentation/img/ETLjob.png"><br />
<br />

### SSIS execution report:<br />
<img src="Documentation/img/ExecutionReport.png"><br />


