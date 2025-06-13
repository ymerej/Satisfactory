# Iron Section Factory - Complete Production Guide

## Production Pipeline Summary

### Sequential Build Order (Standard Recipes Only)
Build your iron factory in this order to ensure each step feeds into the next:

**Floor 1: Primary Processing**
1. **Iron Ore → Iron Ingots** (Smelters)

**Floor 2: Basic Components**
2. **Iron Ingots → Iron Plates** (Constructors)
3. **Iron Ingots → Iron Rods** (Constructors)
4. **Iron Rods → Screws** (Constructors)
5. **Iron Rods → Iron Rebar** (Constructors)

**Floor 3: Intermediate Assembly**
6. **Iron Plates + Screws → Reinforced Iron Plates** (Assemblers)
7. **Iron Rods + Screws → Rotors** (Assemblers)

**Floor 4: Final Assembly**
8. **Reinforced Iron Plates + Iron Rods → Modular Frames** (Assemblers)
9. **Iron Plates + Iron Rods → Portable Miners** (Equipment Workshop)

### Pipeline Flow (Optimized for Minimal Vertical Movement)
```
Floor 1: Iron Ore → Iron Ingots
           ↓
Floor 2: Iron Ingots → [Split 3 ways]
                   ├── Iron Plates ────────┐
                   ├── Iron Rods → Screws ─┤
                   └── Iron Rods ──────────┤
                                          ↓
Floor 3: Iron Plates + Screws → Reinforced Iron Plates
         Iron Rods + Screws → Rotors
                                          ↓
Floor 4: Reinforced Iron Plates + Iron Rods → Modular Frames
         Iron Plates + Iron Rods → Portable Miners
```

### Key Pipeline Notes
- **Start with Iron Ingots:** Everything flows from this base product
- **Floor 2 is the Distribution Hub:** All basic components made here, minimal vertical movement to Floor 3
- **Screw Production is Critical:** Keep screws close to where they're used (Floor 2→3)
- **Reinforced Iron Plates are the Bottleneck:** They take the longest to craft (12 sec)
- **Optimized Vertical Flow:** Each floor primarily feeds the next floor up, reducing belt complexity
- **Storage Between Floors:** Place containers between production stages for smooth flow

---

## Overview
This iron mine area should focus on producing all items that use iron ore as the primary input. This creates a self-contained iron production hub that can supply other areas of your factory.

---

## Primary Iron Processing

### Iron Ingot Production
**Standard Recipe (Smelter):**
- **Input:** Iron Ore: 30/min
- **Output:** Iron Ingot: 30/min
- **Building:** Smelter
- **Craft Time:** 2 sec

**Alternate Recipes (Optional - require other materials):**
- **Pure Iron Ingot:** 35 Iron Ore + 20 Water → 65 Iron Ingot (Refinery)
- **Basic Iron Ingot:** 25 Iron Ore + 40 Limestone → 50 Iron Ingot (Foundry)
- **Iron Alloy Ingot:** 40 Iron Ore + 10 Copper Ore → 75 Iron Ingot (Foundry)
- **Leached Iron Ingot:** 50 Iron Ore + 10 Sulfuric Acid → 100 Iron Ingot (Refinery)

---

## Basic Iron Parts (Iron Ingot → Basic Components)

### Iron Plate
- **Input:** Iron Ingot: 30/min
- **Output:** Iron Plate: 20/min
- **Building:** Constructor
- **Craft Time:** 6 sec
- **Stack Size:** 200
- **Sink Points:** 6

### Iron Rod
- **Input:** Iron Ingot: 15/min
- **Output:** Iron Rod: 15/min
- **Building:** Constructor
- **Craft Time:** 4 sec
- **Stack Size:** 200
- **Sink Points:** 2

### Iron Rebar
- **Input:** Iron Rod: 15/min
- **Output:** Iron Rebar: 15/min
- **Building:** Constructor
- **Craft Time:** 4 sec

---

## Secondary Iron Products (Basic Parts → Advanced Components)

