```mermaid
---
Title: Scanning and Validation Flow
---
flowchart TD
    subgraph KEY
    i1(This is the text in the box) --> i2
    i2([This is the text in the box]) --> i3
    i3[[This is the text in the box]] --> i4
    i4((This is the text in the circle)) --> i5
    i5>This is the text in the box] --> i6
    i6{This is the text in the box} --> i7
    i7{{This is the text in the box}} --> i8
    i8[/This is the text in the box/] --> i9
    i9[\This is the text in the box\] --> i10
    i10[/Christmas\] --> i11
    i11[\Go shopping/] --> i12
    i12(((This is the text in the circle)))
    end
```
# A B C D E F G H I J K L M N O P Q R S T U V W X Y Z
# TODO - Color Code who owns which step
# TODO - Shape code paperwork, computer work, intel, etc
