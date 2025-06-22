# Iron Factory Flow Chart - Jesse Style

## Iron Production Flow Diagram (Visual Style)

```mermaid
flowchart TD
    %% Raw Input
    A[Iron Ore] -->|120/min| B[Smelter<br/>4x]
    
    %% Floor 1 - Iron Ingots
    B -->|120/min| C[Iron Ingots]
    
    %% Floor 2 - Basic Component Split
    C -->|120/min| D[Constructor<br/>4x<br/>Iron Plates]
    C -->|120/min| E[Constructor<br/>8x<br/>Iron Rods]
    
    D -->|80/min| F[Iron Plates]
    E -->|120/min| G[Iron Rods]
    
    %% Iron Rod Distribution Hub
    G -->|120/min| H[Constructor<br/>12x<br/>Screws]
    G -->|20/min| I[Iron Rods<br/>to Rotors]
    G -->|48/min| J[Iron Rods<br/>to Modular Frames]
    G -->|15/min| K[Constructor<br/>1x<br/>Rebar]
    G -->|24/min| L[Iron Rods<br/>to Portable Miners]
    
    H -->|480/min| M[Screws]
    K -->|15/min| N[Iron Rebar]
    
    %% Floor 3 - Assembly Operations
    F -->|120/min| O[Assembler<br/>4x<br/>Reinforced Iron Plates]
    M -->|240/min| O
    M -->|400/min| P[Assembler<br/>4x<br/>Rotors]
    I -->|80/min| P
    
    O -->|20/min| Q[Reinforced Iron Plates]
    P -->|16/min| R[Rotors]
    
    %% Floor 4 - Final Products
    Q -->|12/min| S[Assembler<br/>4x<br/>Modular Frames]
    J -->|48/min| S
    F -->|12/min| T[Equipment Workshop<br/>1x<br/>Portable Miners]
    L -->|24/min| T
    
    S -->|8/min| U[Modular Frames]
    T -->|6/min| V[Portable Miners]
    
    %% Styling - Jesse Inspired
    classDef rawMaterial fill:#2E86AB,stroke:#2E86AB,stroke-width:3px,color:#fff
    classDef machine fill:#A23B72,stroke:#A23B72,stroke-width:2px,color:#fff
    classDef intermediate fill:#F18F01,stroke:#F18F01,stroke-width:2px,color:#fff
    classDef finalProduct fill:#C73E1D,stroke:#C73E1D,stroke-width:3px,color:#fff
    classDef smallOutput fill:#6A994E,stroke:#6A994E,stroke-width:2px,color:#fff
    
    class A rawMaterial
    class B,D,E,H,K,O,P,S,T machine
    class C,F,G,M,Q,I,J,L intermediate
    class U finalProduct
    class R,V,N smallOutput
```

## Production Chain Overview

### Material Flow Summary
```
Iron Ore (120/min)
    ↓ 
Iron Ingots (120/min)
    ├── Iron Plates (80/min) ──┐
    └── Iron Rods (120/min) ───┼── Screws (480/min)
                               │       ├── → Reinforced Iron Plates (20/min)
                               │       └── → Rotors (16/min)
                               ├── → Rotors (20/min direct)
                               ├── → Modular Frames (48/min direct)
                               ├── → Iron Rebar (15/min)
                               └── → Portable Miners (24/min)

Final Outputs:
├── Modular Frames (8/min) ◄── Primary Product
├── Rotors (16/min) 
├── Portable Miners (6/min)
└── Iron Rebar (15/min)
```

### Machine Layout by Floor

#### Floor 1: Primary Processing
| Machine | Count | Input | Output |
|---------|-------|-------|--------|
| Smelter | 4x | 120 Iron Ore/min | 120 Iron Ingots/min |

#### Floor 2: Component Manufacturing  
| Machine | Count | Input | Output |
|---------|-------|-------|--------|
| Constructor (Plates) | 4x | 120 Iron Ingots/min | 80 Iron Plates/min |
| Constructor (Rods) | 8x | 120 Iron Ingots/min | 120 Iron Rods/min |
| Constructor (Screws) | 12x | 120 Iron Rods/min | 480 Screws/min |
| Constructor (Rebar) | 1x | 15 Iron Rods/min | 15 Iron Rebar/min |

#### Floor 3: Intermediate Assembly
| Machine | Count | Input | Output |
|---------|-------|-------|--------|
| Assembler (Reinforced Plates) | 4x | 120 Iron Plates + 240 Screws/min | 20 Reinforced Iron Plates/min |
| Assembler (Rotors) | 4x | 80 Iron Rods + 400 Screws/min | 16 Rotors/min |

#### Floor 4: Final Assembly
| Machine | Count | Input | Output |
|---------|-------|-------|--------|
| Assembler (Modular Frames) | 4x | 12 Reinforced Iron Plates + 48 Iron Rods/min | 8 Modular Frames/min |
| Equipment Workshop | 1x | 12 Iron Plates + 24 Iron Rods/min | 6 Portable Miners/min |

### Critical Design Notes

**Distribution Strategy:**
- **Iron Rods are the Hub:** Split 5 ways from Floor 2
- **Screw Production:** Largest consumer of iron rods (12 constructors needed)
- **Modular Frames:** Primary high-value output target
- **Balanced Production:** All outputs scale proportionally

**Belt Management:**
- **Floor 2 → Floor 3:** Major throughput requirement (screws + plates)
- **Floor 3 → Floor 4:** Lower volume, higher value materials
- **Horizontal Distribution:** Most complexity on Floor 2

**Power Requirements:**
- **Total Consumption:** ~2,240 MW
- **Critical Machines:** Assemblers consume most power (150 MW each)
- **Scaling Factor:** Linear scaling for additional miners
