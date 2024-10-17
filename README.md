# Digital VLSI SoC Design and Planning Training

Welcome to the VLSI SoC Design training! In this program, we will cover the essential steps involved in designing an Application Specific Integrated Circuit (ASIC) using an RTL (Register Transfer Level) to GDS (Graphical Data System) flow. The goal is to provide hands-on experience with each step of the digital design process.

## Lessons Learned

### Understanding the RTL to GDS Flow

1. **End-to-End ASIC Flow**: Gained insight into the process of converting RTL descriptions into physical ASIC layouts.
2. **Significance of Each Step**: Recognized the importance of each phase, from synthesis to final sign-off.

### Synthesis
- **Conversion of RTL**: Learned how RTL descriptions are transformed into gate-level netlists using standard cell libraries.
- **Cell Views**: Explored different views of cells such as Liberty, HDL, SPICE, and layout representations.

### Floor and Power Planning
- **Chip Partitioning**: Understood how to allocate space for different components and manage I/O pad placement efficiently.
- **Power Distribution**: Learned about power planning using power rings, straps, and pads to minimize resistance and delay.

## Day 1 Overview

### RTL to GDSII Flow

The RTL to GDSII flow involves multiple stages, starting from RTL synthesis to generating the final GDSII file. This file is used for chip fabrication and contains the physical layout data. Each step ensures that the design meets the intended functionality and adheres to manufacturing constraints.

### Key Stages
- **RTL Synthesis**: Converts the RTL design into a gate-level netlist.
- **Floor Planning**: Allocates space for different components and I/O pads.
- **Placement & Routing**: Determines the positions of cells and routes signal connections between them.
- **Clock Tree Synthesis (CTS)**: Designs a clock network to minimize skew.
- **Sign-off**: Involves physical and timing checks before tape-out.

## QFN-48 Chip: Components and Terminologies

### Core
The core is the area of the chip that houses all the logic elements. It includes both soft and hard IPs (Intellectual Property blocks) and the necessary interconnections.

### Die
The die encompasses the core and the I/O pads. Multiple die patterns are created on a silicon wafer to optimize production.

### IO Pads
I/O pads connect the internal logic of the chip to the external world, allowing for input and output operations.

### IPs
Foundry IPs are customized blocks like SRAM, PLLs, and ADCs, which are essential for the functionality of the chip.

### PDKs
Process Design Kits (PDKs) provide the necessary tools and data for chip designers to model the fabrication process.

## Introduction to RISC-V Architecture

The RISC-V ISA (Instruction Set Architecture) is an open standard that provides the foundation for modern computer architecture. It serves as an interface between high-level software and machine language, enabling the system to execute operations efficiently.

## Hardware-Software Interaction

Understanding how software interacts with hardware is crucial. Between the software applications and the physical hardware, layers like the operating system and system software act as translators, converting human-readable code into machine-executable instructions.

### Key Layers
- **Operating System**: Translates high-level application code into machine code.
- **Compiler**: Converts OS commands into instruction sets for specific hardware.
- **Assembler**: Transforms instruction sets into binary for hardware execution.

## OpenLane Flow: Components and Tools

OpenLane is an open-source ASIC flow that integrates various tools and processes necessary for digital design.

### Key Components
- **RTL Designs**: The foundation of ASIC design, detailing the data flow between hardware components.
- **EDA Tools**: Electronic Design Automation tools like Yosys and OpenROAD are used for design verification.
- **PDK Data**: Foundry-provided data for modeling the fabrication process.

## Simplified RTL to GDS Flow

The RTL to GDS flow comprises several stages, starting from RTL synthesis to physical layout generation in GDSII format.

### Key Stages:
1. **Synthesis**: Transforms RTL code into a gate-level netlist using standard cells.
2. **Floor Planning**: Allocates space for different components while minimizing chip area.
3. **Placement**: Positions components and cells within the defined boundaries.
4. **Clock Tree Synthesis (CTS)**: Designs a clock network to synchronize operations.
5. **Routing**: Connects components using metal layers for signal propagation.
6. **Sign-off**: Conducts verification checks like DRC and LVS to ensure the design is fabrication-ready.

## Detailed OpenLane ASIC Flow

OpenLane integrates open-source tools such as Yosys, Magic, and KLayout to provide a comprehensive digital design flow. It supports the design of fully open-source silicon chips.

## License

This project is licensed under the MIT License - see the [LICENSE](https://choosealicense.com/licenses/mit/) file for details.
