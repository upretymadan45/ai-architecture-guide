```mermaid

sequenceDiagram



participant Agent

participant Gateway

participant Vertex

participant Model



Agent->>Gateway: Predict Request

Gateway->>Vertex: Invoke Endpoint

Vertex->>Model: Execute Inference



Model-->>Vertex: Prediction

Vertex-->>Gateway: Response

Gateway-->>Agent: Normalized Result

```

