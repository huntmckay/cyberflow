```mermaid
---
Title: Command planning phase
---
flowchart TD
    A[Cyber Respose/Audit Request]
    B[Established MOU?]
    C[Unit Assessment for personel and equiptment]
    D[Orange Mission Brief to Cyber unit]
    H[Guidence of Priorities]
    A --> B
    B --> C
    C --> D
    D --> k1
    D --> r1
    H --> I[Enumerate the network]
    I --> J[END]

    subgraph Response
    r1[Incidents?] --> r2
    r2[Threats?] --> r3
    r3[Critical Elements?] --> r4
    r4[Orange Baseline of users and computers?] --> r5
    r5[Does MPB match Cyber Request]
    r5 --> |NO| A
    r5 --> |YES| H
    end

    subgraph Audit
    k1[Incidents?] --> k2
    k2[Threats?] --> k3
    k3[Critical Elements?] --> k4
    k4[Orange Baseline of users and computers?] --> k5
    k5[Does MPB match Cyber Request]
    k5 --> |NO| A
    k5 --> |YES| H
    end
```

# TODO - Color Code who owns which step
# TODO - Shape code paperwork, computer work, intel, etc
