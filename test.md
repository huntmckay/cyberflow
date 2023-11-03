```mermaid
---
Title: Cyber Response Flow
---
flowhart LR
    subgraph subgraph1
        direction TB
        top1[top] --> bottom1[bottom]
    end
    subgraph subgraph2
        direction TB
        top2[top] --> bottom2[bottom]
    end

    outside --> subgraph1
    outside ---> top2c
```
