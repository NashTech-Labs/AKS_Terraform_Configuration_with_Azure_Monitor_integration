# Azure Kubernetes Service (AKS) Terraform Configuration with Azure Monitor Integration

This repository contains a Terraform configuration script to provision an Azure Kubernetes Service (AKS) cluster with a default node pool and integrate it with Azure Monitor for monitoring purposes.

## Prerequisites

- **Azure Subscription:** Ensure you have an active Azure subscription.
- **Terraform Installed:** Terraform installed on your local machine.

## Configuration Files

- aks.tf and main.tf: Contains the main Terraform configuration for creating the AKS cluster, defining its properties, and integrating with Azure Monitor.

- variables.tf: Declares variables used in the Terraform configuration. Adjust these variables to customize your deployment.

- outputs.tf: Defines the output values that Terraform will display after applying the configuration, including AKS cluster details.

## Azure Monitor Integration

- main.tf:
  -- Creates a Log Analytics workspace.
  --Configures Azure Monitor for AKS by deploying the Container Insights solution.


## Usage

1. Clone this repository to your local machine.
2. Navigate to the directory containing the Terraform code.
3. Initialize the Terraform directory using the command `terraform init`.
4. Create an execution plan with `terraform plan`.
5. Apply the plan with `terraform apply`. You will be prompted to confirm the action by typing `yes`.
6. Once the infrastructure is created, you can connect to your AKS.

Remember to run `terraform destroy` when you no longer require these resources to avoid unnecessary AWS charges.