### Screw
- **Input:** Iron Rod: 10/min
- **Output:** Screw: 40/min
- **Building:** Constructor
- **Craft Time:** 6 sec
- **Stack Size:** 500
- **Sink Points:** 2

**Alternate Recipe:**
- **Cast Screws:** 12.5 Iron Ingot → 50 Screws (Constructor, 24 sec)

### Reinforced Iron Plate
- **Input:** Iron Plate: 30/min + Screw: 60/min
- **Output:** Reinforced Iron Plate: 5/min
- **Building:** Assembler
- **Craft Time:** 12 sec
- **Stack Size:** 100
- **Sink Points:** 120

---

## Advanced Iron Products

### Modular Frame
- **Input:** Reinforced Iron Plate: 3/min + Iron Rod: 12/min
- **Output:** Modular Frame: 2/min
- **Building:** Assembler
- **Craft Time:** 60 sec
- **Stack Size:** 50
- **Sink Points:** 408

### Rotor
- **Input:** Iron Rod: 20/min + Screw: 100/min
- **Output:** Rotor: 4/min
- **Building:** Assembler
- **Craft Time:** 15 sec
- **Stack Size:** 100
- **Sink Points:** 140

---

## Iron-Based Alternate Recipes (When Available)

### Wire (Iron Wire Alternate)
- **Input:** Iron Ingot: 12.5/min
- **Output:** Wire: 22.5/min
- **Building:** Constructor
- **Craft Time:** 24 sec
- **Notes:** Alternative to copper-based wire production

### Steel Pipe (Iron Pipe Alternate)
- **Input:** Iron Ingot: 100/min
- **Output:** Steel Pipe: 25/min
- **Building:** Constructor
- **Craft Time:** 12 sec
- **Notes:** Alternative to steel-based pipe production

---

## Equipment & Tools (Iron-Based)

### Portable Miner
- **Input:** Iron Plate: 3/min + Iron Rod: 6/min
- **Output:** Portable Miner: 1.5/min
- **Building:** Equipment Workshop
- **Craft Time:** 20 sec

### Xeno-Zapper (Partially Iron)
- **Input:** Iron Rod: 15/min + Wire: 75/min
- **Output:** Xeno-Zapper: 1.5/min
- **Building:** Equipment Workshop
- **Craft Time:** 20 sec
- **Notes:** Requires wire (copper-based unless using Iron Wire alternate)

---

## Recommended Production Layout

### Phase 1: Basic Iron Processing
1. **Iron Ore → Iron Ingot** (Multiple Smelters)
2. **Iron Ingot → Iron Plate** (Constructors)
3. **Iron Ingot → Iron Rod** (Constructors)

### Phase 2: Secondary Processing
1. **Iron Rod → Screw** (Constructors)
2. **Iron Rod → Iron Rebar** (Constructors)
3. **Iron Plate + Screw → Reinforced Iron Plate** (Assemblers)

### Phase 3: Advanced Components
1. **Reinforced Iron Plate + Iron Rod → Modular Frame** (Assemblers)
2. **Iron Rod + Screw → Rotor** (Assemblers)

### Phase 4: Equipment Production
1. **Iron Plate + Iron Rod → Portable Miner** (Equipment Workshop)

---

## Production Ratios for Efficient Setup

### For 240 Iron Ore/min Input:
- **Iron Ingots:** 240/min (8 Smelters)
- **Iron Plates:** 80/min (4 Constructors using 120 Iron Ingots)
- **Iron Rods:** 120/min (8 Constructors using 120 Iron Ingots)
- **Screws:** 240/min (6 Constructors using 60 Iron Rods)
- **Reinforced Iron Plates:** 10/min (2 Assemblers using 60 Iron Plates + 120 Screws)
- **Modular Frames:** 3.33/min (2 Assemblers using 6 Reinforced Iron Plates + 24 Iron Rods)
- **Rotors:** 9.6/min (3 Assemblers using 48 Iron Rods + 240 Screws)

