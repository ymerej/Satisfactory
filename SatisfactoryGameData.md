# Satisfactory - Ingredients and Parts Data

This file contains production recipes and data for ingredients and parts in Satisfactory.

## Raw Materials / Ingredients

### Iron Ore
- **Source:** Miner on Iron Node
- **Used in:**
  - Iron Ingot (Standard recipe)
  - Iron Alloy Ingot (Alternate)
  - Basic Iron Ingot (Alternate)
  - Leached Iron Ingot (Alternate)
  - Pure Iron Ingot (Alternate)

### Copper Ore
- **Source:** Miner on Copper Node
- **Used in:**
  - Copper Ingot (Standard recipe)
  - Iron Alloy Ingot (Alternate)

### Limestone
- **Source:** Miner on Limestone Node
- **Used in:**
  - Concrete (Standard recipe)
  - Basic Iron Ingot (Alternate)

### Coal
- **Source:** Miner on Coal Node
- **Used in:**
  - Steel Ingot (Standard recipe)
  - Solid Steel Ingot (Alternate)
  - Compacted Coal
  - Gas Filter

### Water
- **Source:** Water Extractor on Water Body
- **Used in:**
  - Concrete (Standard recipe)
  - Pure Iron Ingot (Alternate)
  - Pure Copper Ingot (Alternate)
  - Pure Caterium Ingot (Alternate)
  - Nitric Acid

### Crude Oil
- **Source:** Oil Extractor on Oil Node
- **Used in:**
  - Plastic
  - Rubber
  - Fuel
  - Heavy Oil Residue

### Caterium Ore
- **Source:** Miner on Caterium Node
- **Used in:**
  - Caterium Ingot

### Bauxite
- **Source:** Miner on Bauxite Node
- **Used in:**
  - Alumina Solution
  - Aluminum Scrap

### Raw Quartz
- **Source:** Miner on Quartz Node
- **Used in:**
  - Quartz Crystal
  - Silica

### Sulfur
- **Source:** Miner on Sulfur Node
- **Used in:**
  - Black Powder
  - Sulfuric Acid

### Uranium
- **Source:** Miner on Uranium Node
- **Used in:**
  - Encased Uranium Cell
  - Non-Fissile Uranium

### SAM
- **Source:** SAM Ore Node
- **Used in:**
  - Reanimated SAM

### Nitrogen Gas
- **Source:** Resource Well Extractor on Nitrogen Gas Geyser
- **Used in:**
  - Nitric Acid
  - Cooling System

---

## Basic Materials

### Iron Ingot
- **Inputs:**
  - Iron Ore: 30/min
- **Outputs:**
  - Iron Ingot: 30/min
- **Building:** Smelter
- **Craft Time:** 2 sec

#### Alternate Recipes:
- **Basic Iron Ingot:** 25 Iron Ore + 40 Limestone → 50 Iron Ingot (Foundry, 12 sec)
- **Iron Alloy Ingot:** 40 Iron Ore + 10 Copper Ore → 75 Iron Ingot (Foundry, 12 sec)
- **Pure Iron Ingot:** 35 Iron Ore + 20 Water → 65 Iron Ingot (Refinery, 12 sec)
- **Leached Iron Ingot:** 50 Iron Ore + 10 Sulfuric Acid → 100 Iron Ingot (Refinery, 6 sec)

### Copper Ingot
- **Inputs:**
  - Copper Ore: 30/min
- **Outputs:**
  - Copper Ingot: 30/min
- **Building:** Smelter
- **Craft Time:** 2 sec

### Steel Ingot
- **Inputs:**
  - Iron Ore: 45/min
  - Coal: 45/min
- **Outputs:**
  - Steel Ingot: 45/min
- **Building:** Foundry
- **Craft Time:** 4 sec

#### Alternate Recipes:
- **Solid Steel Ingot:** 40 Iron Ingot + 40 Coal → 60 Steel Ingot (Foundry, 3 sec)

### Concrete
- **Inputs:**
  - Limestone: 45/min
- **Outputs:**
  - Concrete: 15/min
- **Building:** Constructor
- **Craft Time:** 4 sec

---

## Basic Parts

### Iron Plate
- **Inputs:**
  - Iron Ingot: 30/min
- **Outputs:**
  - Iron Plate: 20/min
- **Building:** Constructor
- **Craft Time:** 6 sec
- **Stack Size:** 200
- **Sink Points:** 6

#### Alternate Recipes:
- **Coated Iron Plate:** 37.5 Iron Ingot + 7.5 Plastic → 75 Iron Plate (Assembler, 8 sec)
- **Steel Cast Plate:** 15 Iron Ingot + 15 Steel Ingot → 45 Iron Plate (Foundry, 4 sec)

### Iron Rod
- **Inputs:**
  - Iron Ingot: 15/min
- **Outputs:**
  - Iron Rod: 15/min
- **Building:** Constructor
- **Craft Time:** 4 sec
- **Stack Size:** 200
- **Sink Points:** 2

### Wire
- **Inputs:**
  - Copper Ingot: 15/min
- **Outputs:**
  - Wire: 30/min
- **Building:** Constructor
- **Craft Time:** 4 sec
- **Stack Size:** 500
- **Sink Points:** 6

#### Alternate Recipes:
- **Iron Wire:** 12.5 Iron Ingot → 22.5 Wire (Constructor, 24 sec)

### Cable
- **Inputs:**
  - Wire: 60/min
- **Outputs:**
  - Cable: 30/min
- **Building:** Constructor
- **Craft Time:** 4 sec
- **Stack Size:** 200
- **Sink Points:** 24

