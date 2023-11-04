```mermaid
---
Title: Scanning and Validation Flow
---
flowchart TD
    A[Baseline Validation] --> B
    B[Enumeration]

    subgraph HOST 
    HOST1[Delta From Baseline] --> REPORTING
    end

    subgraph HUNT 
    D1 --> D2[Delta From Baseline]
    D2 --> REPORTING
    end

    subgraph INTEL
    E1 --> E2[Delta From Baseline]
    E2 --> REPORTING
    end

    subgraph NETWORK 
    E1 --> E2[Delta From Baseline]
    E2 --> REPORTING
    end

    subgraph REPORTING
    Z[Report to First Line]
    end

    B --> HOST1
    B --> HUNT
    B --> INTEL
    B --> NETWORK

    HOST --> REPORTING
    HUNT --> REPORTING
    INTEL --> REPORTING
    NETWORK --> REPORTING

```
# A B C D E F G H I J K L M N O P Q R S T U V W X Y Z
# TODO - Color Code who owns which step
# TODO - Shape code paperwork, computer work, intel, etc
