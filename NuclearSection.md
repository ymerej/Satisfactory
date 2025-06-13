# Nuclear Section Factory - Complete Production Guide

## Production Pipeline Summary

### Sequential Build Order (Standard Recipes Only)
Build your nuclear factory in this order to ensure each step feeds into the next:

**Floor 1: Uranium Processing**
1. **Uranium → Encased Uranium Cell** (Blenders)
2. **Uranium → Non-Fissile Uranium** (Blenders)

**Floor 2: Uranium Power Generation**
3. **Encased Uranium Cell + Encased Industrial Beam + Electromagnetic Control Rod → Uranium Fuel Rod** (Manufacturers)
4. **Uranium Fuel Rod → Nuclear Power Generation** (Nuclear Power Plants)

**Floor 3: Plutonium Processing**
5. **Non-Fissile Uranium + Uranium Waste → Plutonium Pellet** (Particle Accelerators)
6. **Plutonium Pellet + Sulfuric Acid → Encased Plutonium Cell** (Assemblers)

**Floor 4: Plutonium Power Generation**
7. **Encased Plutonium Cell + Steel Beam + Electromagnetic Control Rod + Heat Sink → Plutonium Fuel Rod** (Manufacturers)
8. **Plutonium Fuel Rod → Nuclear Power Generation** (Nuclear Power Plants)

**Floor 5: Advanced Nuclear Materials**
9. **Copper Powder + Pressure Conversion Cube → Nuclear Pasta** (Particle Accelerators)

### Pipeline Flow (Optimized for Minimal Vertical Movement)
```
Floor 1: Uranium → [Split 2 ways]
              ├── Encased Uranium Cell → Uranium Fuel Rod
              └── Non-Fissile Uranium → Plutonium Processing
                                          ↓
Floor 2: Uranium Fuel Rod → Nuclear Power Plant → Uranium Waste
                                          ↓
Floor 3: Non-Fissile Uranium + Uranium Waste → Plutonium Pellet → Encased Plutonium Cell
                                          ↓
Floor 4: Encased Plutonium Cell → Plutonium Fuel Rod → Nuclear Power Plant → Plutonium Waste
                                          ↓
Floor 5: Advanced Materials → Nuclear Pasta
```

### Key Pipeline Notes
- **Start with Uranium:** Everything flows from this base radioactive material
- **Floor 1 is the Uranium Hub:** Basic uranium processing
- **Uranium Waste Recycling:** Critical for plutonium processing efficiency
- **Extremely High Power Output:** Nuclear plants generate 2,500 MW each
- **Radioactive Waste Management:** Plutonium waste must be handled carefully
- **Water Infrastructure:** Massive water consumption for nuclear plants

### Optimal Building Ratios for Maximum Throughput

Based on production rates and consumption ratios, here are the ideal building combinations:

#### Starting with 1 Uranium Miner (300 Uranium/min):

**Floor 1 - Basic Uranium Processing:**
- **Encased Uranium Cell:** 10 Blenders (uses 200 uranium + 120 concrete + 240 sulfuric acid → 200 cells)
- **Non-Fissile Uranium:** 5 Blenders (uses 150 uranium + 100 uranium waste + 100 nitric acid → 200 non-fissile uranium)

**Floor 2 - Uranium Power:**
- **Uranium Fuel Rod:** 10 Manufacturers (uses 200 encased uranium cells + 12 encased industrial beams + 20 electromagnetic control rods → 4 uranium fuel rods)
- **Nuclear Power Plant:** 20 Nuclear Power Plants (uses 4 uranium fuel rods + 4,800 water → 50,000 MW + 200 uranium waste)

**Floor 3 - Plutonium Processing:**
- **Plutonium Pellet:** 2 Particle Accelerators (uses 200 non-fissile uranium + 50 uranium waste → 60 plutonium pellets)
- **Encased Plutonium Cell:** 8 Assemblers (uses 60 plutonium pellets + 120 concrete + 60 sulfuric acid → 30 encased plutonium cells)

**Floor 4 - Plutonium Power:**
- **Plutonium Fuel Rod:** 120 Manufacturers (uses 900 encased plutonium cells + 540 steel beams + 180 electromagnetic control rods + 300 heat sinks → 30 plutonium fuel rods)
- **Nuclear Power Plant:** 300 Nuclear Power Plants (uses 30 plutonium fuel rods + 72,000 water → 750,000 MW + 300 plutonium waste)

#### Scaling Up - Common Factory Sizes:

**For 4 Uranium Miners (1,200 Uranium/min):**
- **Encased Uranium Cell:** 40 Blenders
- **Non-Fissile Uranium:** 20 Blenders
- **Uranium Fuel Rod:** 40 Manufacturers
- **Plutonium Pellet:** 8 Particle Accelerators
- **Nuclear Power Plants:** 1,200+ (massive power generation)