### Screw
- **Inputs:**
  - Iron Rod: 10/min
- **Outputs:**
  - Screw: 40/min
- **Building:** Constructor
- **Craft Time:** 6 sec
- **Stack Size:** 500
- **Sink Points:** 2

#### Alternate Recipes:
- **Cast Screws:** 12.5 Iron Ingot → 50 Screws (Constructor, 24 sec)

### Reinforced Iron Plate
- **Inputs:**
  - Iron Plate: 30/min
  - Screw: 60/min
- **Outputs:**
  - Reinforced Iron Plate: 5/min
- **Building:** Assembler
- **Craft Time:** 12 sec
- **Stack Size:** 100
- **Sink Points:** 120

#### Alternate Recipes:
- **Adhered Iron Plate:** 11.25 Iron Plate + 3.75 Rubber → 3.75 Reinforced Iron Plate (Assembler, 16 sec)
- **Bolted Iron Plate:** 90 Iron Plate + 250 Screws → 15 Reinforced Iron Plate (Assembler, 12 sec)
- **Stitched Iron Plate:** 18.75 Iron Plate + 37.5 Wire → 5.625 Reinforced Iron Plate (Assembler, 32 sec)

### Copper Sheet
- **Inputs:**
  - Copper Ingot: 20/min
- **Outputs:**
  - Copper Sheet: 10/min
- **Building:** Constructor
- **Craft Time:** 6 sec
- **Stack Size:** 200
- **Sink Points:** 24

### Steel Beam
- **Inputs:**
  - Steel Ingot: 60/min
- **Outputs:**
  - Steel Beam: 15/min
- **Building:** Constructor
- **Craft Time:** 4 sec
- **Stack Size:** 200
- **Sink Points:** 64

### Steel Pipe
- **Inputs:**
  - Steel Ingot: 30/min
- **Outputs:**
  - Steel Pipe: 20/min
- **Building:** Constructor
- **Craft Time:** 6 sec
- **Stack Size:** 200
- **Sink Points:** 54

#### Alternate Recipes:
- **Iron Pipe:** 100 Iron Ingot → 25 Steel Pipe (Constructor, 12 sec)

### Rotor
- **Inputs:**
  - Iron Rod: 20/min
  - Screw: 100/min
- **Outputs:**
  - Rotor: 4/min
- **Building:** Assembler
- **Craft Time:** 15 sec
- **Stack Size:** 100
- **Sink Points:** 140

### Modular Frame
- **Inputs:**
  - Reinforced Iron Plate: 3/min
  - Iron Rod: 12/min
- **Outputs:**
  - Modular Frame: 2/min
- **Building:** Assembler
- **Craft Time:** 60 sec
- **Stack Size:** 50
- **Sink Points:** 408

---

## Oil Processing Products

### Plastic
- **Inputs:**
  - Crude Oil: 30/min
- **Outputs:**
  - Plastic: 20/min
- **Building:** Refinery
- **Craft Time:** 6 sec
- **Stack Size:** 200
- **Sink Points:** 75

### Rubber
- **Inputs:**
  - Crude Oil: 30/min
- **Outputs:**
  - Rubber: 20/min
- **Building:** Refinery
- **Craft Time:** 6 sec
- **Stack Size:** 200
- **Sink Points:** 60

### Circuit Board
- **Inputs:**
  - Copper Sheet: 15/min
  - Plastic: 30/min
- **Outputs:**
  - Circuit Board: 7.5/min
- **Building:** Assembler
- **Craft Time:** 8 sec
- **Stack Size:** 200
- **Sink Points:** 696

### Fuel
- **Inputs:**
  - Crude Oil: 60/min
- **Outputs:**
  - Fuel: 40/min
  - Polymer Resin: 30/min
- **Building:** Refinery
- **Craft Time:** 6 sec
- **Stack Size:** N/A (Fluid)
- **Energy Value:** 750 MJ

---

## Advanced Components

### Computer
- **Inputs:**
  - Circuit Board: 10/min
  - Cable: 20/min
  - Plastic: 40/min
- **Outputs:**
  - Computer: 2.5/min
- **Building:** Manufacturer
- **Craft Time:** 24 sec
- **Stack Size:** 50
- **Sink Points:** 8,352

#### Alternate Recipes:
- **Caterium Computer:** 15 Circuit Board + 52.5 Quickwire + 22.5 Rubber → 3.75 Computer (Manufacturer, 16 sec)
- **Crystal Computer:** 5 Circuit Board + 1.67 Crystal Oscillator → 3.33 Computer (Assembler, 36 sec)

### Heavy Modular Frame
- **Inputs:**
  - Modular Frame: 5/min
  - Steel Pipe: 15/min
  - Encased Industrial Beam: 5/min
  - Screw: 100/min
- **Outputs:**
  - Heavy Modular Frame: 2/min
- **Building:** Manufacturer
- **Craft Time:** 30 sec
- **Stack Size:** 50
- **Sink Points:** 11,520

### Motor
- **Inputs:**
  - Rotor: 10/min
  - Stator: 10/min
- **Outputs:**
  - Motor: 5/min
- **Building:** Assembler
- **Craft Time:** 12 sec
- **Stack Size:** 50
- **Sink Points:** 1,520

### Stator
- **Inputs:**
  - Steel Pipe: 15/min
  - Wire: 40/min
- **Outputs:**
  - Stator: 5/min
- **Building:** Assembler
- **Craft Time:** 12 sec
- **Stack Size:** 100
- **Sink Points:** 240

