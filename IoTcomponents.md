## Flowchar tuff

``` mermaid

graph LR
  A[IoT Sensors] -->|Raw Data| B[Data Collection Layer]
  B -->|Stream| C[Data Processing Layer]
  C -->|Clean Data| D[Storage Layer]
  D -->|Query| E[Analytics Layer]

  subgraph Edge Layer
  A
  B
  end

  subgraph Cloud Platform
  C
  D
  E
  end

  E -->|Insights| F[Visualization Dashboard]
  E -->|Alerts| G[Notification System]

  style A fill:#90EE90
  style B fill:#ADD8E6
  style C fill:#FFB6C1
  style D fill:#DDA0DD
  style E fill:#F0E68C
  style F fill:#98FB98
  style G fill:#FFA07A
```