# Azure Arc enabled Kubernetes

The below deployment options are focused on Azure Arc for Kubernetes. They are designed to quickly spin up a Kubernetes cluster that is ready to be projected in Azure Arc and ready for use with Azure native tooling. 

## General

This example demonstrates how to connect an existing Kubernetes cluster to Arc. It assumes you already have a cluster ready to work with.

* [Connect an existing Kubernetes cluster to Azure Arc](docs/onboard_k8s.md)

### Azure Kubernetes Service (AKS)

If you do not yet have a Kubernetes cluster, the following examples walk through creating an AKS cluster to simulate an "on-premises" cluster. Examples are provided for deploying with either Terraform or with an ARM template.

* [Deploy AKS cluster and connect it to Azure Arc using Azure ARM template](docs/aks_arm_template.md)

* [Deploy AKS cluster and connect it to Azure Arc using Terraform](docs/aks_terraform.md)

### Amazon Elastic Kubernetes Service (EKS)

This example uses Terraform to deploy an EKS cluster on AWS and connect it to Azure with Azure Arc.

* [Deploy EKS cluster and connect it to Azure Arc using Terraform](docs/eks_terraform.md)

### Google Kubernetes Engine (GKE)

This example uses Terraform to deploy a GKE cluster on Google Cloud and connect it to Azure with Azure Arc.

* [Deploy GKE cluster and connect it to Azure Arc using Terraform](docs/gke_terraform.md)

### Rancher k3s

These examples deploy [Rancher k3s](https://github.com/rancher/k3s) on an Azure VM or VMware and onboards the cluster with Azure Arc. 

* [Deploy Rancher k3s on an Azure VM and connect it to Azure Arc using Azure ARM template](docs/rancher_k3s_azure_arm_template.md)

* [Deploy Rancher k3s on an Azure VM and connect it to Azure Arc using Terraform](docs/rancher_k3s_azure_terraform.md)

* [Deploy Rancher k3s on a VMware vSphere VM and connect it to Azure Arc using Terraform](docs/rancher_k3s_vmware_terraform.md)

### Azure Red Hat OpenShift (ARO) V4

Azure Arc can also support Azure Red Hat OpenShift (ARO). This example uses Terraform to deploy a new ARO cluster and onboards it to Azure with Azure Arc.

* [Deploy Azure Redhat Openshift Cluster and connect it to Azure Arc using automation](docs/aro_script.md)

### Azure Arc for Kubernetes - Day-2 Scenarios & Use-Cases

Once you have Kubernetes clusters projected into Azure with Azure Arc, you can start to use native Azure tooling to manage the clusters as native Azure resources. The following guides show examples of using Azure management tools such as Azure Monitor, GitOps configurations, and Azure Policy.

#### AKS

* [Deploy GitOps configurations and perform basic GitOps flow on AKS as an Azure Arc Connected Cluster](docs/aks_gitops_basic.md)

* [Deploy GitOps configurations and perform Helm-based GitOps flow on AKS as an Azure Arc Connected Cluster](docs/aks_gitops_helm.md)

* [Integrate Azure Monitor for Containers with AKS as an Azure Arc Connected Cluster](docs/aks_monitor.md)

* [Apply GitOps configurations on AKS as an Azure Arc Connected Cluster using Azure Policy for Kubernetes ](docs/aks_policy.md)

#### GKE

* [Deploy GitOps configurations and perform basic GitOps flow on GKE as an Azure Arc Connected Cluster](docs/gke_gitops_basic.md)

* [Deploy GitOps configurations and perform Helm-based GitOps flow on GKE as an Azure Arc Connected Cluster](docs/gke_gitops_helm.md)

* [Integrate Azure Monitor for Containers with GKE as an Azure Arc Connected Cluster](docs/gke_monitor.md)

* [Apply GitOps configurations on GKE as an Azure Arc Connected Cluster using Azure Policy for Kubernetes ](docs/gke_policy.md)