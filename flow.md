```mermaid
---
Title: Command planning phase
---
flowchart TD
    A[Cyber Respose/Audit Request] --> B[Established MOU?]
    B --> C[Unit Assessment for personel and equiptment]
    C --> D[Orange Mission Brief to Cyber unit]
    D --> Audit
    D --> Response
    H[Guidence of Priorities]
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

    subgraph Audit
    a1[Incidents?] --> a2
    a2[Threats?] --> a3
    a3[Critical Elements?] --> a4
    a4[Orange Baseline of users and computers?] --> a5
    a5[Does MPB match Cyber Request]
    a5 --> |NO| A
    a5 --> |YES| H
```

# TODO - Color Code who owns which step
# TODO - Shape code paperwork, computer work, intel, etc
