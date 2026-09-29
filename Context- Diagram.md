```mermaid
flowchart TD
    A[Customer] -->|Drops off Clothes| B[Reception]
    B -->|Sorts Laundry| C[Sorting Station]
    C -->|Delicate| D[Delicate Wash]
    C -->|Regular| E[Regular Wash]
    C -->|Heavy Duty| F[Heavy Duty Wash]
    D -->|Drying| G[Delicate Dryer]
    E -->|Drying| H[Regular Dryer]
It should be:

```mermaid
flowchart TD
    A[Customer] -->|Drops off Clothes| B[Reception]
    B -->|Sorts Laundry| C[Sorting Station]
    C -->|Delicate| D[Delicate Wash]
    C -->|Regular| E[Regular Wash]
    C -->|Heavy Duty| F[Heavy Duty Wash]
    F -->|Drying| I[Heavy Duty Dryer]
    G -->|Folding| J[Folding Station]
    H -->|Folding| J
    I -->|Folding| J
    J -->|Quality Check| K[QC Station]
    K -->|Packing| L[Packing Station]
    L -->|Ready for Pickup| M[Pickup Counter]
    M -->|Pickup| A
    B -->|Payment| N[Billing System]
    N -->|Receipt| A
    style A fill:#eef2ff,stroke:#818cf8
    style B fill:#f0fdfa,stroke:#2dd4bf
    style C fill:#f0fdfa,stroke:#2dd4bf
    style D fill:#fff7ed,stroke:#fb923c
    style E fill:#fff7ed,stroke:#fb923c
    style F fill:#fff7ed,stroke:#fb923c
    style G fill:#fdf4ff,stroke:#e879f9
    style H fill:#fdf4ff,stroke:#e879f9
    style I fill:#fdf4ff,stroke:#e879f9
    style J fill:#f0fdf4,stroke:#4ade80
    style K fill:#f0f9ff,stroke:#38bdf8
    style L fill:#ecfeff,stroke:#22d3ee
    style M fill:#f0fdf4,stroke:#4ade80
    
