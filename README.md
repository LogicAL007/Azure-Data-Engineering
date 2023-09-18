# Azure Data Pipelines 

This project merges local tweets and satellite images as json file and sends it through http to Azure API management, processes via Azure Functions, and employs Azure Event Hub for seamless message queuing. Subsequently, an Azure Function stores data in Azure Cosmos Database, enabling real-time analytics. This holistic approach integrates diverse data sources, empowering efficient disaster response decision-making, and exemplifying data's pivotal role in disaster management innovation.

## Data Sources

[Hurricane Harvey Tweets](https://www.kaggle.com/dan195/hurricaneharvey)  from Kaggle

[Satellite Images of Hurricane Damage](https://www.kaggle.com/datasets/kmader/satellite-images-of-hurricane-damage) also from Kaggle

## Data Pipeline 

![AZURE_WEATHER_DATA](https://github.com/LogicAL007/Azure-Data-Engineering/assets/122959675/438ada62-0b27-4e42-b1b2-737df7e34399)


## Tools
### Connect

- [Azure API Management](https://docs.microsoft.com/en-us/azure/api-management/api-management-key-concepts)
  >>API Management (APIM) is a solution that establishes modern and consistent API gateways for existing backend services. It enables organizations to publish, manage, and monitor APIs securely, offering features like authentication, rate limiting, and analytics. APIM streamlines the process of exposing backend services as APIs while maintaining control and security, allowing effective API governance and performance management.
  
### Buffer

- [Azure Event Hubs](https://docs.microsoft.com/en-us/azure/event-hubs/event-hubs-about)
  >>Azure Event Hubs is a robust big data streaming platform and event ingestion service provided by Microsoft Azure. With the capability to handle massive throughput, it can efficiently receive and process millions of events per second. Event Hub serves as a scalable entry point for ingesting data from various sources. Data sent to an Event Hub can be transformed, processed, and stored by utilizing real-time analytics solutions or through batch processing and storage adapters. This makes it an integral component for building scalable and real-time data processing pipelines in various applications. 

### Processing

- [Azure Function](https://docs.microsoft.com/en-us/azure/azure-functions/functions-overview)
  >>Azure Functions is a serverless computing solution offered by Microsoft Azure, designed to minimize the amount of code you need to write, reduce infrastructure management tasks, and optimize costs. With Azure Functions, you focus on writing the code that performs specific tasks without the need to concern yourself with server provisioning and maintenance. The cloud infrastructure automatically provides the necessary resources to ensure your applications run smoothly, allowing you to concentrate on your application's logic rather than infrastructure concerns. This serverless approach simplifies development and resource management, offering an efficient way to build and deploy applications.

### Storage

- [Azure Blob Storage](https://docs.microsoft.com/en-us/azure/storage/blobs/storage-blobs-introduction) 
  >> Azure Blob Storage serves as Microsoft's cloud-based object storage solution. Specifically optimized for the storage of vast quantities of unstructured data, it is ideal for handling data that doesn't conform to a fixed data model or structure, including text, binary files, images, and more. This flexible storage solution accommodates various data types, allowing developers and organizations to efficiently manage and access unstructured data at scale within the Azure cloud environment.

- [Azure Cosmos DB](https://docs.microsoft.com/en-us/azure/cosmos-db/introduction) - SQL Core - Document Store
  >> Azure Cosmos DB is a comprehensive, fully managed NoSQL database service tailored for contemporary application development. Its standout features include single-digit millisecond response times, ensuring swift data retrieval and manipulation regardless of database size. The database's automatic and instant scalability guarantees that performance remains consistent as data grows. Azure Cosmos DB offers robust business continuity through SLA-backed availability and enterprise-grade security, making it a reliable choice for applications that demand high-speed, globally distributed, and secure data storage and retrieval.

### Visualization
