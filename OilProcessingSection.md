# Oil Processing Section Factory - Complete Production Guide

## Production Pipeline Summary

### Sequential Build Order (Standard Recipes Only)
Build your oil processing factory in this order to ensure each step feeds into the next:

**Floor 1: Primary Processing**
1. **Crude Oil → Plastic** (Refineries)
2. **Crude Oil → Rubber** (Refineries)
3. **Crude Oil → Fuel + Polymer Resin** (Refineries)

**Floor 2: Advanced Fuel Processing**
4. **Fuel + Compacted Coal → Turbofuel** (Refineries)
5. **Turbofuel + Nitric Acid → Rocket Fuel** (Blenders)
6. **Rocket Fuel + Power Shards → Ionized Fuel** (Refineries)

**Floor 3: Plastic Applications**
7. **Plastic → Various End Products** (Distributed to other sections)

**Floor 4: Fuel Distribution & Power Generation**
8. **Fuel/Turbofuel → Power Generation** (Fuel Generators)

### Pipeline Flow (Optimized for Minimal Vertical Movement)
```
Floor 1: Crude Oil → [Split 3 ways]
                 ├── Plastic → Electronics Manufacturing
                 ├── Rubber → Various Applications
                 └── Fuel + Polymer Resin → Advanced Fuels
                                          ↓
Floor 2: Fuel → Turbofuel → Rocket Fuel → Ionized Fuel
                                          ↓
Floor 3: Plastic Distribution to Copper Section (665/min required)
                                          ↓
Floor 4: Fuel/Turbofuel → Power Generation (Fuel Generators)
```

### Key Pipeline Notes
- **Start with Crude Oil:** Everything flows from this base resource
- **Floor 1 is the Distribution Hub:** All basic petroleum products made here
- **Plastic is Critical Output:** Essential for electronics manufacturing
- **Fuel Chain Progression:** Each fuel type has higher energy value
- **Major Factory Supplier:** Provides plastic to copper section and power to entire factory
- **Storage Between Floors:** Fluid storage crucial for smooth production

### Optimal Building Ratios for Maximum Throughput

Based on production rates and consumption ratios, here are the ideal building combinations:

#### Starting with 1 Oil Extractor (120 Crude Oil/min):

**Floor 1 - Basic Processing:**
- **Plastic Production:** 2 Refineries (uses 60 crude oil → 40 plastic)
- **Rubber Production:** 1 Refinery (uses 30 crude oil → 20 rubber) 
- **Fuel Production:** 1 Refinery (uses 60 crude oil → 40 fuel + 30 polymer resin)

**Floor 2 - Advanced Fuels:**
- **Turbofuel:** 2 Refineries (uses 45 fuel + 30 compacted coal → 37.5 turbofuel)
- **Rocket Fuel:** 2 Blenders (uses 120 turbofuel + 20 nitric acid → 200 rocket fuel)
- **Ionized Fuel:** 5 Refineries (uses 200 rocket fuel + 12.5 power shards → 200 ionized fuel)

#### Scaling Up - Common Factory Sizes:

**For 4 Oil Extractors (480 Crude Oil/min):**
- **Plastic:** 8 Refineries (160 plastic/min)
- **Rubber:** 4 Refineries (80 rubber/min)
- **Fuel:** 4 Refineries (160 fuel/min + 120 polymer resin/min)
- **Turbofuel:** 8 Refineries (150 turbofuel/min)
- **Rocket Fuel:** 8 Blenders (800 rocket fuel/min)
- **Ionized Fuel:** 20 Refineries (800 ionized fuel/min)

**For 8 Oil Extractors (960 Crude Oil/min):**
- **Plastic:** 16 Refineries (320 plastic/min)
- **Rubber:** 8 Refineries (160 rubber/min)
- **Fuel:** 8 Refineries (320 fuel/min + 240 polymer resin/min)

#### Key Throughput Bottlenecks:
1. **Crude Oil Input:** Limited by oil node capacity and extractor count
2. **Compacted Coal Dependency:** Turbofuel requires coal processing integration
3. **Nitric Acid Requirement:** Rocket fuel needs nitrogen gas processing
4. **Power Shard Supply:** Ionized fuel requires power shard production or collection

