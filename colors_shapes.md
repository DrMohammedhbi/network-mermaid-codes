## Flowchart with some colors and shapes and stuff

``` mermaid
flowchart TD
    A(Christmas) -->|Get money| B(Go shopping)
    style A fill:red,stroke:black,stroke-width:4px,shadow:shadow
    B --> C{Let me think}
    style B fill:green,stroke:black,stroke-width:4px,shadow:shadow
    C -->|One| D[Laptop]
    style C fill:blue,stroke:black,stroke-width:4px,shadow:shadow
    C -->|Two| E[iPhone]
    C -->|Three| F[fa:fa-car Car]
    style D fill:yellow,stroke:black,stroke-width:2px,shadow:shadow
    style E fill:brown,stroke:black,stroke-width:2px,shadow:shadow
    style F fill:navy,stroke:black,stroke-width:2px,shadow:shadow
```