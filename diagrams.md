---
layout: default
title: Diagrams
permalink: /diagrams/
---
<!-- NYXERA_BRANDING_HEADER_START -->
<p align="center">
  <img src="/assets/img/product-logo.png" alt="VectorVue" width="220" />
</p>

<p align="center">
  <a href="https://docs.vectorvue.nyxera.cloud">Docs</a> |
  <a href="https://vectorvue.nyxera.cloud">VectorVue</a> |
  <a href="https://nexus.nyxera.cloud">Nexus</a> |
  <a href="https://nyxera.cloud">Nyxera Labs</a>
</p>
<!-- NYXERA_BRANDING_HEADER_END -->


# Diagrams

## System Architecture

```mermaid
flowchart TD
SpectraStrike --> IngestionLayer
CloudEvents --> IngestionLayer
IngestionLayer --> CorrelationEngine
CorrelationEngine --> GraphModel
GraphModel --> Dashboard
```

## Data Model

```mermaid
flowchart LR
TelemetryEvent --> CanonicalRecord --> CorrelationEntity --> AssuranceView
```

## Wrapper Lifecycle Integration

```mermaid
flowchart LR
WrapperExecution --> SignedPayload --> Ingestion --> Correlation --> EvidenceStore
```

## Federation Model

```mermaid
flowchart TD
OrgA --> FederationCore
OrgB --> FederationCore
FederationCore --> GlobalPolicy
GlobalPolicy --> VectorVueClusters
```

## Evidence Lifecycle

```mermaid
flowchart LR
Collect --> Normalize --> Correlate --> Score --> Report
```

<!-- NYXERA_BRANDING_FOOTER_START -->

---

<p align="center">
  <img src="/assets/img/nyxera-logo.png" alt="Nyxera Labs" width="110" />
</p>

<p align="center">
  2026 VectorVue by Nyxera Labs. All rights reserved.
</p>

<p align="center">
  <a href="https://docs.vectorvue.nyxera.cloud">Docs</a> |
  <a href="https://vectorvue.nyxera.cloud">VectorVue</a> |
  <a href="https://nexus.nyxera.cloud">Nexus</a> |
  <a href="https://nyxera.cloud">Nyxera Labs</a>
</p>
<!-- NYXERA_BRANDING_FOOTER_END -->
