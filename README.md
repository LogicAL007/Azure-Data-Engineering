# Azure Data Pipelines 

This project merges local tweets and satellite images as json file and sends it through http to Azure API management, processes via Azure Functions, and employs Azure Event Hub for seamless message queuing. Subsequently, an Azure Function stores data in Azure Cosmos Database, enabling real-time analytics. This holistic approach integrates diverse data sources, empowering efficient disaster response decision-making, and exemplifying data's pivotal role in disaster management innovation.

## Data Sources

[Hurricane Harvey Tweets](https://www.kaggle.com/dan195/hurricaneharvey)  from Kaggle

[Satellite Images of Hurricane Damage](https://www.kaggle.com/datasets/kmader/satellite-images-of-hurricane-damage) also from Kaggle

## Data Pipeline 

![AZURE_WEATHER_DATA](https://github.com/LogicAL007/Azure-Data-Engineering/assets/122959675/438ada62-0b27-4e42-b1b2-737df7e34399)
