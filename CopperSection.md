# Copper Section Factory - Complete Production Guide

## Production Pipeline Summary

### Sequential Build Order (Standard Recipes Only)
Build your copper factory in this order to ensure each step feeds into the next:

**Floor 1: Primary Processing**
1. **Copper Ore → Copper Ingots** (Smelters)

**Floor 2: Basic Components**
2. **Copper Ingots → Copper Sheets** (Constructors)
3. **Copper Ingots → Wire** (Constructors)

**Floor 3: Intermediate Assembly**
4. **Wire → Cable** (Constructors)
5. **Copper Sheets + Plastic → Circuit Boards** (Assemblers)

**Floor 4: Advanced Components**
6. **Circuit Boards + Plastic → Computers** (Manufacturers)

**Floor 5: Ultra-Advanced Components**
7. **Computers + Plastic → Supercomputers** (Manufacturers)

### Pipeline Flow (Optimized for Minimal Vertical Movement)
```
Floor 1: Copper Ore → Copper Ingots
           ↓
Floor 2: Copper Ingots → [Split 2 ways]
                     ├── Copper Sheets → Circuit Boards
                     └── Wire → Cable
                                          ↓
Floor 3: Copper Sheets + Plastic → Circuit Boards
         Wire → Cable
                                          ↓
Floor 4: Circuit Boards + Plastic → Computers
                                          ↓
Floor 5: Computers + Plastic → Supercomputers
```

### Key Pipeline Notes
- **Start with Copper Ingots:** Everything flows from this base product
- **Floor 2 is the Distribution Hub:** Basic components made here, minimal vertical movement to Floor 3
- **Wire Production is High Volume:** 2:1 output ratio (30 ingots → 60 wire)
- **Circuit Boards are the Bottleneck:** Require plastic input from oil processing
- **Optimized Vertical Flow:** Each floor primarily feeds the next floor up, reducing belt complexity
- **Storage Between Floors:** Place containers between production stages for smooth flow

### Optimal Building Ratios for Maximum Throughput

Based on production rates and consumption ratios, here are the ideal building combinations:

#### Starting with 1 Copper Ingot Smelter (30 Copper Ingots/min):

**Floor 2 - Basic Components:**
- **Copper Sheets:** 1.5 Constructors (uses 30 ingots → 15 sheets)
- **Wire:** 2 Constructors (uses 30 ingots → 60 wire)

**Floor 3 - Intermediate Assembly:**
- **Cable:** 2 Constructors (uses 60 wire → 30 cable)
- **Circuit Boards:** 2 Assemblers (uses 30 copper sheets + 60 plastic → 15 circuit boards)

**Floor 4 - Advanced Components:**
- **Computers:** 6 Assemblers (uses 60 circuit boards + 240 plastic → 15 computers)

#### Scaling Up - Common Factory Sizes:

**For 4 Copper Ore Miners (480 Copper Ore/min = 16 Smelters):**
- **Copper Sheets:** 24 Constructors
- **Wire:** 32 Constructors
- **Cable:** 32 Constructors
- **Circuit Boards:** 32 Assemblers
- **Computers:** 96 Assemblers

**For 1 Copper Ore Miner (120 Copper Ore/min = 4 Smelters):**
- **Copper Sheets:** 6 Constructors
- **Wire:** 8 Constructors
- **Cable:** 8 Constructors
- **Circuit Boards:** 8 Assemblers
- **Computers:** 24 Assemblers

#### Key Throughput Bottlenecks:
1. **Plastic Dependency:** Circuit boards and computers require significant plastic input
2. **Computer Production:** Requires 4:1 ratio of plastic to circuit boards
3. **Circuit Board Craft Time:** 8 seconds - plan production accordingly

#### Building Pairing Strategy:
- **Group Wire Constructors:** High output rate, need multiple constructors
- **Circuit Board Assemblers:** Require plastic input - plan oil processing integration
- **Computer Manufacturers:** Highest plastic consumption - ensure adequate plastic supply

---

## Overview
This copper mine area should focus on producing all items that use copper ore as the primary input. This creates a self-contained copper production hub that can supply electronics to other areas of your factory.

---

## Primary Copper Processing

### Copper Ingot Production
**Standard Recipe (Smelter):**
- **Input:** Copper Ore: 30/min
- **Output:** Copper Ingot: 30/min
- **Building:** Smelter
- **Craft Time:** 2 sec

---

## Basic Copper Parts (Copper Ingot → Basic Components)

### Copper Sheet
- **Input:** Copper Ingot: 20/min
- **Output:** Copper Sheet: 10/min
- **Building:** Constructor
- **Craft Time:** 6 sec
- **Stack Size:** 200
- **Sink Points:** 24

### Wire
- **Input:** Copper Ingot: 15/min
- **Output:** Wire: 30/min
- **Building:** Constructor
- **Craft Time:** 4 sec
- **Stack Size:** 500
- **Sink Points:** 6

---

## Secondary Copper Products (Basic Parts → Advanced Components)

### Cable
- **Input:** Wire: 60/min
- **Output:** Cable: 30/min
- **Building:** Constructor
- **Craft Time:** 4 sec
- **Stack Size:** 200
- **Sink Points:** 24

### Circuit Board
- **Input:** Copper Sheet: 15/min + Plastic: 30/min
- **Output:** Circuit Board: 7.5/min
- **Building:** Assembler
- **Craft Time:** 8 sec
- **Stack Size:** 200
- **Sink Points:** 696
- **Notes:** Requires plastic from oil processing

