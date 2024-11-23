## Flowchart with lots of options and neatly arranged code

``` mermaid
flowchart LR
 id1[MQTT Broker]
  id2([IoT Device])
  id3[(Database)]
  id4((Cloud Service))
  id5{{API Gateway}}
  id6[/Data Processor/]
  id7[/Analytics Engine/]

  id1-- Publish -->id2
  id1--> |Subscribe| id3
  id1--- |Store Data| id4
  id2-.-|Send Data| id5
  subgraph "Data Flow"
  id3 == Process ==> id6
  end
  subgraph "Analytics"
  id4 <--> id7 --> id6
  end

  style id1 fill:green,stroke:black
  style id2 fill:white,stroke:#f66,stroke-dasharray: 5, 5
  style id3 fill:#66f,stroke:#f6f,stroke-width:4px
  style id4 fill:red,stroke:yellow
  style id5 fill:orange,stroke:white
  style id6 fill:yellow,stroke:blue
  style id7 fill:brown,stroke:blue
```