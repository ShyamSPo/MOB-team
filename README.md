# MOB-team — Cloud Infrastructure & Enterprise RAG Platform (WIP)

> **Status:** Active work in progress / post-internship cleanup. Expect rough edges, unpolished configs, and ongoing refactoring.

## Overview
This repository contains Infrastructure-as-Code (Terraform), CI/CD pipelines, backend services, and AI/RAG components built around an enterprise employee training and compliance AI portal. It provisions cloud infrastructure and supports document ingestion, conversational/RAG workflows, quiz generation, and multi-tenant safeguards.

## Stack & Tooling
* **Infrastructure as Code:** Terraform (`infra/`)
* **CI/CD & Automation:** Azure Pipelines (`azure-pipelines-backend.yml`, `azure-pipelines-frontend.yml`) and GitHub Actions (`.github/workflows/`)
* **Backend & AI Services:** Python (`api/`, `chatbot/`, `quizgen/`, `functions/`, `src/`), RAG pipeline with tenant isolation and security validation
* **Data & Frontend:** Database schemas/scripts (`db/`), sample/demo assets (`data/documents/`, `demo-data/`), and web interfaces (`web/`, `web-app/`)

## Repository Structure

```text
├── .claude/                        # AI coding agent configuration/context
├── .github/workflows/              # GitHub Actions workflows
├── .planning/                      # Project planning notes/artifacts
├── api/                            # Backend API endpoints/services
├── chatbot/                        # Conversational / RAG assistant logic
├── data/documents/                 # Source/ingested document fixtures
├── db/                             # Database scripts / schema definitions
├── demo-data/                      # Sample/demo datasets
├── docs/                           # Project documentation
├── functions/                      # Serverless / background functions
├── infra/                          # Terraform IaC configurations[cite: 1]
├── quizgen/                        # Quiz generation module
├── scripts/                        # Utility & operational scripts
├── src/                            # Core application / pipeline source code
├── tests/                          # Test suites (including security/isolation checks)[cite: 1]
├── web/ & web-app/                 # Frontend / web application code
├── azure-pipelines-backend.yml     # Backend CI/CD pipeline[cite: 1]
├── azure-pipelines-frontend.yml    # Frontend CI/CD pipeline[cite: 1]
└── requirements.txt                # Python dependencies