### Encased Industrial Beam
- **Inputs:**
  - Steel Beam: 24/min
  - Concrete: 30/min
- **Outputs:**
  - Encased Industrial Beam: 6/min
- **Building:** Assembler
- **Craft Time:** 10 sec
- **Stack Size:** 100
- **Sink Points:** 632

### Adaptive Control Unit
- **Inputs:**
  - Automated Wiring: 5/min
  - Circuit Board: 5/min
  - Heavy Modular Frame: 1/min
  - Computer: 2/min
- **Outputs:**
  - Adaptive Control Unit: 1/min
- **Building:** Manufacturer
- **Craft Time:** 60 sec
- **Stack Size:** 50
- **Sink Points:** 86,120

---

## Aluminum Processing

### Aluminum Ingot
- **Inputs:**
  - Aluminum Scrap: 90/min
  - Silica: 75/min
- **Outputs:**
  - Aluminum Ingot: 60/min
- **Building:** Foundry
- **Craft Time:** 4 sec

### Aluminum Scrap
- **Inputs:**
  - Alumina Solution: 240/min
  - Coal: 120/min
- **Outputs:**
  - Aluminum Scrap: 360/min
  - Water: 120/min
- **Building:** Refinery
- **Craft Time:** 1 sec

### Alumina Solution
- **Inputs:**
  - Bauxite: 120/min
  - Water: 180/min
- **Outputs:**
  - Alumina Solution: 120/min
  - Silica: 50/min
- **Building:** Refinery
- **Craft Time:** 6 sec

### Alclad Aluminum Sheet
- **Inputs:**
  - Aluminum Ingot: 30/min
  - Copper Ingot: 10/min
- **Outputs:**
  - Alclad Aluminum Sheet: 30/min
- **Building:** Assembler
- **Craft Time:** 6 sec

### Aluminum Casing
- **Inputs:**
  - Aluminum Ingot: 90/min
- **Outputs:**
  - Aluminum Casing: 60/min
- **Building:** Constructor
- **Craft Time:** 2 sec

---

## High-Tech Components

### Supercomputer
- **Inputs:**
  - Computer: 7.5/min
  - AI Limiter: 3.75/min
  - High-Speed Connector: 5.625/min
  - Plastic: 52.5/min
- **Outputs:**
  - Supercomputer: 1.875/min
- **Building:** Manufacturer
- **Craft Time:** 32 sec
- **Stack Size:** 50
- **Sink Points:** 99,576

#### Alternate Recipes:
- **Super-State Computer:** 7.2 Computer + 2.4 Electromagnetic Control Rod + 24 Battery + 60 Wire → 2.4 Supercomputer (Manufacturer, 25 sec)

### Radio Control Unit
- **Inputs:**
  - Aluminum Casing: 40/min
  - Crystal Oscillator: 1.25/min
  - Computer: 2.5/min
- **Outputs:**
  - Radio Control Unit: 2.5/min
- **Building:** Manufacturer
- **Craft Time:** 48 sec
- **Stack Size:** 50
- **Sink Points:** 19,312

---

## Quantum Processing & Late Game Items

### Time Crystal
- **Inputs:**
  - Diamonds: 12/min
- **Outputs:**
  - Time Crystal: 6/min
- **Building:** Converter
- **Craft Time:** 10 sec
- **Power:** 100-400 MW

### Dark Matter Residue
- **Inputs:**
  - Reanimated SAM: 50/min
- **Outputs:**
  - Dark Matter Residue: 100/min
- **Building:** Converter
- **Craft Time:** 6 sec
- **Power:** 100-400 MW

### Dark Matter Crystal
- **Inputs:**
  - Diamonds: 30/min
  - Dark Matter Residue: 150/min
- **Outputs:**
  - Dark Matter Crystal: 30/min
- **Building:** Particle Accelerator
- **Craft Time:** 2 sec
- **Power:** 500-1,500 MW

### Excited Photonic Matter
- **Inputs:**
  - (no ingredients listed)
- **Outputs:**
  - Excited Photonic Matter: 200/min
- **Building:** Converter
- **Craft Time:** 3 sec
- **Power:** 100-400 MW

### Neural-Quantum Processor
- **Inputs:**
  - Time Crystal: 15/min
  - Supercomputer: 3/min
  - Ficsite Trigon: 45/min
  - Excited Photonic Matter: 75/min
- **Outputs:**
  - Neural-Quantum Processor: 3/min
  - Dark Matter Residue: 75/min
- **Building:** Quantum Encoder
- **Craft Time:** 20 sec
- **Power:** 0-2,000 MW

### Superposition Oscillator
- **Inputs:**
  - Dark Matter Crystal: 30/min
  - Crystal Oscillator: 5/min
  - Alclad Aluminum Sheet: 45/min
  - Excited Photonic Matter: 125/min
- **Outputs:**
  - Superposition Oscillator: 5/min
  - Dark Matter Residue: 125/min
- **Building:** Quantum Encoder
- **Craft Time:** 12 sec
- **Power:** 0-2,000 MW

### AI Expansion Server
- **Inputs:**
  - Magnetic Field Generator: 4/min
  - Neural-Quantum Processor: 4/min
  - Superposition Oscillator: 4/min
  - Excited Photonic Matter: 100/min
- **Outputs:**
  - AI Expansion Server: 4/min
  - Dark Matter Residue: 100/min
- **Building:** Quantum Encoder
- **Craft Time:** 15 sec
- **Power:** 0-2,000 MW

### Singularity Cell
- **Inputs:**
  - Nuclear Pasta: 1/min
  - Dark Matter Crystal: 20/min
  - Iron Plate: 100/min
  - Concrete: 200/min
