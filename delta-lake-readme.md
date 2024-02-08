# Delta Lake

Delta Lake is the default storage format for all operations on [Azure Databricks](/databrick-readme.md) for storing data and tables in the [Databricks lakehouse](/data-lakehouse-readme.md). It extends [Apache Parquet](https://www.databricks.com/glossary/what-is-parquet) data files with a file-based transaction log for [ACID transactions](https://learn.microsoft.com/en-us/azure/databricks/lakehouse/acid) and scalable metadata handling. Delta Lake is fully compatible with Apache Spark APIs having tight integration with Structured Streaming, allowing to use a single copy of data for both batch and streaming operations and providing incremental processing at scale.

## See Delta Lake in action using Azure Databrick
[Run your first ETL workload on Azure Databricks](https://learn.microsoft.com/en-us/azure/databricks/getting-started/etl-quick-start)

## Azure Databricks & Delta Lake use case

![alt txt](/images/adb-adl-usecase.png)

![alt txt](/images/delta-lake.png)

## References
* [Delta Lake](https://learn.microsoft.com/en-us/azure/databricks/delta/)
* [Azure Databricks & Delta Lake use case](https://techcommunity.microsoft.com/t5/analytics-on-azure-blog/how-to-reduce-infrastructure-costs-by-up-to-80-with-azure/ba-p/1820280)