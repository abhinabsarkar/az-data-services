# Azure Databricks

Azure Databricks is a fully `managed service` provided by Microsoft that offers the capabilities to create an open [Data Lakehouse](/data-lakehouse-readme.md) within the Azure cloud environment. It offers data processing platform [(ETL/ELT)](https://www.jamesserra.com/archive/2012/01/difference-between-etl-and-elt/), [building data pipelines](https://www.projectpro.io/article/data-pipeline-definition-architecture-examples/528#mcetoc_1gl9sqrc84m), & cloud-based analytics for various data-related task.

![alt txt](/images/azure-databricks.png)

Data engineering use cases where Azure Databricks can be used.
* Data Ingestion: handle ingestion of the large volume of data from various sources such as data lakes, databases, streaming platforms, or IoT devices. 
* Building Interactive Dashboards and Visualizations: create interactive dashboards and visualizations using tools like Apache Spark, which enables efficient data processing and analysis at scale.
* Compute Management: manage the compute resources required for data processing tasks. It can scale up or down based on demand and provides autoscaling capabilities for efficient resource utilization.
* Data Discovery, Exploration, and Annotation: a collaborative environment for data scientists and analysts to explore and discover insights from data.  
* Machine Learning Modeling and Tracking: enables data scientists to build, train, and deploy machine learning models at scale, while also providing tools for model tracking and experimentation.
* Executing SQL Queries: provides SQL interface for data exploration and analysis, for analysts and data scientists to work with data.

![alt txt](/images/analytics-architecture-az-databricks.png)

## Architecture
Azure Databricks consists of the following key components:
* Workspace: The workspace is the central hub for all the users working on Azure Databricks. It provides a collaborative environment where teams can create and manage notebooks, libraries, and data. 
* Notebooks: Azure databricks notebooks are interactive web-based interfaces that allow users to create and execute code, visualize data, and document their analysis. 
* Clusters: Clusters are the computational units in Azure Databricks. They are responsible for executing the code written in notebooks. 
* Jobs: Jobs in Azure Databricks enable users to schedule and automate the execution of notebooks or scripts. Users can define job parameters, set scheduling intervals, and monitor the job status through the Azure portal or REST APIs.
* Libraries: Libraries are reusable packages or dependencies that can be installed on the clusters to extend the functionality of Azure Databricks.
* Data Sources: Azure Databricks supports various data sources, both structured and unstructured, including Azure Blob Storage, Azure Data Lake Store, SQL data warehouse, and more. 

Azure Databricks uses a control plane (managed by Microsoft) and a data plane (managed by customer) to ensure secure and efficient data processing. Azure Databricks manages the control plane and consists of backend services hosted in its Azure account. It stores and encrypts notebook commands and workspace configurations. On the other hand, the data plane is managed by your Azure account and is where your data resides. This is also where data processing takes place. 

![alt text](/images/Microsoft_Azure_Databricks_Architecture.png)

The above architecture diagram represents the typical structure and flow of data in Azure Databricks. While custom configurations can affect the architecture, such as deploying the workspace to your virtual network, the control and data planes remain fundamental.

Your data is stored in your Azure account in the data plane and your data sources, giving you complete control and ownership. Job results are stored in your storage account. Interactive notebook results are stored in a combination of the control plane (partial results for UI presentation) and your Azure storage.

## See Azure Databrick in action
[Run your first ETL workload on Azure Databricks](https://learn.microsoft.com/en-us/azure/databricks/getting-started/etl-quick-start)

## References
* [Azure Databricks](https://www.projectpro.io/article/azure-databricks/865)
* [Azure Databricks Fundamentals - video](https://vimeo.com/505582284)
* [Databricks architecture](https://learn.microsoft.com/en-us/azure/databricks/getting-started/overview)
