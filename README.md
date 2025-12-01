# azure-cloud-architecture-demo
Sample Azure cloud architecture and DR design for learning and demonstration purposes. No client or production data.
# Azure Cloud Architecture Demo

This repository contains a **sample Azure cloud architecture** for learning and demonstration purposes.
It is based on my experience in data center, smart city, and enterprise infrastructure, but does **not**
use any real client data.

## Scenario

Design a basic Azure environment for:
- Application servers
- Database
- Storage & backup
- Secure connectivity

## High-Level Architecture

- **Azure Virtual Network (VNet)**
  - Subnet-1: Application VMs
  - Subnet-2: Database VM
  - Subnet-3: Management / Bastion

- **Compute**
  - Azure Virtual Machines (Linux/Windows)
  - VM Scale Set (future expansion – optional)

- **Storage**
  - Azure Storage Account (Blob for backups & logs)
  - Managed Disks for VMs

- **Networking & Security**
  - Network Security Groups (NSG)
  - Azure Bastion / VPN Gateway
  - Azure Firewall / WAF (optional)

- **Monitoring & Management**
  - Azure Monitor
  - Log Analytics Workspace
  - Alerts & Dashboards

## Disaster Recovery (Sample Idea)

- Regular VM backups using Azure Backup
- Geo-redundant storage (GRS) for critical data
- DR runbook for VM restore and failover

## Purpose

This project is created to showcase:
- Understanding of Azure cloud building blocks
- Ability to design a basic, secure, and scalable architecture
- DR and backup thinking for critical workloads

> All diagrams, names, and values are generic and meant only for demo and learning.
