``` mermaid
graph TD
  A[IoT Devices] -->|Generate Data| B[Data Collection Layer]
  B -->|Real-time Processing| C[Processing Layer]

  subgraph Data Collection
      B --> D[Temperature Sensors]
      B --> E[Humidity Sensors]
      B --> F[Light Sensors]
      B --> G[CO2 Sensors]
  end

  subgraph Processing & Storage
      C --> H[Data Cleaning]
      H --> I[Feature Engineering]
      I --> J[(Database Storage)]
  end

  J -->|Analytics| K[Data Analysis]
  K --> L[Visualization]
  K --> M[Anomaly Detection]
  K --> N[Predictive Models]

  style A fill:#f9f,stroke:#333,stroke-width:2px
  style B fill:#bbf,stroke:#333,stroke-width:2px
  style C fill:#dfd,stroke:#333,stroke-width:2px
  style J fill:#fdd,stroke:#333,stroke-width:2px
```