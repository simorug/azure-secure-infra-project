# Azure Secure Infrastructure Project

## Overview
This project demonstrates the implementation of a secure Azure infrastructure environment focused on private connectivity, identity-based access, and secure administrative access.

The environment was built as part of my Azure Administrator (AZ-104) learning path and includes networking, security, storage, identity, and private endpoint integration.

---

## Architecture
![Architecture](images/architecture.PNG)

---

# Project Goals

- Deploy a secure Azure Virtual Machine environment
- Implement private access to Azure services
- Avoid public exposure of sensitive resources
- Use identity-based authentication instead of embedded credentials
- Demonstrate Azure networking and security best practices

---

# Azure Services Used

## Compute
- Azure Virtual Machine

## Networking
- Virtual Network (VNet)
- Subnets
- Network Security Group (NSG)
- Azure Bastion
- Private Endpoints
- Private DNS Zones

## Security
- Azure Key Vault
- Managed Identity
- IAM (RBAC)

## Storage
- Azure Storage Account

---

# Security Design

## Secure Administrative Access
The Virtual Machine is accessed through Azure Bastion, avoiding direct public RDP exposure.

## Private Connectivity
Storage Account and Key Vault are integrated using Private Endpoints and Private DNS Zones to ensure private communication inside the Virtual Network.

## Identity-Based Access
Managed Identity is used to securely authenticate Azure resources without storing credentials inside the VM.

---

# Networking Design

The infrastructure is divided into separate subnets:

- Compute Subnet
- Private Endpoint Subnet

Private DNS Zones are configured for:
- privatelink.blob.core.windows.net
- privatelink.vaultcore.azure.net

---

# Skills Demonstrated

- Azure Infrastructure Administration
- Azure Networking
- Private Link / Private Endpoints
- Identity and Access Management (IAM)
- Azure Security Best Practices
- Secure Remote Administration
- Azure Resource Organization

---

# Screenshots

## Resource Group
![Resource Group](images/01-resource-list.PNG)

---

## Virtual Network
![Virtual Network](images/02-vnet-overview.PNG)

## Subnets
![Subnets](images/03-subnets.PNG)

---

## Virtual Machine
![Virtual Machine](images/04-vm-overview.PNG)

## VM Networking
![VM Networking](images/05-vm-networking.PNG)

## NIC Overview
![NIC Overview](images/14-nic-overview.PNG)

---

## Network Security Group
![NSG Rules](images/06-nsg-rules.PNG)

---

## Azure Bastion
![Azure Bastion](images/07-bastion.PNG)

---

## Storage Account
![Storage](images/08-storage-overview.PNG)

## Storage Private Endpoint
![Storage Private Endpoint](images/09-storage-private-endpoint.PNG)

## Storage IAM
![Storage IAM](images/18-storage-iam.PNG)

---

## Key Vault
![Key Vault](images/10-keyvault-overview.PNG)

## Key Vault Networking
![Key Vault Networking](images/11-keyvault-networking.PNG)

## Key Vault IAM
![Key Vault IAM](images/16-keyvault-iam.PNG)

---

## Private DNS
![Private DNS](images/12-private-dns.PNG)

## Private Endpoint
![Private Endpoint](images/13-private-endpoint.PNG)

## Private Endpoint DNS
![Private Endpoint DNS](images/15-private-endpoint-dns.PNG)

---

## Managed Identity
![VM Identity](images/17-vm-identity.PNG)

---

# Notes

This project was created for learning and portfolio purposes as part of my transition into Cloud Administration and Azure infrastructure management.
