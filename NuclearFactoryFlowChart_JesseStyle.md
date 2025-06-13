# Nuclear Factory Flow Chart - Jesse Style

## Nuclear Processing Production Flow Diagram (Visual Style)

```mermaid
flowchart TD
    %% Raw Inputs
    A[Uranium<br/>600/min]
    B[Water<br/>14,400/min]
    
    %% Floor 1 - Uranium Processing
    A -->|400/min| C[Blender<br/>20x<br/>Encased Uranium Cell]
    D[Concrete<br/>600/min<br/>External Input] -->|600/min| C
    E[Sulfuric Acid<br/>1,200/min<br/>External Input] -->|1,200/min| C
    C -->|800/min| F[Encased Uranium Cell]
    
    A -->|200/min| G[Blender<br/>10x<br/>Non-Fissile Uranium]
    H[Uranium Waste<br/>100/min<br/>From Nuclear Plants] -->|100/min| G
    I[Nitric Acid<br/>250/min<br/>External Input] -->|250/min| G
    G -->|400/min| J[Non-Fissile Uranium]
    
    %% Floor 2 - Uranium Power Generation
    F -->|400/min| K[Manufacturer<br/>20x<br/>Uranium Fuel Rod]
    L[Encased Industrial Beam<br/>24/min<br/>External Input] -->|24/min| K
    M[Electromagnetic Control Rod<br/>40/min<br/>External Input] -->|40/min| K
    K -->|8/min| N[Uranium Fuel Rod]
    
    N -->|4/min| O[Nuclear Power Plant<br/>20x<br/>Uranium Power]
    B -->|4,800/min| O
    O -->|50,000 MW| P[Uranium Power Output]
    O -->|200/min| Q[Uranium Waste]
    
    %% Floor 3 - Plutonium Processing
    J -->|400/min| R[Particle Accelerator<br/>4x<br/>Plutonium Pellet]
    Q -->|100/min| R
    R -->|120/min| S[Plutonium Pellet]
    
    S -->|60/min| T[Assembler<br/>12x<br/>Encased Plutonium Cell]
    D -->|240/min| T
    E -->|120/min| T
    T -->|60/min| U[Encased Plutonium Cell]
    
    %% Floor 4 - Plutonium Power Generation
    U -->|60/min| V[Manufacturer<br/>24x<br/>Plutonium Fuel Rod]
    W[Steel Beam<br/>108/min<br/>External Input] -->|108/min| V
    M -->|36/min| V
    X[Heat Sink<br/>60/min<br/>External Input] -->|60/min| V
    V -->|6/min| Y[Plutonium Fuel Rod]
    
    Y -->|3/min| Z[Nuclear Power Plant<br/>30x<br/>Plutonium Power]
    B -->|7,200/min| Z
    Z -->|75,000 MW| AA[Plutonium Power Output]
    Z -->|300/min| BB[Plutonium Waste]
    
    %% Floor 5 - Advanced Nuclear Materials
    CC[Copper Powder<br/>100/min<br/>External Input] -->|100/min| DD[Particle Accelerator<br/>1x<br/>Nuclear Pasta]
    EE[Pressure Conversion Cube<br/>0.5/min<br/>External Input] -->|0.5/min| DD
    DD -->|0.5/min| FF[Nuclear Pasta]
    
    %% Power Output Summary
    P -->|50,000 MW| GG[Total Nuclear Power<br/>125,000 MW]
    AA -->|75,000 MW| GG
    
    %% Waste Management
    Q -->|100/min| HH[Uranium Waste<br/>Recycling to Plutonium]
    BB -->|300/min| II[Plutonium Waste<br/>To Quantum Section]
    
    %% External Dependencies - Major Inputs
    JJ[Limestone Processing<br/>Concrete Production]
    KK[Sulfur Processing<br/>Acid Production]
    LL[Steel Section<br/>Structural Components]
    MM[Aluminum Section<br/>Heat Sink Production]
    NN[Water Infrastructure<br/>Massive Water Supply]
    
    JJ -.->|840/min| D
    KK -.->|1,320/min| E
    LL -.->|132/min| W
    MM -.->|60/min| X
    NN -.->|12,000/min| B
    
    %% Advanced Applications
    FF -->|0.5/min| OO[Singularity Cell<br/>Production Input]
    BB -->|300/min| PP[Ficsonium<br/>Production Input]
    
    %% Styling
    classDef inputNode fill:#ff6b6b,stroke:#d63031,stroke-width:2px,color:#fff
    classDef blenderNode fill:#74b9ff,stroke:#0984e3,stroke-width:2px,color:#fff
    classDef manufacturerNode fill:#fd79a8,stroke:#e84393,stroke-width:2px,color:#fff
    classDef acceleratorNode fill:#a29bfe,stroke:#6c5ce7,stroke-width:2px,color:#fff
    classDef nuclearNode fill:#00b894,stroke:#00a085,stroke-width:2px,color:#fff
    classDef powerNode fill:#fdcb6e,stroke:#e17055,stroke-width:3px,color:#000
    classDef wasteNode fill:#636e72,stroke:#2d3436,stroke-width:2px,color:#fff
    classDef externalNode fill:#ddd,stroke:#999,stroke-width:1px,color:#000
    
    class A,B inputNode
    class C,G blenderNode
    class K,V manufacturerNode
    class R,DD acceleratorNode
    class O,Z nuclearNode
    class P,AA,GG powerNode
    class Q,BB,HH,II wasteNode
    class D,E,H,I,L,M,W,X,CC,EE,JJ,KK,LL,MM,NN externalNode
```

---

## Production Chain Overview

