```mermaid
flowchart TD
    A[Customer] -->|Drops off Clothes| B[Reception]
    B -->|Sorts Laundry| C[Sorting Station]
    C -->|Delicate| D[Delicate Wash]
    C -->|Regular| E[Regular Wash]
    C -->|Heavy Duty| F[Heavy Duty Wash]