#### Building Pairing Strategy:
- **Group Plastic Refineries:** High demand from electronics manufacturing
- **Fuel Processing Chain:** Sequential processing from fuel → turbofuel → rocket fuel → ionized fuel
- **Rubber Production:** Lower priority, supplement as needed
- **Advanced Fuel Storage:** Large fluid storage for complex fuel chains

---

## Overview
This oil processing area transforms crude oil into essential plastics, fuels, and advanced materials. This creates the chemical foundation that powers both electronics manufacturing and the entire factory's energy needs.

---

## Primary Oil Processing

### Plastic Production
**Standard Recipe (Refinery):**
- **Input:** Crude Oil: 30/min
- **Output:** Plastic: 20/min
- **Building:** Refinery
- **Craft Time:** 6 sec
- **Stack Size:** 200
- **Sink Points:** 75
- **Notes:** Essential for electronics manufacturing

### Rubber Production
**Standard Recipe (Refinery):**
- **Input:** Crude Oil: 30/min
- **Output:** Rubber: 20/min
- **Building:** Refinery
- **Craft Time:** 6 sec
- **Stack Size:** 200
- **Sink Points:** 60
- **Notes:** Used in equipment and alternate recipes

### Fuel Production
**Standard Recipe (Refinery):**
- **Input:** Crude Oil: 60/min
- **Output:** Fuel: 40/min + Polymer Resin: 30/min
- **Building:** Refinery
- **Craft Time:** 6 sec
- **Energy Value:** 750 MJ
- **Notes:** Produces both fuel and polymer resin as byproduct

---

## Advanced Fuel Processing

### Turbofuel
- **Input:** Fuel: 22.5/min + Compacted Coal: 15/min
- **Output:** Turbofuel: 18.75/min
- **Building:** Refinery
- **Craft Time:** 16 sec
- **Energy Value:** 2,000 MJ
- **Notes:** 2.67x more efficient than regular fuel

### Rocket Fuel
- **Input:** Turbofuel: 60/min + Nitric Acid: 10/min
- **Output:** Rocket Fuel: 100/min + Compacted Coal: 10/min
- **Building:** Blender
- **Craft Time:** 6 sec
- **Energy Value:** 10,000 MJ
- **Notes:** Ultra-high energy density fuel

### Ionized Fuel
- **Input:** Rocket Fuel: 40/min + Power Shard: 2.5/min
- **Output:** Ionized Fuel: 40/min + Compacted Coal: 5/min
- **Building:** Refinery
- **Craft Time:** 24 sec
- **Energy Value:** 15,000 MJ
- **Notes:** Highest energy fuel in the game

---

## Fuel Energy Comparison

### Energy Density Analysis:
- **Fuel:** 750 MJ (baseline)
- **Turbofuel:** 2,000 MJ (2.67x more efficient)
- **Rocket Fuel:** 10,000 MJ (13.33x more efficient)
- **Ionized Fuel:** 15,000 MJ (20x more efficient)

### Fuel Generator Efficiency:
- **Fuel:** 150 MW per generator
- **Turbofuel:** 400 MW per generator
- **Rocket Fuel:** 2,000 MW per generator
- **Ionized Fuel:** 3,000 MW per generator

---

## Major Applications & Distribution

### Plastic Distribution (Primary Output):
- **Copper Section Electronics:** 665 plastic/min (circuit boards, computers, supercomputers)
- **Equipment Manufacturing:** Various amounts for tools and equipment
- **Alternate Recipes:** Iron plates, reinforced iron plates, etc.

### Fuel Distribution:
- **Power Generation:** Fuel generators throughout factory
- **Vehicle Fuel:** Tractors, trucks, explorers
- **Jetpack Fuel:** Personal mobility

### Rubber Applications:
- **Equipment:** Gas masks, hazmat suits, medical inhalers
- **Alternate Recipes:** Reinforced iron plates, computer alternates
- **Fabric Production:** Combined with mycelia

---

## External Dependencies

