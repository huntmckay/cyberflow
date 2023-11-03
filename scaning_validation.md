```mermaid
---
Title: Scanning and Validation Flow
---
flowchart TD
    A[Validate Baseline] 
    A --> B[HOST] --> E
    A --> C[NETWORK] --> E
    A --> D[INTEL] --> E
    E{HUNT} --> F[Delta From Baseline]
    F --> G{Finding?}
    G --> |NO| --> H
    I --> |YES| --> J[DOCUMENT and Nofity other teams] --> K[IOC?]
    K --> |NO| --> H
    L --> |YES| --> M[Report To First Line Leader] & N[Report To Intel] --> P[Blue Brief to Orange]
    L --> O[IOC Validation] --> P[Blue Brief to Orange]
    O --> |NO| --> P[Reprioritize CAL?]
    O --> |YES| --> R[Pack up and debrief] -- S[END]
    P --> |NO| --> A
    P --> |YES| --> A
```
A B C D E F G H I J K L M N O P Q R S T U V W X Y Z
# TODO - Color Code who owns which step
# TODO - Shape code paperwork, computer work, intel, etc