- **Outputs:**
  - Singularity Cell: 10/min
- **Building:** Manufacturer
- **Craft Time:** 60 sec

### Ballistic Warp Drive
- **Inputs:**
  - Thermal Propulsion Rocket: 1/min
  - Singularity Cell: 5/min
  - Superposition Oscillator: 2/min
  - Dark Matter Crystal: 40/min
- **Outputs:**
  - Ballistic Warp Drive: 1/min
- **Building:** Manufacturer
- **Craft Time:** 60 sec

### Ficsonium
- **Inputs:**
  - Plutonium Waste: 10/min
  - Singularity Cell: 10/min
  - Dark Matter Residue: 200/min
- **Outputs:**
  - Ficsonium: 10/min
- **Building:** Particle Accelerator
- **Craft Time:** 6 sec
- **Power:** 500-1,500 MW

### Ficsonium Fuel Rod
- **Inputs:**
  - Ficsonium: 5/min
  - Electromagnetic Control Rod: 5/min
  - Ficsite Trigon: 100/min
  - Excited Photonic Matter: 50/min
- **Outputs:**
  - Ficsonium Fuel Rod: 2.5/min
  - Dark Matter Residue: 50/min
- **Building:** Quantum Encoder
- **Craft Time:** 24 sec
- **Power:** 0-2,000 MW

---

## Biomass & Organic Items

### Biomass (Wood)
- **Inputs:**
  - Wood: 60/min
- **Outputs:**
  - Biomass: 300/min
- **Building:** Constructor
- **Craft Time:** 4 sec

### Biomass (Leaves)
- **Inputs:**
  - Leaves: 120/min
- **Outputs:**
  - Biomass: 60/min
- **Building:** Constructor
- **Craft Time:** 5 sec

### Biomass (Mycelia)
- **Inputs:**
  - Mycelia: 15/min
- **Outputs:**
  - Biomass: 150/min
- **Building:** Constructor
- **Craft Time:** 4 sec

### Biomass (Alien Protein)
- **Inputs:**
  - Alien Protein: 15/min
- **Outputs:**
  - Biomass: 1,500/min
- **Building:** Constructor
- **Craft Time:** 4 sec

### Solid Biofuel
- **Inputs:**
  - Biomass: 120/min
- **Outputs:**
  - Solid Biofuel: 60/min
- **Building:** Constructor
- **Craft Time:** 4 sec
- **Stack Size:** 200
- **Sink Points:** 48
- **Energy Value:** 450 MJ

### Liquid Biofuel
- **Inputs:**
  - Solid Biofuel: 90/min
  - Water: 45/min
- **Outputs:**
  - Liquid Biofuel: 60/min
- **Building:** Refinery
- **Craft Time:** 4 sec
- **Energy Value:** 750 MJ

### Alien Protein Processing
- **Hog Protein:**
  - Hog Remains: 20/min → Alien Protein: 20/min (Constructor, 3 sec)
- **Spitter Protein:**
  - Spitter Remains: 20/min → Alien Protein: 20/min (Constructor, 3 sec)
- **Stinger Protein:**
  - Stinger Remains: 20/min → Alien Protein: 20/min (Constructor, 3 sec)
- **Hatcher Protein:**
  - Hatcher Remains: 20/min → Alien Protein: 20/min (Constructor, 3 sec)

### Alien DNA Capsule
- **Inputs:**
  - Alien Protein: 10/min
- **Outputs:**
  - Alien DNA Capsule: 10/min
- **Building:** Constructor
- **Craft Time:** 6 sec

### Fabric
- **Inputs:**
  - Mycelia: 15/min
  - Biomass: 75/min
- **Outputs:**
  - Fabric: 15/min
- **Building:** Assembler
- **Craft Time:** 4 sec
- **Stack Size:** 200
- **Sink Points:** 140

---

## Nuclear Processing

### Uranium Fuel Rod
- **Inputs:**
  - Encased Uranium Cell: 20/min
  - Encased Industrial Beam: 1.2/min
  - Electromagnetic Control Rod: 2/min
- **Outputs:**
  - Uranium Fuel Rod: 0.4/min
- **Building:** Manufacturer
- **Craft Time:** 150 sec

### Uranium Fuel Rod (Burning)
- **Inputs:**
  - Uranium Fuel Rod: 0.2/min
  - Water: 240/min
- **Outputs:**
  - Uranium Waste: 10/min
- **Building:** Nuclear Power Plant
- **Craft Time:** 300 sec
- **Power Output:** 2,500 MW

### Plutonium Pellet
- **Inputs:**
  - Non-Fissile Uranium: 100/min
  - Uranium Waste: 25/min
- **Outputs:**
  - Plutonium Pellet: 30/min
- **Building:** Particle Accelerator
- **Craft Time:** 60 sec
- **Power:** 250-750 MW

### Plutonium Fuel Rod
- **Inputs:**
  - Encased Plutonium Cell: 7.5/min
  - Steel Beam: 4.5/min
  - Electromagnetic Control Rod: 1.5/min
  - Heat Sink: 2.5/min
- **Outputs:**
  - Plutonium Fuel Rod: 0.25/min
- **Building:** Manufacturer
- **Craft Time:** 240 sec

### Plutonium Fuel Rod (Burning)
- **Inputs:**
  - Plutonium Fuel Rod: 0.1/min
  - Water: 240/min
- **Outputs:**
  - Plutonium Waste: 1/min
