# Iron Factory Flow Chart

## Production Flow Diagram with Input/Output Rates

```mermaid
flowchart TD
    %% Raw Materials
    A[Iron Ore<br/>120/min] --> B[Smelter<br/>4x Units]
    
    %% Floor 1 - Primary Processing
    B --> C[Iron Ingots<br/>120/min]
    
    %% Floor 2 - Basic Components Distribution
    C --> D[Constructor<br/>4x Units<br/>Iron Plates]
    C --> E[Constructor<br/>8x Units<br/>Iron Rods]
    
    D --> F[Iron Plates<br/>80/min]
    E --> G[Iron Rods<br/>120/min]
    
    %% Iron Rod Splitting
    G --> H[Constructor<br/>12x Units<br/>Screws]
    G --> I[Iron Rods<br/>20/min<br/>to Rotors]
    G --> J[Iron Rods<br/>24/min<br/>to Modular Frames]
    G --> K[Iron Rods<br/>15/min<br/>to Rebar]
    
    H --> L[Screws<br/>480/min]
    K --> M[Iron Rebar<br/>15/min]
    
    %% Floor 3 - Intermediate Assembly
    F --> N[Assembler<br/>4x Units<br/>Reinforced Iron Plates]
    L --> N
    L --> O[Assembler<br/>4x Units<br/>Rotors]
    I --> O
    
    N --> P[Reinforced Iron Plates<br/>20/min]
    O --> Q[Rotors<br/>16/min]
    
    %% Floor 4 - Final Assembly
    P --> R[Assembler<br/>4x Units<br/>Modular Frames]
    J --> R
    F --> S[Equipment Workshop<br/>Portable Miners]
    G --> S
    
    R --> T[Modular Frames<br/>8/min]
    S --> U[Portable Miners<br/>6/min]
      %% Styling
    classDef inputNode fill:#ff6b6b,stroke:#d63031,stroke-width:2px,color:#fff
    classDef processNode fill:#4ecdc4,stroke:#00b894,stroke-width:2px,color:#fff
    classDef outputNode fill:#a29bfe,stroke:#6c5ce7,stroke-width:2px,color:#fff
    classDef splitNode fill:#fdcb6e,stroke:#e17055,stroke-width:2px,color:#000
    
    class A inputNode
    class B,D,E,H,N,O,R,S processNode
    class T,U,M,Q outputNode
    class C,F,G,L,P splitNode
```

## Detailed Flow Breakdown

### Production Chain Summary:
- **Input:** 120 Iron Ore/min (1 Normal Iron Node)
- **Primary Output:** 8 Modular Frames/min
- **Secondary Outputs:** 16 Rotors/min, 6 Portable Miners/min, 15 Iron Rebar/min

### Machine Count Requirements:
| Machine Type | Quantity | Product | Input Rate | Output Rate |
|--------------|----------|---------|------------|-------------|
| Smelter | 4 | Iron Ingots | 120 Iron Ore/min | 120 Iron Ingots/min |
| Constructor | 4 | Iron Plates | 120 Iron Ingots/min | 80 Iron Plates/min |
| Constructor | 8 | Iron Rods | 120 Iron Ingots/min | 120 Iron Rods/min |
| Constructor | 12 | Screws | 120 Iron Rods/min | 480 Screws/min |
| Constructor | 1 | Iron Rebar | 15 Iron Rods/min | 15 Iron Rebar/min |
| Assembler | 4 | Reinforced Iron Plates | 120 Iron Plates + 240 Screws/min | 20 Reinforced Iron Plates/min |
| Assembler | 4 | Rotors | 80 Iron Rods + 400 Screws/min | 16 Rotors/min |
| Assembler | 4 | Modular Frames | 12 Reinforced Iron Plates + 48 Iron Rods/min | 8 Modular Frames/min |
| Equipment Workshop | 1 | Portable Miners | 12 Iron Plates + 24 Iron Rods/min | 6 Portable Miners/min |

### Critical Split Points:
1. **Iron Ingots (120/min)** splits to:
   - Iron Plates: 120/min
   - Iron Rods: 120/min

2. **Iron Rods (120/min)** splits to:
   - Screws: 120/min (becomes 480 screws)
   - Rotors: 80/min
   - Modular Frames: 48/min
   - Rebar: 15/min
   - Portable Miners: 24/min

3. **Screws (480/min)** splits to:
   - Reinforced Iron Plates: 240/min
   - Rotors: 400/min

4. **Iron Plates (80/min)** splits to:
   - Reinforced Iron Plates: 120/min
   - Portable Miners: 12/min

### Power Requirements:
- **Total Estimated Power:** ~2,240 MW
- **Recommended Power Source:** 3-4 Coal Generators or 1-2 Fuel Generators
