```mermaid
---
Title: Scanning and Validation Flow
---
flowchart TD
    A[Validate Baseline] --> B[HOST] & C[NETWORK] & D[INTEL] --> F{HUNT}
    F --> G[Delta From Baseline] --> H{Finding?}
    H --> |NO| --> F
    H --> |YES| --> I[DOCUMENT and Nofity other teams] --> J[IOC?]
    J --> |NO| --> I
    K --> |YES| --> L[Report To First Line Leader] & M[Report To Intel] --> O[Blue Brief to Orange]
    M --> N[IOC Validation] --> O[Blue Brief to Orange]
    P --> |NO| --> Q[Reprioritize CAL?]
    P --> |YES| --> R[Pack up and debrief] -- Z[END]
    Q --> |NO| --> A
    Q --> |YES| --> A
```

# TODO - Color Code who owns which step
# TODO - Shape code paperwork, computer work, intel, etc
