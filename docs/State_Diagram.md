```mermaid
stateDiagram-v2
  [*] --> Registered
  Registered --> InTransit
  InTransit --> OutForDelivery
  OutForDelivery --> Delivered
  InTransit --> Delayed
  Delayed --> InTransit
  Delivered --> [*]
  ```
