# Azure ETL Pipeline for COVID-19 Data

## Overview

This project demonstrates an end-to-end ETL pipeline using Azure services to fetch, transform, and load COVID-19 data from Azure Blob Storage and HTTP links. The processed data is stored in Azure Data Lake Storage Gen2 and Azure SQL Database. The pipeline is automated with both manual and automated build approaches, and the infrastructure is managed using Azure Resource Manager (ARM) templates. Azure DevOps is used for continuous integration and deployment, and Azure Monitor and Log Analytics are used for monitoring the pipelines. Data visualization is performed using Power BI.

## Architecture

![Pipeline Architecture](path_to_your_architecture_diagram.png)

## Features

- **Data Ingestion**:
  - Fetch data from Azure Blob Storage and HTTP links.
  
- **Data Transformation and Loading**:
  - ETL pipelines to process and transform data.
  - Store transformed data in Azure Data Lake Storage Gen2.
  - Store transformed data in Azure SQL Database.
  
- **Automation**:
  - Manual Build/Publish Approach: Manual publishing of the pipeline.
  - Automated Build Approach: Fully automated pipeline with no manual intervention.
  
- **Infrastructure Provisioning**:
  - Use of ARM templates to provision Azure resources.
  
- **Security**:
  - Use of Azure Key Vault to securely store credentials.
  
- **Monitoring**:
  - Azure Monitor and Log Analytics for pipeline monitoring and logging.
  
- **Visualization**:
  - Integration with Power BI for data visualization.

## Prerequisites

- Azure Subscription
- Azure DevOps Account
- Power BI Account

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/azure-etl-pipeline-covid19.git
cd azure-etl-pipeline-covid19
```

### 2. Set Up Azure Resources

Provision the required Azure resources using ARM templates.

```bash
az deployment group create --resource-group yourResourceGroup --template-file azuredeploy.json
```

### 3. Configure Azure Key Vault

Store your credentials and secrets in Azure Key Vault.

### 4. Set Up Azure DevOps Pipelines

Configure your Azure DevOps pipelines for CI/CD.

- **Manual Build/Publish Pipeline**: Set up the pipeline to manually trigger builds.
- **Automated Build Pipeline**: Configure the pipeline for automated builds without manual intervention.

### 5. Run the ETL Pipelines

- Trigger the ETL pipelines through Azure Data Factory.
- Monitor the pipeline execution using Azure Monitor and Log Analytics.

### 6. Visualize Data in Power BI

Connect Power BI to your Azure SQL Database or Data Lake Storage to visualize the processed data.

## Monitoring

- **Azure Monitor**: Track the health and performance of your ETL pipelines.
- **Log Analytics**: Analyze logs and metrics to troubleshoot issues.

## Automation Scripts

- **ARM Templates**: Automate infrastructure provisioning.
- **Pipeline Scripts**: Automate data processing tasks.
