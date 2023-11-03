```mermaid
---
Title: Scanning and Validation Flow
---
flowchart TD
    A[Baseline Validation] 
    A --> B
    B[HOST TEAM] --> B1[HUNT]
    B1 --> B2[Delta From Baseline]
    B2 --> |YES| --> report
    B2 --> |NO| --> B1
    subgraph one
    end

    A --> C
    C[NETWORK TEAM] --> C1[HUNT]
    C1 --> C2[Delta From Baseline]
    C2 --> Z
    subgraph two
    end

    A --> D
    D[SIEM TEAM] --> D1[HUNT]
    D1 --> D2[Delta From Baseline]
    D2 --> Z
    subgraph three
    end


    A --> E
    E[INTEL] --> E1[HUNT]
    E1 --> E2[Delta From Baseline]
    E2 --> Z
    subgraph four
    end

    X --> Y
    Y[Report to First Line] --> Z
    subgraph report
    end

    one --> report
    two --> report
    three --> report
    four --> report


    Z[END]
```
# A B C D E F G H I J K L M N O P Q R S T U V W X Y Z
# TODO - Color Code who owns which step
# TODO - Shape code paperwork, computer work, intel, etc
