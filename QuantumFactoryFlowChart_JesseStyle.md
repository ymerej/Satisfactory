# Quantum Factory Flow Chart - Jesse Style

## Quantum Processing Production Flow Diagram (Visual Style)

```mermaid
flowchart TD
    %% Raw Inputs
    A[Reanimated SAM<br/>200/min]
    B[Diamonds<br/>60/min]
    
    %% Floor 1 - Basic Quantum Materials
    A -->|200/min| C[Converter<br/>2x<br/>Dark Matter Residue]
    C -->|400/min| D[Dark Matter Residue]
    
    E[Converter<br/>4x<br/>Excited Photonic Matter]
    E -->|800/min| F[Excited Photonic Matter]
    
    D -->|300/min| G[Particle Accelerator<br/>2x<br/>Dark Matter Crystal]
    B -->|60/min| G
    G -->|40/min| H[Dark Matter Crystal]
    
    %% Floor 2 - Quantum Components
    I[Time Crystal<br/>33.33/min<br/>External Input]
    J[Supercomputer<br/>4/min<br/>External Input]
    K[Ficsite Trigon<br/>93.33/min<br/>External Input]
    
    H -->|20/min| L[Quantum Encoder<br/>2x<br/>Neural-Quantum Processor]
    I -->|20/min| L
    J -->|4/min| L
    K -->|60/min| L
    F -->|100/min| L
    L -->|4/min| M[Neural-Quantum Processor]
    L -->|100/min| N[Dark Matter Residue Return]
    
    O[Crystal Oscillator<br/>6.67/min<br/>External Input]
    P[Alclad Aluminum Sheet<br/>60/min<br/>External Input]
    
    H -->|20/min| Q[Quantum Encoder<br/>2x<br/>Superposition Oscillator]
    O -->|6.67/min| Q
    P -->|60/min| Q
    F -->|166.67/min| Q
    Q -->|6.67/min| R[Superposition Oscillator]
    Q -->|166.67/min| S[Dark Matter Residue Return]
    
    %% Floor 3 - Advanced Quantum Components
    T[Magnetic Field Generator<br/>5.33/min<br/>External Input]
    
    M -->|5.33/min| U[Quantum Encoder<br/>2x<br/>AI Expansion Server]
    R -->|5.33/min| U
    T -->|5.33/min| U
    F -->|133.33/min| U
    U -->|5.33/min| V[AI Expansion Server]
    U -->|133.33/min| W[Dark Matter Residue Return]
    
    %% Synthetic Power Shard Production
    X[Quartz Crystal<br/>80/min<br/>External Input]
    
    I -->|13.33/min| Y[Quantum Encoder<br/>2x<br/>Synthetic Power Shard]
    H -->|13.33/min| Y
    X -->|80/min| Y
    F -->|80/min| Y
    Y -->|6.67/min| Z[Synthetic Power Shard]
    Y -->|80/min| AA[Dark Matter Residue Return]
    
    %% Floor 4 - End-Game Applications
    BB[Ficsonium<br/>5/min<br/>External Input]
    CC[Electromagnetic Control Rod<br/>5/min<br/>External Input]
    
    BB -->|5/min| DD[Quantum Encoder<br/>2x<br/>Ficsonium Fuel Rod]
    CC -->|5/min| DD
    K -->|33.33/min| DD
    F -->|66.67/min| DD
    DD -->|3.33/min| EE[Ficsonium Fuel Rod]
    DD -->|66.67/min| FF[Dark Matter Residue Return]
    
    %% Output Products
    V -->|5.33/min| GG[AI Expansion Server<br/>Ultra-High Value Product]
    Z -->|6.67/min| HH[Synthetic Power Shard<br/>Infinite Power Production]
    EE -->|3.33/min| II[Ficsonium Fuel Rod<br/>Ultimate Energy Storage]
    
    %% External Dependencies - Major Inputs
    JJ[Diamond Production<br/>Coal + Limestone or Alternates]
    KK[Supercomputer Production<br/>From Copper Section]
    LL[Time Crystal Production<br/>From Quartz Processing]
    MM[Alclad Aluminum<br/>From Aluminum Section]
    NN[SAM Processing<br/>Reanimated SAM Production]
    
    JJ -.->|60/min| B
    KK -.->|4/min| J
    LL -.->|33.33/min| I
    MM -.->|60/min| P
    NN -.->|200/min| A
    
    %% Styling
    classDef inputNode fill:#ff6b6b,stroke:#d63031,stroke-width:2px,color:#fff
    classDef converterNode fill:#74b9ff,stroke:#0984e3,stroke-width:2px,color:#fff
    classDef acceleratorNode fill:#fd79a8,stroke:#e84393,stroke-width:2px,color:#fff
    classDef encoderNode fill:#a29bfe,stroke:#6c5ce7,stroke-width:2px,color:#fff
    classDef outputNode fill:#00b894,stroke:#00a085,stroke-width:2px,color:#fff
    classDef externalNode fill:#fdcb6e,stroke:#e17055,stroke-width:2px,color:#000
    
    class A,B inputNode
    class C,E converterNode
    class G acceleratorNode
    class L,Q,U,Y,DD encoderNode
    class V,Z,EE,GG,HH,II outputNode
    class I,J,K,O,P,T,X,BB,CC,JJ,KK,LL,MM,NN externalNode
```

