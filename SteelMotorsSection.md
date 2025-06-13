# Steel & Motors Section Factory - Complete Production Guide

## Production Pipeline Summary

### Sequential Build Order (Standard Recipes Only)
Build your steel & motors factory in this order to ensure each step feeds into the next:

**Floor 1: Primary Processing**
1. **Iron Ore + Coal → Steel Ingots** (Foundries)

**Floor 2: Basic Steel Components**
2. **Steel Ingots → Steel Beams** (Constructors)
3. **Steel Ingots → Steel Pipes** (Constructors)

**Floor 3: Intermediate Assembly**
4. **Steel Beams + Concrete → Encased Industrial Beams** (Assemblers)
5. **Steel Pipes + Wire → Stators** (Assemblers)

**Floor 4: Advanced Assembly**
6. **Rotors + Stators → Motors** (Assemblers)
7. **Modular Frames + Steel Pipes + Encased Industrial Beams + Screws → Heavy Modular Frames** (Manufacturers)

### Pipeline Flow (Optimized for Minimal Vertical Movement)
```
Floor 1: Iron Ore + Coal → Steel Ingots
           ↓
Floor 2: Steel Ingots → [Split 2 ways]
                    ├── Steel Beams → Encased Industrial Beams
                    └── Steel Pipes → Stators
                                          ↓
Floor 3: Steel Beams + Concrete → Encased Industrial Beams
         Steel Pipes + Wire → Stators
                                          ↓
Floor 4: Rotors + Stators → Motors
         Modular Frames + Steel Components → Heavy Modular Frames
```

### Key Pipeline Notes
- **Start with Steel Ingots:** Everything flows from this base product
- **Floor 2 is the Distribution Hub:** Basic steel components made here
- **External Dependencies:** Requires wire, rotors, modular frames, concrete, and screws
- **High-Value Outputs:** Motors and heavy modular frames are essential for advanced recipes
- **Optimized Vertical Flow:** Each floor primarily feeds the next floor up
- **Storage Between Floors:** Place containers between production stages for smooth flow

### Optimal Building Ratios for Maximum Throughput

Based on production rates and consumption ratios, here are the ideal building combinations:

#### Starting with 1 Steel Ingot Foundry (45 Steel Ingots/min):

**Floor 2 - Basic Components:**
- **Steel Beams:** 3 Constructors (uses 45 ingots → 11.25 beams)
- **Steel Pipes:** 1.5 Constructors (uses 45 ingots → 30 pipes)

**Floor 3 - Intermediate Assembly:**
- **Encased Industrial Beams:** 1.88 Assemblers (uses 45 steel beams + 56.25 concrete → 11.25 encased beams)
- **Stators:** 6 Assemblers (uses 90 steel pipes + 240 wire → 30 stators)

**Floor 4 - Advanced Assembly:**
- **Motors:** 6 Assemblers (uses 60 rotors + 60 stators → 30 motors)
- **Heavy Modular Frames:** 15 Assemblers (uses 75 modular frames + 225 steel pipes + 75 encased beams + 1500 screws → 30 heavy modular frames)

#### Scaling Up - Common Factory Sizes:

**For 4 Steel Production Lines (180 Steel Ingots/min):**
- **Steel Beams:** 12 Constructors
- **Steel Pipes:** 6 Constructors
- **Encased Industrial Beams:** 8 Assemblers
- **Stators:** 24 Assemblers
- **Motors:** 24 Assemblers
- **Heavy Modular Frames:** 60 Assemblers

**For 2 Steel Production Lines (90 Steel Ingots/min):**
- **Steel Beams:** 6 Constructors
- **Steel Pipes:** 3 Constructors
- **Encased Industrial Beams:** 4 Assemblers
- **Stators:** 12 Assemblers
- **Motors:** 12 Assemblers
- **Heavy Modular Frames:** 30 Assemblers

#### Key Throughput Bottlenecks:
1. **Steel Pipe Demand:** Heavy modular frames consume enormous amounts of steel pipes
2. **External Dependencies:** Requires massive input of rotors, modular frames, wire, and screws
3. **Heavy Modular Frame Production:** Longest craft time (30 sec) and highest component count