#### Key Throughput Bottlenecks:
1. **Water Supply:** Enormous water consumption for nuclear plants
2. **Concrete Production:** Large concrete requirements for encased cells
3. **Acid Production:** Sulfuric acid dependency for cell production
4. **Waste Management:** Radioactive waste handling and storage

#### Building Pairing Strategy:
- **Uranium Processing Clusters:** Group blenders and manufacturers
- **Nuclear Power Arrays:** Massive nuclear plant installations
- **Water Infrastructure:** Industrial-scale water extraction and piping
- **Acid Production Integration:** Large-scale sulfuric acid supply

---

## Overview
This nuclear processing area transforms uranium ore into the most powerful energy generation system in the game. Nuclear power provides massive energy output but requires careful radioactive material handling and extensive infrastructure.

---

## Primary Uranium Processing

### Encased Uranium Cell Production
**Standard Recipe (Blender):**
- **Input:** Uranium: 50/min + Concrete: 30/min + Sulfuric Acid: 60/min
- **Output:** Encased Uranium Cell: 50/min
- **Building:** Blender
- **Craft Time:** 12 sec
- **Stack Size:** 50
- **Notes:** Foundation for uranium fuel rod production

### Non-Fissile Uranium Production
**Standard Recipe (Blender):**
- **Input:** Uranium: 37.5/min + Uranium Waste: 25/min + Nitric Acid: 25/min
- **Output:** Non-Fissile Uranium: 50/min
- **Building:** Blender
- **Craft Time:** 24 sec
- **Stack Size:** 500
- **Notes:** Used for plutonium pellet production

---

## Uranium Power Generation

### Uranium Fuel Rod
- **Input:** Encased Uranium Cell: 20/min + Encased Industrial Beam: 1.2/min + Electromagnetic Control Rod: 2/min
- **Output:** Uranium Fuel Rod: 0.4/min
- **Building:** Manufacturer
- **Craft Time:** 150 sec
- **Stack Size:** 50
- **Notes:** Primary nuclear fuel, extremely long craft time

### Uranium Fuel Rod (Burning)
- **Input:** Uranium Fuel Rod: 0.2/min + Water: 240/min
- **Output:** Uranium Waste: 10/min
- **Building:** Nuclear Power Plant
- **Craft Time:** 300 sec
- **Power Output:** 2,500 MW
- **Notes:** Massive power generation with radioactive waste byproduct

---

## Plutonium Processing

### Plutonium Pellet
- **Input:** Non-Fissile Uranium: 100/min + Uranium Waste: 25/min
- **Output:** Plutonium Pellet: 30/min
- **Building:** Particle Accelerator
- **Craft Time:** 60 sec
- **Power:** 250-750 MW
- **Stack Size:** 100
- **Notes:** Advanced nuclear material processing

### Encased Plutonium Cell
- **Input:** Plutonium Pellet: 10/min + Concrete: 20/min + Sulfuric Acid: 10/min
- **Output:** Encased Plutonium Cell: 5/min
- **Building:** Assembler
- **Craft Time:** 120 sec
- **Stack Size:** 50
- **Notes:** Advanced nuclear fuel cell component

---

## Plutonium Power Generation

### Plutonium Fuel Rod
- **Input:** Encased Plutonium Cell: 7.5/min + Steel Beam: 4.5/min + Electromagnetic Control Rod: 1.5/min + Heat Sink: 2.5/min
- **Output:** Plutonium Fuel Rod: 0.25/min
- **Building:** Manufacturer
- **Craft Time:** 240 sec
- **Stack Size:** 50
- **Notes:** Ultimate nuclear fuel, extremely complex production

### Plutonium Fuel Rod (Burning)
- **Input:** Plutonium Fuel Rod: 0.1/min + Water: 240/min
- **Output:** Plutonium Waste: 1/min
- **Building:** Nuclear Power Plant
- **Craft Time:** 600 sec
- **Power Output:** 2,500 MW
- **Notes:** Same power output as uranium but longer burn time

---

## Advanced Nuclear Materials

### Nuclear Pasta
- **Input:** Copper Powder: 100/min + Pressure Conversion Cube: 0.5/min
- **Output:** Nuclear Pasta: 0.5/min
- **Building:** Particle Accelerator
- **Craft Time:** 120 sec
- **Power:** 500-1,500 MW
- **Stack Size:** 100
- **Notes:** Ultra-advanced nuclear material for singularity cells

---

## Recommended Production Layout

### Phase 1: Basic Uranium Processing
1. **Uranium → Encased Uranium Cell** (Multiple Blenders)
2. **Uranium → Non-Fissile Uranium** (Multiple Blenders)
3. **Acid Production Integration** (Sulfuric acid supply)

### Phase 2: Uranium Power Generation
1. **Uranium Fuel Rod Production** (Manufacturers)
2. **Nuclear Power Plant Array** (Multiple nuclear plants)
3. **Water Infrastructure** (Massive water extraction)