- **Building:** Nuclear Power Plant
- **Craft Time:** 600 sec
- **Power Output:** 2,500 MW

### Nuclear Pasta
- **Inputs:**
  - Copper Powder: 100/min
  - Pressure Conversion Cube: 0.5/min
- **Outputs:**
  - Nuclear Pasta: 0.5/min
- **Building:** Particle Accelerator
- **Craft Time:** 120 sec
- **Power:** 500-1,500 MW

---

## Caterium Processing

### Caterium Ingot
- **Inputs:**
  - Caterium Ore: 45/min
- **Outputs:**
  - Caterium Ingot: 15/min
- **Building:** Smelter
- **Craft Time:** 4 sec
- **Stack Size:** 100
- **Sink Points:** 42

### Quickwire
- **Inputs:**
  - Caterium Ingot: 12/min
- **Outputs:**
  - Quickwire: 60/min
- **Building:** Constructor
- **Craft Time:** 5 sec
- **Stack Size:** 500
- **Sink Points:** 17

### AI Limiter
- **Inputs:**
  - Copper Sheet: 25/min
  - Quickwire: 100/min
- **Outputs:**
  - AI Limiter: 5/min
- **Building:** Assembler
- **Craft Time:** 12 sec
- **Stack Size:** 100
- **Sink Points:** 920

### High-Speed Connector
- **Inputs:**
  - Quickwire: 210/min
  - Cable: 37.5/min
  - Circuit Board: 3.75/min
- **Outputs:**
  - High-Speed Connector: 3.75/min
- **Building:** Manufacturer
- **Craft Time:** 16 sec
- **Stack Size:** 100
- **Sink Points:** 3,776

---

## Quartz Processing

### Quartz Crystal
- **Inputs:**
  - Raw Quartz: 37.5/min
- **Outputs:**
  - Quartz Crystal: 22.5/min
- **Building:** Constructor
- **Craft Time:** 8 sec
- **Stack Size:** 200
- **Sink Points:** 50

### Silica
- **Inputs:**
  - Raw Quartz: 22.5/min
- **Outputs:**
  - Silica: 37.5/min
- **Building:** Constructor
- **Craft Time:** 8 sec
- **Stack Size:** 200
- **Sink Points:** 20

### Crystal Oscillator
- **Inputs:**
  - Quartz Crystal: 18/min
  - Cable: 14/min
  - Reinforced Iron Plate: 2.5/min
- **Outputs:**
  - Crystal Oscillator: 1/min
- **Building:** Manufacturer
- **Craft Time:** 120 sec
- **Stack Size:** 50
- **Sink Points:** 3,072

---

## Equipment & Tools

These Equipment & Tools are items that are produced in small quantities.  
These items are handheld and 1 needs to be created for the player to hold.

Exceptions include the various Rebar(Iron Rebar, Stun Rebar, Shatter Rebar, and Explosive Rebar).  These are ammo for the Rebar gun.

### Xeno-Zapper
- **Inputs:**
  - Iron Rod: 15/min
  - Reinforced Iron Plate: 3/min
  - Cable: 22.5/min
  - Wire: 75/min
- **Outputs:**
  - Xeno-Zapper: 1.5/min
- **Building:** Equipment Workshop
- **Craft Time:** 20 sec

### Xeno-Basher
- **Inputs:**
  - Xeno-Zapper: 1.5/min
  - Modular Frame: 3.75/min
  - Iron Rod: 18.75/min
  - Wire: 375/min
- **Outputs:**
  - Xeno-Basher: 0.75/min
- **Building:** Equipment Workshop
- **Craft Time:** 40 sec

### Chainsaw
- **Inputs:**
  - Reinforced Iron Plate: 5/min
  - Iron Rod: 25/min
  - Screw: 160/min
  - Cable: 15/min
- **Outputs:**
  - Chainsaw: 1/min
- **Building:** Equipment Workshop
- **Craft Time:** 30 sec

### Object Scanner
- **Inputs:**
  - Reinforced Iron Plate: 6/min
  - Wire: 30/min
  - Screw: 75/min
- **Outputs:**
  - Object Scanner: 1.5/min
- **Building:** Equipment Workshop
- **Craft Time:** 20 sec

### Portable Miner
- **Inputs:**
  - Iron Plate: 3/min
  - Iron Rod: 6/min
- **Outputs:**
  - Portable Miner: 1.5/min
- **Building:** Equipment Workshop
- **Craft Time:** 20 sec

### Rebar Gun
- **Inputs:**
  - Reinforced Iron Plate: 6/min
  - Iron Rod: 16/min
  - Screw: 100/min
- **Outputs:**
  - Rebar Gun: 1/min
- **Building:** Equipment Workshop
- **Craft Time:** 30 sec

### Iron Rebar
- **Inputs:**
  - Iron Rod: 15/min
- **Outputs:**
  - Iron Rebar: 15/min
- **Building:** Constructor
- **Craft Time:** 4 sec

### Stun Rebar
- **Inputs:**
  - Iron Rebar: 10/min
  - Quickwire: 50/min
- **Outputs:**
  - Stun Rebar: 10/min
- **Building:** Assembler
- **Craft Time:** 6 sec

### Shatter Rebar
- **Inputs:**
  - Iron Rebar: 10/min
  - Quartz Crystal: 15/min
- **Outputs:**
  - Shatter Rebar: 5/min
- **Building:** Assembler
- **Craft Time:** 12 sec

### Explosive Rebar
- **Inputs:**
  - Iron Rebar: 10/min
  - Smokeless Powder: 10/min
  - Steel Pipe: 10/min