#### Building Pairing Strategy:
- **Group Steel Pipe Constructors:** Heavy modular frames need massive steel pipe input
- **Stator Assembly Line:** Requires reliable wire supply from copper section
- **Motor Production:** Balance rotor import with stator production
- **Heavy Modular Frame Preparation:** Ensure adequate supply of all four input components

---

## Overview
This steel & motors area focuses on producing advanced structural and mechanical components. This creates a specialized production hub that transforms basic materials into high-value industrial components.

---

## Primary Steel Processing

### Steel Ingot Production
**Standard Recipe (Foundry):**
- **Input:** Iron Ore: 45/min + Coal: 45/min
- **Output:** Steel Ingot: 45/min
- **Building:** Foundry
- **Craft Time:** 4 sec

**Alternate Recipe:**
- **Solid Steel Ingot:** 40 Iron Ingot + 40 Coal → 60 Steel Ingot (Foundry, 3 sec)

---

## Basic Steel Parts (Steel Ingot → Basic Components)

### Steel Beam
- **Input:** Steel Ingot: 60/min
- **Output:** Steel Beam: 15/min
- **Building:** Constructor
- **Craft Time:** 4 sec
- **Stack Size:** 200
- **Sink Points:** 64

### Steel Pipe
- **Input:** Steel Ingot: 30/min
- **Output:** Steel Pipe: 20/min
- **Building:** Constructor
- **Craft Time:** 6 sec
- **Stack Size:** 200
- **Sink Points:** 54

**Alternate Recipe:**
- **Iron Pipe:** 100 Iron Ingot → 25 Steel Pipe (Constructor, 12 sec)

---

## Intermediate Steel Products

### Encased Industrial Beam
- **Input:** Steel Beam: 24/min + Concrete: 30/min
- **Output:** Encased Industrial Beam: 6/min
- **Building:** Assembler
- **Craft Time:** 10 sec
- **Stack Size:** 100
- **Sink Points:** 632
- **Notes:** Requires concrete from limestone processing

### Stator
- **Input:** Steel Pipe: 15/min + Wire: 40/min
- **Output:** Stator: 5/min
- **Building:** Assembler
- **Craft Time:** 12 sec
- **Stack Size:** 100
- **Sink Points:** 240
- **Notes:** Requires wire from copper section

---

## Advanced Steel Products

### Motor
- **Input:** Rotor: 10/min + Stator: 10/min
- **Output:** Motor: 5/min
- **Building:** Assembler
- **Craft Time:** 12 sec
- **Stack Size:** 50
- **Sink Points:** 1,520
- **Notes:** Requires rotors from iron section

### Heavy Modular Frame
- **Input:** Modular Frame: 5/min + Steel Pipe: 15/min + Encased Industrial Beam: 5/min + Screw: 100/min
- **Output:** Heavy Modular Frame: 2/min
- **Building:** Manufacturer
- **Craft Time:** 30 sec
- **Stack Size:** 50
- **Sink Points:** 11,520
- **Notes:** Ultra-high-value product, requires inputs from multiple sections

---

## Steel-Based Alternate Recipes (When Available)

### Encased Industrial Pipe (Alternate)
- **Input:** Steel Pipe: 28/min + Concrete: 20/min
- **Output:** Encased Industrial Beam: 4/min
- **Building:** Assembler
- **Craft Time:** 15 sec
- **Notes:** Alternative encased beam production

### Heavy Encased Frame (Alternate)
- **Input:** Modular Frame: 7.5/min + Encased Industrial Beam: 9.375/min + Steel Pipe: 33.75/min + Concrete: 20.625/min
- **Output:** Heavy Modular Frame: 2.8125/min
- **Building:** Manufacturer
- **Craft Time:** 64 sec
- **Notes:** More efficient heavy modular frame production

---

## Recommended Production Layout

### Phase 1: Basic Steel Processing
1. **Iron Ore + Coal → Steel Ingot** (Multiple Foundries)
2. **Steel Ingot → Steel Beam** (Constructors)
3. **Steel Ingot → Steel Pipe** (Constructors)

### Phase 2: Intermediate Assembly
1. **Steel Beam + Concrete → Encased Industrial Beam** (Assemblers)
2. **Steel Pipe + Wire → Stator** (Assemblers)

