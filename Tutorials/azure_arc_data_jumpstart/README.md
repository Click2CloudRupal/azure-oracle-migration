# Azure Arc enabled Data Services

The below deployment options are focused on Azure Arc for Data Services. They are designed to quickly spin up Azure data services in Kubernetes that are ready to be projected in Azure Arc and ready for use with Azure native tooling.

**Disclaimer: Azure Arc for Data Services is currently in Private Preview.**

## Data Services on Azure Kubernetes Service (AKS)

If you do not yet have a Kubernetes cluster, the following examples walk through creating an AKS cluster to simulate an "on-premises" cluster and deploy Azure Arc Data Services on top of it.

* [Azure Arc Data Controller Vanilla Deployment on AKS using Azure ARM template](docs/aks_dc_vanilla_arm_template.md)

* [Azure PostgreSQL Hyperscale (Citus) Deployment on AKS](../azure_arc_postgres_hyperscale/README.md)