---

## Production Chain Overview

### Material Flow Summary
```
Reanimated SAM (200/min) → Dark Matter Residue (400/min)
    ├── Dark Matter Crystal (40/min) → Quantum Components
    └── Excited Photonic Matter (800/min) → Universal Quantum Input
    
Quantum Components:
├── Neural-Quantum Processor (4/min)
├── Superposition Oscillator (6.67/min)
├── AI Expansion Server (5.33/min) ◄── Primary Product
├── Synthetic Power Shard (6.67/min) ◄── Infinite Power Source
└── Ficsonium Fuel Rod (3.33/min) ◄── Ultimate Energy Storage

External Dependencies:
├── Diamonds (60/min) ◄── From Coal/Limestone Processing
├── Supercomputers (4/min) ◄── From Copper Section
├── Time Crystals (33.33/min) ◄── From Quartz Processing
├── Alclad Aluminum Sheets (60/min) ◄── From Aluminum Section
├── Crystal Oscillators (6.67/min) ◄── From Quartz Processing
├── Magnetic Field Generators (5.33/min) ◄── From Caterium Processing
└── Various Advanced Materials ◄── From Multiple Sections
```

### Machine Layout by Floor

#### Floor 1: Basic Quantum Materials
| Machine | Count | Input | Output |
|---------|-------|-------|--------|
| Converter (Dark Matter Residue) | 2x | 200 Reanimated SAM/min | 400 Dark Matter Residue/min |
| Converter (Excited Photonic Matter) | 4x | No input required | 800 Excited Photonic Matter/min |
| Particle Accelerator (Dark Matter Crystal) | 2x | 60 Diamonds + 300 Dark Matter Residue/min | 40 Dark Matter Crystal/min |

#### Floor 2: Quantum Component Manufacturing
| Machine | Count | Input | Output |
|---------|-------|-------|--------|
| Quantum Encoder (Neural-Quantum Processor) | 2x | 20 Time Crystal + 4 Supercomputer + 60 Ficsite Trigon + 100 Excited Photonic Matter/min | 4 Neural-Quantum Processor + 100 Dark Matter Residue/min |
| Quantum Encoder (Superposition Oscillator) | 2x | 20 Dark Matter Crystal + 6.67 Crystal Oscillator + 60 Alclad Aluminum Sheet + 166.67 Excited Photonic Matter/min | 6.67 Superposition Oscillator + 166.67 Dark Matter Residue/min |

#### Floor 3: Advanced Quantum Systems
| Machine | Count | Input | Output |
|---------|-------|-------|--------|
| Quantum Encoder (AI Expansion Server) | 2x | 5.33 Magnetic Field Generator + 5.33 Neural-Quantum Processor + 5.33 Superposition Oscillator + 133.33 Excited Photonic Matter/min | 5.33 AI Expansion Server + 133.33 Dark Matter Residue/min |
| Quantum Encoder (Synthetic Power Shard) | 2x | 13.33 Time Crystal + 13.33 Dark Matter Crystal + 80 Quartz Crystal + 80 Excited Photonic Matter/min | 6.67 Synthetic Power Shard + 80 Dark Matter Residue/min |

#### Floor 4: Ultimate Quantum Technology
| Machine | Count | Input | Output |
|---------|-------|-------|--------|
| Quantum Encoder (Ficsonium Fuel Rod) | 2x | 5 Ficsonium + 5 Electromagnetic Control Rod + 33.33 Ficsite Trigon + 66.67 Excited Photonic Matter/min | 3.33 Ficsonium Fuel Rod + 66.67 Dark Matter Residue/min |

### Power Requirements Analysis
| Machine Type | Count | Power Range | Total Power |
|--------------|--------|-------------|-------------|
| Converter | 6x | 100-400 MW each | 600-2,400 MW |
| Particle Accelerator | 2x | 500-1,500 MW each | 1,000-3,000 MW |
| Quantum Encoder | 8x | 0-2,000 MW each | 0-16,000 MW |
| **Total Power Consumption** | **16x** | | **1,600-21,400 MW** |

### Critical Design Notes

**Quantum Material Flow:**
- **Dark Matter Residue is Central:** All quantum processing stems from this base material
- **Excited Photonic Matter is Universal:** Required in nearly every quantum recipe
- **Dark Matter Residue Recycling:** Quantum Encoders return Dark Matter Residue as byproduct
- **Massive Power Requirements:** Variable power consumption based on production rates

**External Dependencies:**
- **Diamond Production:** Essential for Dark Matter Crystal (60/min required)
- **Electronics Integration:** Supercomputers from copper section (4/min)
- **Material Processing:** Advanced materials from aluminum, quartz, and caterium sections
- **SAM Processing Foundation:** Reanimated SAM production from SAM ore processing

**Power Infrastructure:**
- **Variable Power Consumption:** Quantum Encoders scale power usage with production
- **Peak Power:** Up to 21,400 MW for full quantum processing
- **Nuclear Power Integration:** Requires multiple nuclear power plants or advanced fuel systems

**Strategic Value:**
- **AI Expansion Server:** Enables ultimate automation and space elevator progression
- **Synthetic Power Shard:** Infinite power shard production for ionized fuel
- **Ficsonium Fuel Rod:** Ultimate energy storage technology
- **Technology Gateway:** Quantum section unlocks end-game content progression
```