### Phase 3: Advanced Assembly
1. **Rotor + Stator → Motor** (Assemblers)
2. **Modular Frame + Steel Components → Heavy Modular Frame** (Manufacturers)

---

## Production Ratios for Efficient Setup

### For 180 Steel Ingots/min Input (4 Foundries):
- **Steel Beams:** 45/min (3 Constructors using 180 Steel Ingots)
- **Steel Pipes:** 120/min (6 Constructors using 180 Steel Ingots)
- **Encased Industrial Beams:** 11.25/min (2 Assemblers using 45 Steel Beams + 56.25 Concrete)
- **Stators:** 25/min (5 Assemblers using 75 Steel Pipes + 200 Wire)
- **Motors:** 25/min (5 Assemblers using 50 Rotors + 50 Stators)
- **Heavy Modular Frames:** 6/min (3 Manufacturers using 15 Modular Frames + 45 Steel Pipes + 15 Encased Beams + 300 Screws)

**External Requirements:**
- **Coal:** 180/min
- **Concrete:** 56.25/min
- **Wire:** 200/min
- **Rotors:** 50/min
- **Modular Frames:** 15/min
- **Screws:** 300/min

---

## Storage Requirements

### Recommended Storage per Product:
- **Iron Ore:** 2-3 Industrial Storage Containers
- **Coal:** 2-3 Industrial Storage Containers
- **Steel Ingots:** 2-3 Industrial Storage Containers
- **Steel Beams:** 1-2 Industrial Storage Containers
- **Steel Pipes:** 2-3 Industrial Storage Containers (high consumption)
- **Encased Industrial Beams:** 1 Industrial Storage Container
- **Stators:** 1-2 Industrial Storage Containers
- **Motors:** 1 Industrial Storage Container
- **Heavy Modular Frames:** 1 Industrial Storage Container (ultra-high value)

---

## Power Requirements

### Estimated Power Consumption for Full Setup:
- **Foundries (4):** 640 MW
- **Constructors (9):** 360 MW
- **Assemblers (12):** 1,800 MW
- **Manufacturers (3):** 825 MW
- **Total:** ~3,625 MW

**Recommended:** 5-7 Coal Generators or 2-3 Fuel Generators to power this section

---

## External Dependencies

### Required Inputs from Other Sections:
- **Iron Ore:** 180/min from iron mining
- **Coal:** 180/min from coal mining
- **Concrete:** 56.25/min from limestone processing
- **Wire:** 200/min from copper section
- **Rotors:** 50/min from iron section
- **Modular Frames:** 15/min from iron section
- **Screws:** 300/min from iron section

### Integration Points:
- **Iron Section:** Essential for rotors, modular frames, and screws
- **Copper Section:** Essential for wire supply
- **Limestone Processing:** Essential for concrete
- **Coal Mining:** Direct coal input for steel production
- **Main Factory Bus:** For distributing motors and heavy modular frames

---

## Expansion Considerations

### Future Upgrades:
1. **Alternate Recipes:** Unlock more efficient steel and motor production
2. **Integration Optimization:** Streamline input pipelines from other sections
3. **Automation:** Connect to main factory bus system
4. **Advanced Products:** Expand to adaptive control units and other high-tech items

### Output Connections:
- **Motors:** Essential for vehicles, manufacturing equipment, and Space Elevator
- **Heavy Modular Frames:** Required for advanced construction and Space Elevator
- **Encased Industrial Beams:** Used in nuclear processing and advanced recipes
- **Steel Components:** Basic building blocks for industrial equipment

### Scaling Considerations:
- **Multi-Section Coordination:** Requires careful balancing with iron and copper sections
- **High External Dependency:** Most complex integration requirements
- **Power Intensive:** Significant power infrastructure needed
- **Ultra-High Value:** Produces some of the most valuable components in the game

### Critical Success Factors:
1. **Reliable Input Streams:** Ensure consistent supply from all contributing sections
2. **Balanced Production:** Match output rates with downstream consumption
3. **Strategic Location:** Position for easy access to multiple input sources
4. **Expandable Design:** Plan for scaling up heavy modular frame production
