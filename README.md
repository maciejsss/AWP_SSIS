# AWP
**AdventureWorks DW Project**

## Data flow diagram:

<img src="Documentation/img/flow.png" width="700">

### Load data from flat files to staging DB:<br />
Products<br />
<img src="Documentation/img/PackageProducts.png" width="300"><img src="Documentation/img/DFT_Products.png"><br />
<br />
Customers<br />
<img src="Documentation/img/PackageCustomers.png" width="300"><img src="Documentation/img/DFT_Customers.png"><br />
<br />
Calendar<br />
<img src="Documentation/img/PackageCalendar.png" width="300"><img src="Documentation/img/DFT_Calendar.png"><br />
<br />
Sales<br />
<img src="Documentation/img/PackageSales.png" width="300"><img src="Documentation/img/DFT_Sales.png" width="500"><br />
<br />
<img src="Documentation/img/LoadRAWDataToStagingDB.png" width="300"><br />
<br />
Logging inserted rows:<br />
<img src="Documentation/img/SQL_logging.png" width="600"><br />
<img src="Documentation/img/SQL_LoggingPara.png" width="500"><br />
<img src="Documentation/img/LogsTableStagingDB.png" width="300"><br />
<br />
Load dimensions and facts tables from staging DB to DW:<br />
<img src="Documentation/img/LoadDimensions.png" width="500"><img src="Documentation/img/LoadFacts.png" width="400"><br />
<br />
Slowly changing dimesion Categories:<br />
<img src="Documentation/img/DFT_SCDCategories.png" width="400"><br />
<br />
Data cleansing in T-SQL:<br />
<img src="Documentation/img/DataCleansingStagingToDB.png" width="700"><br />
<br />

### Data from DW is processed to OLAP database ([AWP_SSAS Project](https://github.com/maciejsss/AWPOLAP)):<br />
<img src="Documentation/img/OLAPdb.png"><br />
<br />
Sales cube:<br />
<img src="Documentation/img/SalesCube.png"><br />
<br />

### All previous stages combined in one SQL job:<br />
<img src="Documentation/img/ETLjob.png" width="700"><br />
<br />

### SSIS execution report:<br />
<img src="Documentation/img/ExecutionReport.png"><br />


