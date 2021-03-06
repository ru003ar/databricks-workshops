## 1.0. About
This is a workshop showcasing most aspects of an end to end Azure IoT solution as referenced [below](decks/ReferenceArchitecture.pptx).<br>
![ReferenceArchitecture](images/ReferenceArchitecture.png)

It covers:<br> 
1.  simulated device telemetry publishing to Azure IoT hub, 
2.  device telemetry from #1, sourced to Kafka on HDInsight through KafkaConnect<BR> 
3.  telemetry ingestion via Spark structured streaming on Azure Databricks<BR>
4.  telemetry persistence into Azure Cosmos DB<br>
5.  reports generated in Azure Databricks, persisted to an RDBMS<br>
6.  live device stats dashboard<br>
  
The workshop solution leverages multiple Azure PaaS services - <BR>
  - Azure IoT Hub (Scalable IoT PaaS) <BR>
  - Azure HDInsight Kafka (Scalable streaming pub-sub) - Hortonworks Kafka PaaS <BR>
  - Azure Cosmos DB (NoSQL PaaS)  - for device registry and streaming device telemetry persistent store <BR>
  - Azure Databricks (Spark PaaS) - for distributed processing <BR>
  - Azure SQL Database (SQL Server PaaS) - for reporting serve layer <BR>
  - Power BI (BI SaaS) <BR>
  
  
## 2.0. Get started
### 2.0.1. Provision Azure resources
1.  [Device Telemetry Simulator & Azure IoT Hub](docs/Provisioning-1-AzureIoT.md)
2.  [Azure resource group and virtual network](docs/Provisioning-2-Common.md)
3.  [Azure Cosmos DB](docs/Provisioning-3-AzureCosmosDB.md)
4.  [Azure Databricks](docs/Provisioning-4-AzureDatabricks.md)
5.  [HDInsight Kafka](Provisioning-5-Kafka.md)
6.  [KafkaConnect Azure IoT Hub Source Connector](Provisioning-6-KafkaConnect.md)

## 3.0. Start the services provisioned
1.  [Start the components](docs/Provisioning-7-StartTheComponents.md)

## 4.0. Workshop
### 4.0.1. Setup
##### 4.0.1.1. Mount blob storage

### 4.0.2. Stuctured streaming from Kafka to Azure Cosmos DB telemetry state store (OLTP store)

### 4.0.3. Stuctured streaming from Kafka to Databricks Delta (analytics store)
