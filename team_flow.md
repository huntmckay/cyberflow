```mermaid
---
Title: Scanning and Validation Flow
---
flowchart TD
    A[Baseline Validation] --> B
    B[Enumeration]

    subgraph HOST
    HOST1[Delta From Baseline]
    end

    subgraph HUNT
    HUNT1[Delta From Baseline]
    end

    subgraph INTEL
    INTEL1[Delta From Baseline]
    end

    subgraph NETWORK
    NETWORK1[Delta From Baseline]
    end

    B --> HOST
    B --> HUNT
    B --> INTEL
    B --> NETWORK

    HOST --> REPORTING
    HUNT --> REPORTING
    INTEL --> REPORTING
    NETWORK --> REPORTING

    subgraph REPORTING
    R1[Accuratly Document finding] --> R2
    R2[Report to First Line Leader] --> R3
    R3[Line Leader informs other teams] --> R4
    R4[Enough for IOC?] 
    R4 -- YES --> R5
    R4 -- NO --> R6
    R5[Inform Commander]
    R6[STOP]
    end
```
# A B C D E F G H I J K L M N O P Q R S T U V W X Y Z
# TODO - Color Code who owns which step
# TODO - Shape code paperwork, computer work, intel, etc
