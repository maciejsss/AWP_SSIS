# AWP
AdventureWorks DW Project

Data flow diagram
<img src="Documentation/img/flow.png">

Load data from flat files to staging DB:<br />
-Products<br />
<img src="Documentation/img/PackageProducts.png"><img src="Documentation/img/DFT_Products.png">
-Customers<br />
<img src="Documentation/img/PackageCustomers.png"><img src="Documentation/img/DFT_Customers.png">
-Calendar<br />
<img src="Documentation/img/PackageCalendar.png"><img src="Documentation/img/DFT_Calendar.png">
-Sales<br />
<img src="Documentation/img/PackageSales.png"><img src="Documentation/img/DFT_Sales.png">

<img src="Documentation/img/LoadRAWDataToStagingDB.png">

Logging inserted rows:
<img src="Documentation/img/LogsTableStagingDB.png">

Slowly changing dimesion Categories:
<img src="Documentation/img/DFT_SCDCategories.png">

Data cleansing in T-SQL:
<img src="Documentation/img/DataCleansingStagingToDB.png">

Load dimensions and facts tables from staging DB to DW:
<img src="Documentation/img/LoadDimensions.png"><img src="Documentation/img/LoadFacts.png">

Data from DW is processed to OLAP database ([AWPOLAP Project](https://github.com/maciejsss/AWPOLAP)):
<img src="Documentation/img/OLAPdb.png">

Sales cube:
<img src="Documentation/img/SalesCube.png">

All previous stages combined in one SQL job: 
<img src="Documentation/img/ETLjob.png">

SSIS execution report:
<img src="Documentation/img/ExecutionReport.png">


