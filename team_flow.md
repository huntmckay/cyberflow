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
    HUNT1[Delta From Baseline] --> REPORTING
    end

    subgraph INTEL 
    INTEL1[Delta From Baseline] --> REPORTING
    end

    subgraph NETWORK 
    NETWORK1[Delta From Baseline] --> REPORTING
    end

    B --> HOST1
    B --> HUNT1
    B --> INTEL1
    B --> NETWORK1

    subgraph REPORTING
    R1[Accuratly Document finding]
    R2[Report to First Line Leader]
    R3[Line Leader informs other teams]
    R4[Enough for IOC?]
    R5[Inform Commander call attention to the SOC]

    R1 --> R2
    R2 --> R3
    R3 --> R4
    R4 - YES -> R5
    R4 - NO -> B
    end

```
# A B C D E F G H I J K L M N O P Q R S T U V W X Y Z
# TODO - Color Code who owns which step
# TODO - Shape code paperwork, computer work, intel, etc
