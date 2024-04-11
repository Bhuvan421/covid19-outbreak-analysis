# covid19-outbreak-analysis

Data Source:
``https://www.ecdc.europa.eu/en/covid-19/data``
* Built a data integration pipeline that triggers every midnight at 12am and copies data (cases, deaths, hospital admissions, testing) from ECDC website using http connector into the azure data lake.
* Implemented multiple data transformation pipelines using Azure Data Flow, HDInsight using Hive and Azure Databricks using PySpark and stored the data in Azure SQL database for downstream analytics.
* Published the data to Microsoft PowerBI and built auto refreshing dynamic dashboards.
* Created alerts, monitored the data flow using Azure Monitor and Log Analytics, and built error monitoring workbooks using Kusto Query Language (KQL) to analyze trigger/pipeline runs, memory/compute usage by each resource and so on.
* Architected continuous integration, delivery, and monitoring (CI/CD) throughout the project using Npm package build pipeline, pre/post deployment scripts in release pipelines using Azure DevOps/Git and automated the publish stage (ARM generation) for continuous deployment in test and prod stages, removing the manual publish/commit of changes. 

#### Tech Stack used:

```
1. Azure DevOps (CI/CD)
2. Azure Data Factory
3. Azure Data Lake Gen 2
4. Azure Data Flows
5. HDInsight (Hive)
6. Azure Databricks (PySpark, Spark SQL)
7. Azure SQL database (T-SQL - Transact-SQL)
8. Azure Monitor/Log Analytics (KQL - Kusto Query Language)
9. Microsoft PowerBI
```

One of the transformation pipeline:

![alt text](hospital-data-transformation-pipeline.png)