---

## Storage Requirements

### Recommended Storage per Product:
- **Iron Ore:** 2-3 Industrial Storage Containers
- **Iron Ingots:** 2-3 Industrial Storage Containers  
- **Iron Plates:** 1-2 Industrial Storage Containers
- **Iron Rods:** 1-2 Industrial Storage Containers
- **Screws:** 2-3 Industrial Storage Containers (high consumption rate)
- **Reinforced Iron Plates:** 1 Industrial Storage Container
- **Modular Frames:** 1 Industrial Storage Container
- **Rotors:** 1 Industrial Storage Container

---

## Power Requirements

### Estimated Power Consumption for Full Setup:
- **Smelters (8):** 320 MW
- **Constructors (18):** 720 MW
- **Assemblers (7):** 1,050 MW
- **Equipment Workshop (1):** 150 MW
- **Total:** ~2,240 MW

**Recommended:** 3-4 Coal Generators or 1-2 Fuel Generators to power this section

---

## Expansion Considerations

### Future Upgrades:
1. **Alternate Recipes:** Unlock and implement more efficient iron processing
2. **Steel Integration:** Add coal input for steel production
3. **Automation:** Connect to main factory bus system
4. **Quality of Life:** Add hyper tubes and vehicles for easy access

### Output Connections:
- **Modular Frames:** Essential for Space Elevator and advanced construction
- **Reinforced Iron Plates:** Used in many advanced recipes
- **Iron Plates/Rods:** Basic components for all factory areas
- **Screws:** High-demand component across all production lines

---

### Optimal Building Ratios for Maximum Throughput

Based on production rates and consumption ratios, here are the ideal building combinations:

#### Starting with 1 Iron Ingot Smelter (30 Iron Ingots/min):

**Floor 2 - Basic Components:**
- **Iron Plates:** 1 Constructor (uses 30 ingots → 20 plates)
- **Iron Rods:** 2 Constructors (uses 30 ingots → 30 rods total)
- **Screws:** 3 Constructors (uses 30 rods → 120 screws total)
- **Iron Rebar:** 1 Constructor (uses 15 rods → 15 rebar)

**Floor 3 - Intermediate Assembly:**
- **Reinforced Iron Plates:** 1 Assembler (uses 30 plates + 60 screws → 5 reinforced plates)
- **Rotors:** 1 Assembler (uses 20 rods + 100 screws → 4 rotors)

**Floor 4 - Final Assembly:**
- **Modular Frames:** 1 Assembler (uses 3 reinforced plates + 12 rods → 2 modular frames)

#### Scaling Up - Common Factory Sizes:

**For 4 Iron Ore Miners (480 Iron Ore/min = 16 Smelters):**
- **Iron Plates:** 16 Constructors
- **Iron Rods:** 32 Constructors  
- **Screws:** 48 Constructors
- **Reinforced Iron Plates:** 16 Assemblers
- **Rotors:** 16 Assemblers
- **Modular Frames:** 16 Assemblers

**For 1 Iron Ore Miner (120 Iron Ore/min = 4 Smelters):**
- **Iron Plates:** 4 Constructors
- **Iron Rods:** 8 Constructors
- **Screws:** 12 Constructors
- **Reinforced Iron Plates:** 4 Assemblers
- **Rotors:** 4 Assemblers
- **Modular Frames:** 4 Assemblers

#### Key Throughput Bottlenecks:
1. **Screw Production:** Always needs the most constructors (3:1 ratio vs iron rods)
2. **Iron Rod Splitting:** Need to split iron rod output between screws, rotors, and modular frames
3. **Reinforced Iron Plates:** Longest craft time (12 sec) - consider this your limiting factor

#### Building Pairing Strategy:
- **Group Screw Constructors:** Place 3+ screw constructors together for efficient belt management
- **Iron Rod Distribution:** Use splitters to divide iron rod output efficiently
- **Assembler Timing:** Reinforced iron plates are your bottleneck - plan other production around this timing