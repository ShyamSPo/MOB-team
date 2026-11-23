# MOB-team — Cloud Infrastructure & Enterprise RAG Pipeline (WIP)

> **Status:** Rough draft / active work in progress. Expect rough edges, unpolished configs, and ongoing refactoring.

## Overview
This repository houses the Infrastructure-as-Code (Terraform) configurations and backend architecture developed around an enterprise employee training and compliance AI portal[cite: 1]. The system provisions cloud resources to ingest internal policy documents, index them for retrieval-augmented generation (RAG), and serve compliance queries with multi-tenant isolation[cite: 1].

## Architecture & Stack
* **Infrastructure as Code:** Terraform (resource provisioning, networking/access controls, environment setup)[cite: 1]
* **Cloud & Storage:** Microsoft Azure (Blob Storage for document ingestion, Azure AI Search for keyword/vector chunking, Azure DevOps workflows)[cite: 1]
* **Backend & AI Pipeline:** Python, RAG pipeline with tenant isolation and security safeguards[cite: 1]

## Repository Structure
*(Update paths below if your current directory names differ)*
```text
├── terraform/          # Core IaC modules and environment configurations
├── src/                # Backend ingestion, chunking, and RAG query logic
└── tests/              # Safeguard and isolation validation scripts
