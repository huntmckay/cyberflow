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


    subgraph REPORTING
    Z[Report to First Line]
    end

    B --> HOST1
    B --> HUNT1
    B --> INTEL1
    B --> NETWORK1


```
# A B C D E F G H I J K L M N O P Q R S T U V W X Y Z
# TODO - Color Code who owns which step
# TODO - Shape code paperwork, computer work, intel, etc
