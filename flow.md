```mermaid
---
Title: Command planning phase
---
flowchart TD
    A[Cyber Respose/Audit Request] --> B[Established MOU?]
    B --> C[Unit Assessment for personel and equiptment]
    C --> D[Orange Mission Brief to Cyber unit]
    D --> E[If Audit, what audit?] & F[If Response, Incident? Threats? Critical Elements? Orange Baseline of users and computers?] --> G[Does MPB match Cyber Request]
    G --> |NO| A 
    G --> |YES| H[Guidence of Priorities]
    H --> I[Enumerate the network]
    I --> J[END]
```

# TODO - Color Code who owns which step
# TODO - Shape code paperwork, computer work, intel, etc
