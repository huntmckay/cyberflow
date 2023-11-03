```mermaid
---
Title: TESTBED
---
flowchart TD
    A[TEST]
    A --> B
    A --> C
    A --> D
    B --> E
    C --> E
    D --> E
    E --> F
    F --> G
    G -- YES --> H
    I -- YES --> J 
    J --> K
    K -- NO --> H
    L -- YES --> M & N --> P
    L --> O --> P
    O -- NO --> P
    O -- YES --> R -- S
    P -- NO --> A
    P -- YES --> A
    S[END]
```
A B C D E F G H I J K L M N O P Q R S T U V W X Y Z
# TODO - Color Code who owns which step
# TODO - Shape code paperwork, computer work, intel, etc
