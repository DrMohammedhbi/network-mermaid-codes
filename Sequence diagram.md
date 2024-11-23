## Sequence diagram

``` mermaid
sequenceDiagram
    participant Device as IoT Device
    participant Gateway as IoT Gateway
    participant Server as Cloud Server
    participant User as User

    User->>Device: Send command
    Device->>Gateway: Transmit data
    Gateway->>Server: Forward data securely
    loop Security Check
        Server->>Server: Validate data integrity
        Server->>Server: Authenticate device
    end
    Note right of Server: Data is secure and <br/>authenticated
    Server-->>Gateway: Acknowledge receipt
    Gateway-->>Device: Confirm command execution
    Device-->>User: Command executed successfully
```