- **Outputs:**
  - Explosive Rebar: 5/min
- **Building:** Manufacturer
- **Craft Time:** 12 sec

---

## Sulfur Processing & Explosives

### Black Powder
- **Inputs:**
  - Coal: 15/min
  - Sulfur: 15/min
- **Outputs:**
  - Black Powder: 30/min
- **Building:** Assembler
- **Craft Time:** 4 sec

### Smokeless Powder
- **Inputs:**
  - Black Powder: 20/min
  - Heavy Oil Residue: 10/min
- **Outputs:**
  - Smokeless Powder: 20/min
- **Building:** Refinery
- **Craft Time:** 6 sec

### Compacted Coal
- **Inputs:**
  - Coal: 25/min
  - Sulfur: 25/min
- **Outputs:**
  - Compacted Coal: 25/min
- **Building:** Assembler
- **Craft Time:** 12 sec

### Nobelisk
- **Inputs:**
  - Black Powder: 20/min
  - Steel Pipe: 20/min
- **Outputs:**
  - Nobelisk: 10/min
- **Building:** Assembler
- **Craft Time:** 6 sec

### Gas Nobelisk
- **Inputs:**
  - Nobelisk: 5/min
  - Biomass: 50/min
- **Outputs:**
  - Gas Nobelisk: 5/min
- **Building:** Assembler
- **Craft Time:** 12 sec

### Pulse Nobelisk
- **Inputs:**
  - Nobelisk: 5/min
  - Crystal Oscillator: 1/min
- **Outputs:**
  - Pulse Nobelisk: 5/min
- **Building:** Assembler
- **Craft Time:** 60 sec

### Cluster Nobelisk
- **Inputs:**
  - Nobelisk: 7.5/min
  - Smokeless Powder: 10/min
- **Outputs:**
  - Cluster Nobelisk: 2.5/min
- **Building:** Assembler
- **Craft Time:** 24 sec

### Nuke Nobelisk
- **Inputs:**
  - Nobelisk: 2.5/min
  - Encased Uranium Cell: 10/min
  - Smokeless Powder: 5/min
  - AI Limiter: 3/min
- **Outputs:**
  - Nuke Nobelisk: 0.5/min
- **Building:** Manufacturer
- **Craft Time:** 120 sec

### Nobelisk Detonator
- **Inputs:**
  - Object Scanner: 0.75/min
  - Steel Beam: 7.5/min
  - Cable: 37.5/min
- **Outputs:**
  - Nobelisk Detonator: 0.75/min
- **Building:** Equipment Workshop
- **Craft Time:** 40 sec

---

## Advanced Fuels

### Turbofuel
- **Inputs:**
  - Fuel: 22.5/min
  - Compacted Coal: 15/min
- **Outputs:**
  - Turbofuel: 18.75/min
- **Building:** Refinery
- **Craft Time:** 16 sec
- **Energy Value:** 2,000 MJ

### Rocket Fuel
- **Inputs:**
  - Turbofuel: 60/min
  - Nitric Acid: 10/min
- **Outputs:**
  - Rocket Fuel: 100/min
  - Compacted Coal: 10/min
- **Building:** Blender
- **Craft Time:** 6 sec
- **Energy Value:** 10,000 MJ

### Ionized Fuel
- **Inputs:**
  - Rocket Fuel: 40/min
  - Power Shard: 2.5/min
- **Outputs:**
  - Ionized Fuel: 40/min
  - Compacted Coal: 5/min
- **Building:** Refinery
- **Craft Time:** 24 sec
- **Energy Value:** 15,000 MJ

---

## Power Generation Equipment

### Power Shard Processing
- **Blue Power Slug:** 7.5/min → 1 Power Shard: 7.5/min (Constructor, 8 sec)
- **Yellow Power Slug:** 5/min → 2 Power Shard: 10/min (Constructor, 12 sec)
- **Purple Power Slug:** 2.5/min → 5 Power Shard: 12.5/min (Constructor, 24 sec)

### Synthetic Power Shard
- **Inputs:**
  - Time Crystal: 10/min
  - Dark Matter Crystal: 10/min
  - Quartz Crystal: 60/min
  - Excited Photonic Matter: 60/min
- **Outputs:**
  - Power Shard: 5/min
  - Dark Matter Residue: 60/min
- **Building:** Quantum Encoder
- **Craft Time:** 12 sec
- **Power:** 0-2,000 MW

---

## Personal Equipment & Medical

These Personal Equipment & Medical are items that are produced in small quantities.  
They are for supporting the player.  Several of the components only rely on a single run production including Hazmat Suit, Parachute, Blade Runners and Zipline.  
The rest can also be produced manually.

### Gas Mask
- **Inputs:**
  - Fabric: 50/min
  - Copper Sheet: 10/min
  - Steel Pipe: 10/min
- **Outputs:**
  - Gas Mask: 1/min
- **Building:** Equipment Workshop
- **Craft Time:** 30 sec

### Gas Filter
- **Inputs:**
  - Fabric: 15/min
  - Coal: 30/min
  - Iron Plate: 15/min
- **Outputs:**
  - Gas Filter: 7.5/min
- **Building:** Manufacturer
- **Craft Time:** 8 sec

### Iodine-Infused Filter
- **Inputs:**
  - Gas Filter: 3.75/min
  - Quickwire: 30/min
  - Aluminum Casing: 3.75/min
- **Outputs:**
  - Iodine-Infused Filter: 3.75/min
- **Building:** Manufacturer
- **Craft Time:** 16 sec