### Phase 3: Plutonium Processing
1. **Plutonium Pellet Production** (Particle Accelerators)
2. **Encased Plutonium Cell Production** (Assemblers)

### Phase 4: Plutonium Power Generation
1. **Plutonium Fuel Rod Production** (Manufacturers)
2. **Advanced Nuclear Power Array** (Large nuclear plant installation)

### Phase 5: Advanced Nuclear Materials
1. **Nuclear Pasta Production** (Particle Accelerators)
2. **Waste Management** (Storage and handling systems)

---

## Production Ratios for Efficient Setup

### For 600 Uranium/min Input:
- **Encased Uranium Cell:** 400/min (20 Blenders)
- **Non-Fissile Uranium:** 400/min (10 Blenders)
- **Uranium Fuel Rod:** 8/min (20 Manufacturers)
- **Uranium Waste:** 400/min (40 Nuclear Power Plants)
- **Plutonium Pellet:** 120/min (4 Particle Accelerators)
- **Encased Plutonium Cell:** 60/min (12 Assemblers)
- **Plutonium Fuel Rod:** 2/min (8 Manufacturers)

**Power Generation:**
- **Uranium Power:** 100,000 MW (40 Nuclear Power Plants)
- **Plutonium Power:** 50,000 MW (20 Nuclear Power Plants)
- **Total Nuclear Power:** 150,000 MW

**External Material Requirements:**
- **Concrete:** 1,000/min
- **Sulfuric Acid:** 1,000/min
- **Nitric Acid:** 250/min
- **Water:** 14,400/min
- **Steel Beam:** 9/min
- **Electromagnetic Control Rod:** 15/min
- **Heat Sink:** 5/min

---

## Storage Requirements

### Recommended Storage per Product:
- **Uranium:** 3-4 Industrial Storage Containers
- **Encased Uranium Cell:** 3-4 Industrial Storage Containers
- **Non-Fissile Uranium:** 2-3 Industrial Storage Containers
- **Uranium Fuel Rod:** 2-3 Industrial Storage Containers
- **Uranium Waste:** 4-5 Industrial Storage Containers (high production)
- **Plutonium Pellet:** 2-3 Industrial Storage Containers
- **Encased Plutonium Cell:** 2-3 Industrial Storage Containers
- **Plutonium Fuel Rod:** 1-2 Industrial Storage Containers
- **Plutonium Waste:** 3-4 Industrial Storage Containers
- **Nuclear Pasta:** 1 Industrial Storage Container (ultra-rare)

---

## Power Requirements vs Output

### Power Consumption for Full Setup:
- **Blenders (30):** 2,250 MW
- **Manufacturers (28):** 7,700 MW
- **Assemblers (12):** 1,800 MW
- **Particle Accelerators (4):** 2,000-6,000 MW
- **Water Extractors (48):** 960 MW
- **Total Consumption:** ~14,710-18,710 MW

### Power Generation Output:
- **Nuclear Power Plants (60):** 150,000 MW
- **Net Power Contribution:** +131,290-135,290 MW

**ROI:** Nuclear section provides 7-9x more power than it consumes

---

## External Dependencies

### Required Inputs from Other Sections:
- **Concrete:** 1,000/min from limestone processing
- **Sulfuric Acid:** 1,000/min from sulfur processing
- **Nitric Acid:** 250/min from nitrogen processing
- **Steel Beam:** 9/min from steel section
- **Electromagnetic Control Rod:** 15/min from caterium processing
- **Heat Sink:** 5/min from aluminum processing
- **Encased Industrial Beam:** 24/min from steel section

### Integration Points:
- **Limestone Processing:** Massive concrete supply
- **Sulfur Processing:** Large-scale acid production
- **Steel Section:** Structural components
- **Aluminum Section:** Heat sink production
- **Water Infrastructure:** Industrial-scale water extraction

---

## Expansion Considerations

### Future Upgrades:
1. **Waste Processing:** Plutonium waste applications
2. **Advanced Nuclear Technology:** Nuclear pasta applications
3. **Power Grid Expansion:** Factory-wide nuclear power distribution
4. **Safety Systems:** Radioactive material handling and containment

### Output Connections:
- **Factory Power Grid:** Primary power source for entire factory
- **Plutonium Waste:** Input for Ficsonium production (Quantum Section)
- **Nuclear Pasta:** Input for Singularity Cell production
- **Heat Generation:** Potential for industrial applications

### Scaling Considerations:
- **Uranium Node Limitations:** May require multiple uranium deposits
- **Water Resource Management:** Enormous water consumption
- **Acid Production Scaling:** Large-scale chemical processing
- **Power Grid Infrastructure:** Massive power transmission and distribution
- **Waste Management:** Long-term radioactive waste storage and handling