### Required Inputs:
- **Crude Oil:** 480+ crude oil/min (multiple oil extractors)
- **Compacted Coal:** For turbofuel production (from coal + sulfur)
- **Nitric Acid:** For rocket fuel (from nitrogen gas + water)
- **Power Shards:** For ionized fuel (from power slugs or synthetic production)

### Critical Integration Points:
- **Coal Processing:** Essential for compacted coal supply
- **Nitrogen Processing:** Required for nitric acid production
- **Power Shard Collection:** Manual collection or synthetic production
- **Water Supply:** Various applications throughout oil processing

---

## Production Ratios for Major Factory Support

### To Support Copper Electronics Section (665 Plastic/min):
- **Oil Extractors:** 25 extractors (25 x 120 = 3,000 crude oil/min)
- **Plastic Refineries:** 50 refineries (using 1,500 crude oil/min)
- **Remaining Oil Capacity:** 1,500 crude oil/min for fuel and rubber production

### Power Generation Capacity:
- **Fuel Production:** 1,000 fuel/min → 10 Fuel Generators → 1,500 MW
- **Turbofuel Production:** 375 turbofuel/min → 10 Fuel Generators → 4,000 MW
- **Rocket Fuel Production:** 1,875 rocket fuel/min → 10 Fuel Generators → 20,000 MW

---

## Storage Requirements

### Recommended Storage per Product:
- **Crude Oil:** 4-6 Fluid Storage Tanks (input buffer)
- **Plastic:** 4-6 Industrial Storage Containers (high consumption)
- **Rubber:** 1-2 Industrial Storage Containers
- **Fuel:** 2-4 Fluid Storage Tanks
- **Turbofuel:** 2-4 Fluid Storage Tanks
- **Rocket Fuel:** 1-2 Fluid Storage Tanks (high energy density)
- **Ionized Fuel:** 1-2 Fluid Storage Tanks (ultra-high energy density)
- **Polymer Resin:** 1-2 Fluid Storage Tanks (byproduct)

---

## Power Requirements

### Estimated Power Consumption for Full Setup:
- **Oil Extractors (25):** 500 MW
- **Refineries (80):** 2,400 MW
- **Blenders (8):** 600 MW
- **Pumps & Infrastructure:** 500 MW
- **Total:** ~4,000 MW

**Power Generation Capability:** 20,000+ MW (net positive by 16,000+ MW)

---

## Factory Integration Strategy

### Phase 1: Basic Plastic Supply
1. **Establish Oil Extraction:** 25+ oil extractors
2. **Plastic Production:** 50+ refineries for electronics support
3. **Basic Fuel Production:** Power generation foundation

### Phase 2: Advanced Fuel Processing
1. **Compacted Coal Integration:** Connect coal processing
2. **Turbofuel Production:** Improved power generation
3. **Nitrogen Integration:** Enable rocket fuel production

### Phase 3: Ultimate Fuel Production
1. **Power Shard Supply:** Collection or synthetic production
2. **Rocket Fuel Chain:** Ultra-high efficiency power
3. **Ionized Fuel Production:** Maximum energy density

### Phase 4: Factory-Wide Power
1. **Fuel Generator Arrays:** Distributed power generation
2. **Power Grid Expansion:** Support entire factory growth
3. **Fuel Export:** Supply vehicle and equipment needs

---

## Expansion Considerations

### Future Upgrades:
1. **Alternate Recipes:** More efficient oil processing methods
2. **Synthetic Production:** Polymer resin applications
3. **Packaging Systems:** Packaged fuel for logistics
4. **Nuclear Transition:** Eventually supplement with nuclear power

### Output Connections:
- **Copper Section:** Essential plastic pipeline (665/min minimum)
- **Iron Section:** Plastic for alternate recipes
- **Steel Section:** Potential plastic applications
- **Power Grid:** Factory-wide fuel generator supply
- **Vehicle Infrastructure:** Fuel distribution for logistics

### Scaling Considerations:
- **Oil Node Limitations:** May require multiple oil fields
- **Pipeline Complexity:** Extensive fluid handling infrastructure
- **Chemical Dependencies:** Integration with coal, nitrogen, and power shard production
- **Power Positive:** Oil processing becomes net power generator for entire factory
