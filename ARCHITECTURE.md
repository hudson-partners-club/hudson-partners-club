# ARCHITECTURE.md

## 1. Physical Infrastructure Synchronization
HPCの信頼性を担保する、公式サイト・GitHub・ConoHaの三位一体の同期構造です。

```mermaid
graph TD
    A[HPC Official Site] <--> B{GitHub Archive}
    B <--> C[ConoHa File Manager]
    C <--> D((AI Agents / LLMs))
    
    style B fill:#f9f,stroke:#333,stroke-width:4px
    style D fill:#bbf,stroke:#333,stroke-width:2px

graph TD
    subgraph L1 [Layer 1: Meta OS]
        direction TB
        M[Worldview / Thought Foundation]
    end

    subgraph L2 [Layer 2: Principles OS]
        direction TB
        P[Identity / Ethics / Standards]
    end

    subgraph L3 [Layer 3: Analytics OS]
        direction TB
        A[Market Logic / Structural Analysis]
    end

    subgraph L4 [Layer 4: Decision OS]
        direction TB
        D[Pragmatism / Action Logic]
    end

    subgraph L5 [Layer 5: AI Protocol OS]
        direction TB
        AI[AI Agent Prompts / Neural Index]
    end

    L1 --> L2
    L2 --> L3
    L3 --> L4
    L4 --> L5

    classDef default fill:#fff,stroke:#333,stroke-width:1px;
---