### Material Flow Summary
```
Uranium (600/min) → [Split 2 ways]
    ├── Encased Uranium Cell (800/min) → Uranium Fuel Rod → 50,000 MW Power
    └── Non-Fissile Uranium (400/min) → Plutonium Processing → 75,000 MW Power
    
Power Generation:
├── Uranium Power: 50,000 MW (20 Nuclear Plants)
├── Plutonium Power: 75,000 MW (30 Nuclear Plants)
└── Total Nuclear Power: 125,000 MW ◄── Massive Energy Output

Waste Processing:
├── Uranium Waste (200/min) → Recycled to Plutonium Processing
├── Plutonium Waste (300/min) → To Quantum Section (Ficsonium)
└── Nuclear Pasta (0.5/min) → Advanced Applications (Singularity Cells)

External Dependencies:
├── Concrete (840/min) ◄── From Limestone Processing
├── Sulfuric Acid (1,320/min) ◄── From Sulfur Processing
├── Water (12,000/min) ◄── Industrial Water Infrastructure
├── Steel Components (132/min) ◄── From Steel Section
└── Heat Sinks (60/min) ◄── From Aluminum Section
```

### Machine Layout by Floor

#### Floor 1: Uranium Processing
| Machine | Count | Input | Output |
|---------|-------|-------|--------|
| Blender (Encased Uranium Cell) | 20x | 400 Uranium + 600 Concrete + 1,200 Sulfuric Acid/min | 800 Encased Uranium Cell/min |
| Blender (Non-Fissile Uranium) | 10x | 200 Uranium + 100 Uranium Waste + 250 Nitric Acid/min | 400 Non-Fissile Uranium/min |

#### Floor 2: Uranium Power Generation
| Machine | Count | Input | Output |
|---------|-------|-------|--------|
| Manufacturer (Uranium Fuel Rod) | 20x | 400 Encased Uranium Cell + 24 Encased Industrial Beam + 40 Electromagnetic Control Rod/min | 8 Uranium Fuel Rod/min |
| Nuclear Power Plant (Uranium) | 20x | 4 Uranium Fuel Rod + 4,800 Water/min | 50,000 MW + 200 Uranium Waste/min |

#### Floor 3: Plutonium Processing
| Machine | Count | Input | Output |
|---------|-------|-------|--------|
| Particle Accelerator (Plutonium Pellet) | 4x | 400 Non-Fissile Uranium + 100 Uranium Waste/min | 120 Plutonium Pellet/min |
| Assembler (Encased Plutonium Cell) | 12x | 60 Plutonium Pellet + 240 Concrete + 120 Sulfuric Acid/min | 60 Encased Plutonium Cell/min |

#### Floor 4: Plutonium Power Generation
| Machine | Count | Input | Output |
|---------|-------|-------|--------|
| Manufacturer (Plutonium Fuel Rod) | 24x | 60 Encased Plutonium Cell + 108 Steel Beam + 36 Electromagnetic Control Rod + 60 Heat Sink/min | 6 Plutonium Fuel Rod/min |
| Nuclear Power Plant (Plutonium) | 30x | 3 Plutonium Fuel Rod + 7,200 Water/min | 75,000 MW + 300 Plutonium Waste/min |

#### Floor 5: Advanced Nuclear Materials
| Machine | Count | Input | Output |
|---------|-------|-------|--------|
| Particle Accelerator (Nuclear Pasta) | 1x | 100 Copper Powder + 0.5 Pressure Conversion Cube/min | 0.5 Nuclear Pasta/min |

### Power Analysis

#### Power Consumption vs Generation
| Component | Count | Power Consumption | Power Generation | Net Power |
|-----------|--------|------------------|------------------|-----------|
| Blenders | 30x | 2,250 MW | 0 MW | -2,250 MW |
| Manufacturers | 44x | 12,100 MW | 0 MW | -12,100 MW |
| Assemblers | 12x | 1,800 MW | 0 MW | -1,800 MW |
| Particle Accelerators | 5x | 1,250-3,750 MW | 0 MW | -1,250 to -3,750 MW |
| Water Extractors | 40x | 800 MW | 0 MW | -800 MW |
| Nuclear Power Plants | 50x | 0 MW | 125,000 MW | +125,000 MW |
| **Total** | **181x** | **18,200-20,700 MW** | **125,000 MW** | **+104,300-106,800 MW** |

### Critical Design Notes

**Nuclear Power Efficiency:**
- **Input:** 600 Uranium/min → 125,000 MW output
- **ROI:** 5-6x more power generated than consumed
- **Water Critical:** 12,000 water/min requirement for full operation
- **Waste Management:** Uranium waste recycled, plutonium waste exported

**Material Dependencies:**
- **Concrete Production:** 840/min from limestone processing
- **Acid Production:** 1,320/min sulfuric acid from sulfur processing
- **Steel Integration:** 132/min steel components from steel section
- **Water Infrastructure:** Industrial-scale water extraction and distribution

**Production Scaling:**
- **Uranium Processing:** Blenders handle massive material throughput
- **Nuclear Arrays:** 50 nuclear power plants for full power generation
- **Waste Processing:** Efficient uranium waste recycling to plutonium
- **Advanced Materials:** Nuclear pasta for ultimate technology applications

**Safety and Infrastructure:**
- **Radioactive Materials:** Careful handling and storage required
- **Power Distribution:** Massive power grid infrastructure needed
- **Water Management:** Enormous water consumption and distribution
- **Waste Storage:** Long-term radioactive waste containment systems

**Strategic Value:**
- **Primary Power Source:** Foundation for entire factory power grid
- **Plutonium Waste Export:** Essential input for quantum section Ficsonium
- **Nuclear Pasta Production:** Advanced material for singularity technology
- **Energy Independence:** Self-sufficient power generation with massive surplus
```
