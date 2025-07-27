# Solution Overview

## A. System Architecture
```mermaid
flowchart LR
  A[Mobile/Web App] -->|1. SLUDI OIDC| B[SLUDI Sandbox]
  A -->|2. Menu & Subsidy Request| C[NDX Sandbox]
  A -->|4. Subsidy Payment| D[PayDPI Sandbox]
  C -->|3. Consent & Data| E[Gov Canteen API]
  D -->|5. Record Payment| F[NDX Ledger API]
