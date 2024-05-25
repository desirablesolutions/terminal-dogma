---
color: "#20bf6b"
---
# Architecture
##### [[Projects/Blakprint/Blakprint|Blakprint]]

![[blakprint-logo.png]]

## Diagram

```mermaid
flowchart 
 DEFINE["Definition functor"]
 EFFECTOR["Effector actuator"]
 TYPES["Types"]

 DEFINE --> EFFECTOR
```

## Abstract
```mermaid

flowchart TB

  MEMORY_SPACE["Memory Space"]
  EXECUTION_SPACE["Execution Space"]
  ABSTRACTION_SPACE["Abstraction Space"]

  EXECUTION_SPACE <--mutates--> MEMORY_SPACE
  EXECUTION_SPACE <--reads--> ABSTRACTION_SPACE


  MEMORY_SPACE <--reads--> EXECUTION_SPACE


  ABSTRACTION_SPACE <--hypervises--> EXECUTION_SPACE 
  ABSTRACTION_SPACE <--hypervises--> MEMORY_SPACE 
```



# Metadata
> [!info]- *Metadata*
> **Date** = 2023-10-17
> **Status** = [#in-progress]