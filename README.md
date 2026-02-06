# Repository Overview

This repository serves as a **Centralized Configuration Server** for managing environment-specific properties. It bridges AWS infrastructure settings with Dockerized microservices, ensuring a single source of truth for all application configurations.

## Directory Structure
```
.
├── README.md                          # Documentation for setup and usage.
├── application-app-dev.properties     # Configs for the Development environment.
├── application-app-prod.properties    # Configs for the Production environment.
├── application-app-qa.properties      # Configs for the QA/UAT environment.
├── application-app-test.properties    # Configs for the Automation/Testing environment.
└── application-common.properties      # Global settings shared across all environments.
```

## File Breakdown

- **`application-common.properties`**: Stores universal variables such as logging patterns, application metadata, or shared feature flags.
- **Environment Properties** (`-dev`, `-qa`, `-prod`): Stores environment-specific values such as AWS resource ARNs, database credentials, and API endpoints.
