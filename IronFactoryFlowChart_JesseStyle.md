# Iron Factory Flow Chart - Jesse Style

## Iron Production Flow Diagram (Visual Style)

```mermaid
flowchart TD
    %% Raw Input
    A[Iron Ore] -->|120/min| B[Smelter<br/>4x]
    
    %% Floor 1 - Iron Ingots
    B -->|120/min| C[Iron Ingots]
    
    %% Floor 2 - Basic Component Split
    C -->|60/min| D[Constructor<br/>2x<br/>Iron Plates]
    C -->|60/min| E[Constructor<br/>4x<br/>Iron Rods]
    
    D -->|40/min| F[Iron Plates]
    E -->|60/min| G[Iron Rods]
    
    %% Iron Rod Distribution Hub
    G -->|30/min| H[Constructor<br/>3x<br/>Screws]
    G -->|20/min| I[Iron Rods<br/>to Rotors]
    G -->|12/min| J[Iron Rods<br/>to Modular Frames]
    G -->|15/min| K[Constructor<br/>1x<br/>Rebar]
    G -->|12/min| L[Iron Rods<br/>to Portable Miners]
    
    H -->|120/min| M[Screws]
    K -->|15/min| N[Iron Rebar]
    
    %% Floor 3 - Assembly Operations
    F -->|30/min| O[Assembler<br/>1x<br/>Reinforced Iron Plates]
    M -->|60/min| O
    M -->|80/min| P[Assembler<br/>2x<br/>Rotors]
    I -->|20/min| P
    
    O -->|5/min| Q[Reinforced Iron Plates]
    P -->|8/min| R[Rotors]
    
    %% Floor 4 - Final Products
    Q -->|3/min| S[Assembler<br/>1x<br/>Modular Frames]
    J -->|12/min| S
    F -->|6/min| T[Equipment Workshop<br/>1x<br/>Portable Miners]
    L -->|12/min| T
    
    S -->|1.67/min| U[Modular Frames]
    T -->|3/min| V[Portable Miners]
    
    H -->|480/min| M[Screws]
    K -->|15/min| N[Iron Rebar]
      
    %% Floor 3 - Assembly Operations
    F -->|30/min| O[Assembler<br/>1x<br/>Reinforced Iron Plates]
    M -->|60/min| O
    M -->|120/min| P[Assembler<br/>3x<br/>Rotors]
    I -->|24/min| P
    
    O -->|5/min| Q[Reinforced Iron Plates]
    P -->|4.8/min| R[Rotors]
    
    %% Floor 4 - Final Products
    Q -->|3/min| S[Assembler<br/>1x<br/>Modular Frames]
    J -->|12/min| S
    F -->|6/min| T[Equipment Workshop<br/>1x<br/>Portable Miners]
    L -->|12/min| T
    
    S -->|1.67/min| U[Modular Frames]
    T -->|3/min| V[Portable Miners]
    
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
    ├── Iron Plates (40/min) ──┐
    └── Iron Rods (60/min) ────┼── Screws (120/min)
                               │       ├── → Reinforced Iron Plates (5/min)
                               │       └── → Rotors (8/min)
                               ├── → Rotors (20/min direct)
                               ├── → Modular Frames (12/min direct)
                               ├── → Iron Rebar (15/min)
                               └── → Portable Miners (12/min)

Final Outputs:
├── Modular Frames (1.67/min) ◄── Primary Product
├── Rotors (8/min) 
├── Portable Miners (3/min)
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
| Constructor (Plates) | 2x | 60 Iron Ingots/min | 40 Iron Plates/min |
| Constructor (Rods) | 4x | 60 Iron Ingots/min | 60 Iron Rods/min |
| Constructor (Screws) | 3x | 30 Iron Rods/min | 120 Screws/min |
| Constructor (Rebar) | 1x | 15 Iron Rods/min | 15 Iron Rebar/min |

#### Floor 3: Intermediate Assembly
| Machine | Count | Input | Output |
|---------|-------|-------|--------|
| Assembler (Reinforced Plates) | 1x | 30 Iron Plates + 60 Screws/min | 5 Reinforced Iron Plates/min |
| Assembler (Rotors) | 2x | 20 Iron Rods + 80 Screws/min | 8 Rotors/min |

#### Floor 4: Final Assembly
| Machine | Count | Input | Output |
|---------|-------|-------|--------|
| Assembler (Modular Frames) | 1x | 3 Reinforced Iron Plates + 12 Iron Rods/min | 1.67 Modular Frames/min |
| Equipment Workshop | 1x | 6 Iron Plates + 12 Iron Rods/min | 3 Portable Miners/min |

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