### Hazmat Suit
- **Inputs:**
  - Rubber: 25/min
  - Plastic: 25/min
  - Alclad Aluminum Sheet: 25/min
  - Fabric: 25/min
- **Outputs:**
  - Hazmat Suit: 0.5/min
- **Building:** Equipment Workshop
- **Craft Time:** 60 sec

### Medicinal Inhalers
- **Nutritional Inhaler:**
  - Bacon Agaric: 3/min + Paleberry: 6/min + Beryl Nut: 15/min → Medicinal Inhaler: 3/min
- **Protein Inhaler:**
  - Alien Protein: 3/min + Beryl Nut: 30/min → Medicinal Inhaler: 3/min
- **Vitamin Inhaler:**
  - Mycelia: 30/min + Paleberry: 15/min → Medicinal Inhaler: 3/min
- **Therapeutic Inhaler:**
  - Mycelia: 45/min + Alien Protein: 3/min + Bacon Agaric: 3/min → Medicinal Inhaler: 3/min

### Parachute
- **Inputs:**
  - Fabric: 30/min
  - Cable: 15/min
- **Outputs:**
  - Parachute: 1.5/min
- **Building:** Equipment Workshop
- **Craft Time:** 20 sec

### Blade Runners
- **Inputs:**
  - Silica: 20/min
  - Modular Frame: 3/min
  - Rotor: 3/min
- **Outputs:**
  - Blade Runners: 1/min
- **Building:** Equipment Workshop
- **Craft Time:** 30 sec

### Zipline
- **Inputs:**
  - Xeno-Zapper: 1.5/min
  - Quickwire: 45/min
  - Iron Rod: 4.5/min
  - Cable: 15/min
- **Outputs:**
  - Zipline: 1.5/min
- **Building:** Equipment Workshop
- **Craft Time:** 20 sec

---

## FICSMAS Seasonal Items

### FICSMAS Gift
- **Source:** FICSMAS event drop from trees and presents
- **Used in:** Various FICSMAS crafting recipes

### FICSMAS Ornaments
- **Blue FICSMAS Ornament:**
  - FICSMAS Gift: 5/min → Blue FICSMAS Ornament: 10/min (Smelter, 12 sec)
- **Red FICSMAS Ornament:**
  - FICSMAS Gift: 5/min → Red FICSMAS Ornament: 5/min (Smelter, 12 sec)
- **Copper FICSMAS Ornament:**
  - Red FICSMAS Ornament: 10/min + Copper Ingot: 10/min → Copper FICSMAS Ornament: 5/min (Foundry, 12 sec)
- **Iron FICSMAS Ornament:**
  - Blue FICSMAS Ornament: 15/min + Iron Ingot: 15/min → Iron FICSMAS Ornament: 5/min (Foundry, 12 sec)

### FICSMAS Ornament Bundle
- **Inputs:**
  - Copper FICSMAS Ornament: 5/min
  - Iron FICSMAS Ornament: 5/min
- **Outputs:**
  - FICSMAS Ornament Bundle: 5/min
- **Building:** Assembler
- **Craft Time:** 12 sec

### FICSMAS Tree Branch
- **Inputs:**
  - FICSMAS Gift: 10/min
- **Outputs:**
  - FICSMAS Tree Branch: 10/min
- **Building:** Constructor
- **Craft Time:** 6 sec

### FICSMAS Bow
- **Inputs:**
  - FICSMAS Gift: 10/min
- **Outputs:**
  - FICSMAS Bow: 5/min
- **Building:** Constructor
- **Craft Time:** 12 sec

### FICSMAS Wreath
- **Inputs:**
  - FICSMAS Tree Branch: 15/min
  - FICSMAS Ornament Bundle: 6/min
- **Outputs:**
  - FICSMAS Wreath: 2/min
- **Building:** Assembler
- **Craft Time:** 60 sec

### FICSMAS Wonder Star
- **Inputs:**
  - FICSMAS Wreath: 5/min
  - Candy Cane: 20/min
- **Outputs:**
  - FICSMAS Wonder Star: 1/min
- **Building:** Assembler
- **Craft Time:** 60 sec

### Candy Cane
- **Inputs:**
  - FICSMAS Gift: 15/min
- **Outputs:**
  - Candy Cane: 5/min
- **Building:** Constructor
- **Craft Time:** 12 sec

### Candy Cane Basher
- **Inputs:**
  - Xeno-Zapper: 1.5/min
  - Candy Cane: 18.75/min
  - FICSMAS Gift: 11.25/min
- **Outputs:**
  - Candy Cane Basher: 0.75/min
- **Building:** Equipment Workshop
- **Craft Time:** 40 sec

### FICSMAS Actual Snow
- **Inputs:**
  - FICSMAS Gift: 25/min
- **Outputs:**
  - FICSMAS Actual Snow: 10/min
- **Building:** Constructor
- **Craft Time:** 12 sec

### Snowball
- **Inputs:**
  - FICSMAS Actual Snow: 15/min
- **Outputs:**
  - Snowball: 5/min
- **Building:** Constructor
- **Craft Time:** 12 sec

---

## Special Vehicles & Equipment

### Factory Cart™
- **Inputs:**
  - Reinforced Iron Plate: 12/min
  - Iron Rod: 12/min
  - Rotor: 6/min
- **Outputs:**
  - Factory Cart™: 3/min
- **Building:** Equipment Workshop
- **Craft Time:** 20 sec
- **Source:** AWESOME Shop

### Golden Factory Cart™
- **Inputs:**
  - Caterium Ingot: 45/min
  - Iron Rod: 12/min
  - Rotor: 6/min