---

## Advanced Copper Products

### Computer
- **Input:** Circuit Board: 10/min + Plastic: 40/min
- **Output:** Computer: 2.5/min
- **Building:** Manufacturer
- **Craft Time:** 24 sec
- **Stack Size:** 50
- **Sink Points:** 8,352
- **Notes:** High-value product, requires significant plastic input

### Supercomputer
- **Input:** Computer: 7.5/min + Plastic: 52.5/min
- **Output:** Supercomputer: 1.875/min
- **Building:** Manufacturer
- **Craft Time:** 32 sec
- **Stack Size:** 50
- **Sink Points:** 99,576
- **Notes:** Ultra-high-value product, highest plastic consumption

---

## Copper-Based Alternate Recipes (When Available)

### Iron Wire (Alternate)
- **Input:** Iron Ingot: 12.5/min
- **Output:** Wire: 22.5/min
- **Building:** Constructor
- **Craft Time:** 24 sec
- **Notes:** Alternative wire production using iron instead of copper

---

## Equipment & Tools (Copper-Based)

### Xeno-Zapper (Partially Copper)
- **Input:** Iron Rod: 15/min + Wire: 75/min
- **Output:** Xeno-Zapper: 1.5/min
- **Building:** Equipment Workshop
- **Craft Time:** 20 sec
- **Notes:** Primary copper component is wire

### Zipline (Partially Copper)
- **Input:** Xeno-Zapper: 1.5/min + Cable: 15/min
- **Output:** Zipline: 1.5/min
- **Building:** Equipment Workshop
- **Craft Time:** 20 sec

---

## Recommended Production Layout

### Phase 1: Basic Copper Processing
1. **Copper Ore → Copper Ingot** (Multiple Smelters)
2. **Copper Ingot → Copper Sheet** (Constructors)
3. **Copper Ingot → Wire** (Constructors)

### Phase 2: Secondary Processing
1. **Wire → Cable** (Constructors)
2. **Copper Sheet + Plastic → Circuit Board** (Assemblers)

### Phase 3: Advanced Components
1. **Circuit Board + Plastic → Computer** (Manufacturers)

### Phase 4: Ultra-Advanced Components
1. **Computer + Plastic → Supercomputer** (Manufacturers)

### Phase 5: Equipment Production
1. **Wire-based equipment** (Equipment Workshop)

---

## Production Ratios for Efficient Setup

### For 240 Copper Ore/min Input:
- **Copper Ingots:** 240/min (8 Smelters)
- **Copper Sheets:** 80/min (8 Constructors using 160 Copper Ingots)
- **Wire:** 120/min (4 Constructors using 60 Copper Ingots)
- **Cable:** 60/min (2 Constructors using 120 Wire)
- **Circuit Boards:** 40/min (8 Assemblers using 120 Copper Sheets + 240 Plastic)
- **Computers:** 20/min (8 Manufacturers using 80 Circuit Boards + 320 Plastic)
- **Supercomputers:** 3.75/min (2 Manufacturers using 15 Computers + 105 Plastic)

**Plastic Requirement:** 665 Plastic/min total for full copper processing

---

## Storage Requirements

### Recommended Storage per Product:
- **Copper Ore:** 2-3 Industrial Storage Containers
- **Copper Ingots:** 2-3 Industrial Storage Containers
- **Copper Sheets:** 1-2 Industrial Storage Containers
- **Wire:** 2-3 Industrial Storage Containers (high volume)
- **Cable:** 1-2 Industrial Storage Containers
- **Circuit Boards:** 1-2 Industrial Storage Containers
- **Computers:** 1 Industrial Storage Container
- **Plastic:** 3-4 Industrial Storage Containers (high consumption)
- **Supercomputers:** 1 Industrial Storage Container (ultra-high value)

---

## Power Requirements

### Estimated Power Consumption for Full Setup:
- **Smelters (8):** 320 MW
- **Constructors (14):** 560 MW
- **Assemblers (8):** 1,200 MW
- **Manufacturers (8):** 2,200 MW
- **Equipment Workshop (1):** 150 MW
- **Total:** ~4,430 MW

**Recommended:** 6-8 Coal Generators or 2-3 Fuel Generators to power this section

---

## External Dependencies

### Required Inputs from Other Sections:
- **Plastic:** 560/min from oil processing (major dependency)
- **Iron Rods:** For equipment production
- **Optional:** Iron ingots if using Iron Wire alternate recipe

### Integration Points:
- **Oil Processing Plant:** Essential for plastic supply
- **Iron Section:** For equipment and alternate recipes
- **Main Factory Bus:** For distributing computers and circuit boards

---

## Expansion Considerations

### Future Upgrades:
1. **Alternate Recipes:** Unlock more efficient copper processing
2. **Oil Integration:** Establish reliable plastic pipeline
3. **Automation:** Connect to main factory bus system
4. **Advanced Electronics:** Expand to supercomputers and radio control units

### Output Connections:
- **Computers:** Essential for advanced automation and Space Elevator
- **Circuit Boards:** Used in many electronic components
- **Cable:** Basic component for electrical systems
- **Wire:** High-demand component across all electrical production

### Scaling Considerations:
- **Plastic Bottleneck:** Ensure oil processing can support copper section demand
- **High Power Usage:** Plan adequate power generation
- **Complex Ratios:** Copper processing has more complex input/output ratios than iron
