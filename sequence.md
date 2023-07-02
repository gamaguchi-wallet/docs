```mermaid
sequenceDiagram
  User->>+Exchange: Purchase application
  Exchange-->>-User: Complete event
  User->>+Bank: Transfer legal currency
  Bank-->>+Exchange: Transfer event
  Exchange->>+Blockchain: Deploy contract, send asset, setup DApp
  Blockchain-->>-Exchange: Complete event
  Exchange-->>-User: Complete event

  User->>+Blockchain: Send transaction through wallet contract
  Blockchain-->>-User: Complete event
```