- **Outputs:**
  - Golden Factory Cart™: 3/min
- **Building:** Equipment Workshop
- **Craft Time:** 20 sec
- **Source:** AWESOME Shop

---

## Fireworks

### Fancy Fireworks
- **Inputs:**
  - FICSMAS Tree Branch: 10/min
  - FICSMAS Bow: 7.5/min
- **Outputs:**
  - Fancy Fireworks: 2.5/min
- **Building:** Assembler
- **Craft Time:** 24 sec

### Sparkly Fireworks
- **Inputs:**
  - FICSMAS Tree Branch: 7.5/min
  - FICSMAS Actual Snow: 5/min
- **Outputs:**
  - Sparkly Fireworks: 2.5/min
- **Building:** Assembler
- **Craft Time:** 24 sec

### Sweet Fireworks
- **Inputs:**
  - FICSMAS Tree Branch: 15/min
  - Candy Cane: 7.5/min
- **Outputs:**
  - Sweet Fireworks: 2.5/min
- **Building:** Assembler
- **Craft Time:** 24 sec

---

## Matter Conversion (Tier 9)

### Ore Conversion Recipes
All conversion recipes use the Converter building (6 sec craft time, 100-400 MW power):

#### Iron Ore Conversions
- **Coal to Iron Ore:** Reanimated SAM: 10/min + Coal: 360/min → Iron Ore: 120/min
- **Limestone to Iron Ore:** Reanimated SAM: 10/min + Limestone: 240/min → Iron Ore: 120/min

#### Copper Ore Conversions
- **Quartz to Copper Ore:** Reanimated SAM: 10/min + Raw Quartz: 100/min → Copper Ore: 120/min
- **Sulfur to Copper Ore:** Reanimated SAM: 10/min + Sulfur: 120/min → Copper Ore: 120/min

#### Coal Conversions
- **Iron to Coal:** Reanimated SAM: 10/min + Iron Ore: 180/min → Coal: 120/min
- **Limestone to Coal:** Reanimated SAM: 10/min + Limestone: 360/min → Coal: 120/min

#### Limestone Conversions
- **Sulfur to Limestone:** Reanimated SAM: 10/min + Sulfur: 20/min → Limestone: 120/min

#### Caterium Ore Conversions
- **Copper to Caterium Ore:** Reanimated SAM: 10/min + Copper Ore: 150/min → Caterium Ore: 120/min
- **Quartz to Caterium Ore:** Reanimated SAM: 10/min + Raw Quartz: 120/min → Caterium Ore: 120/min

#### Bauxite Conversions
- **Caterium to Bauxite:** Reanimated SAM: 10/min + Caterium Ore: 150/min → Bauxite: 120/min
- **Copper to Bauxite:** Reanimated SAM: 10/min + Copper Ore: 180/min → Bauxite: 120/min

#### Quartz Conversions
- **Bauxite to Raw Quartz:** Reanimated SAM: 10/min + Bauxite: 100/min → Raw Quartz: 120/min
- **Coal to Raw Quartz:** Reanimated SAM: 10/min + Coal: 240/min → Raw Quartz: 120/min

#### Sulfur Conversions
- **Coal to Sulfur:** Reanimated SAM: 10/min + Coal: 200/min → Sulfur: 120/min
- **Iron to Sulfur:** Reanimated SAM: 10/min + Iron Ore: 300/min → Sulfur: 120/min

#### Nitrogen Gas Conversions
- **Bauxite to Nitrogen Gas:** Reanimated SAM: 10/min + Bauxite: 100/min → Nitrogen Gas: 120/min
- **Caterium to Nitrogen Gas:** Reanimated SAM: 10/min + Caterium Ore: 120/min → Nitrogen Gas: 120/min

#### Uranium Conversions
- **Bauxite to Uranium:** Reanimated SAM: 10/min + Bauxite: 480/min → Uranium: 120/min

---

## Additional Alternate Recipes

### Notable High-Efficiency Alternates

#### Cloudy Diamonds (Alternate)
- **Inputs:**
  - Coal: 240/min
  - Limestone: 480/min
- **Outputs:**
  - Diamonds: 20/min
- **Building:** Particle Accelerator
- **Craft Time:** 3 sec
- **Power:** 250-750 MW

#### Oil-Based Diamonds (Alternate)
- **Inputs:**
  - Crude Oil: 200/min
- **Outputs:**
  - Diamonds: 40/min
- **Building:** Particle Accelerator
- **Craft Time:** 3 sec
- **Power:** 250-750 MW

#### Pink Diamonds (Alternate)
- **Inputs:**
  - Coal: 120/min
  - Quartz Crystal: 45/min
- **Outputs:**
  - Diamonds: 15/min
- **Building:** Converter
- **Craft Time:** 4 sec
- **Power:** 100-400 MW

#### Turbo Diamonds (Alternate)
- **Inputs:**
  - Coal: 600/min
  - Packaged Turbofuel: 40/min
- **Outputs:**
  - Diamonds: 60/min
- **Building:** Particle Accelerator
- **Craft Time:** 3 sec
- **Power:** 250-750 MW

#### Dark-Ion Fuel (Alternate)
- **Inputs:**
  - Packaged Rocket Fuel: 240/min
  - Dark Matter Crystal: 80/min
- **Outputs:**
  - Ionized Fuel: 200/min
  - Compacted Coal: 40/min
- **Building:** Converter
- **Craft Time:** 3 sec
- **Power:** 100-400 MW

---

*Last Updated: Based on latest Satisfactory Wiki data including all major updates through 2024*
