# ECG Detection PCB Circuit Design

## Overview
This project involves the design of an ECG detection circuit using Altium Designer. The design consists of a schematic for an ECG circuit, component symbols, and PCB footprints. The aim is to create a printed circuit board (PCB) that captures ECG signals using an instrumentation amplifier and processes the data for further analysis.

## Features
- **Instrumentation Amplifier (AD620)**: Used to amplify low-level ECG signals.
- **CMOS Op-Amp (TLV521DCKT)**: For signal conditioning.
- **Capacitors and Resistors**: Proper signal filtering and biasing.
- **Battery Retainer (CR2032)**: Power source for the circuit.

## Project Structure
- **Schematic Document**: Contains the symbols and connections of the ECG circuit.
- **PCB Document**: Defines the PCB layout with the components placed and routed.
- **Schematic Library**: Custom schematic symbols for the project.
- **PCB Library**: PCB footprints for components such as the battery retainer, headers, and amplifiers.

## Components Used
| Component                | Description                          | Part Number        |
|--------------------------|--------------------------------------|--------------------|
| Battery Retainer          | CR2032 Battery Retainer              | BK-913-TR          |
| 3.5mm Stereo Jack         | Audio Jack                           | SJ-3523-SMT-TR     |
| 2-Pin Header              | 2 Position Header                    | TSW-102-07-L-S     |
| 3-Pin Header              | 3 Position Header                    | TSW-103-07-F-S     |
| CMOS Op-Amp               | 1 Circuit Rail-to-Rail SC-70-5       | TLV521DCKT         |
| Instrumentation Amplifier | 1 Circuit 8-SOIC                     | AD620ARZ-REEL7     |
| Capacitor                 | SMD 22PF 200V NP0                    | 08052U220GAT2A     |
| Resistor                  | SMD 3.3K Ohm 1% 1/8W 0805            | CRCW08053K30FKEA   |

## Design Constraints
- **Via Sizes**: 
  - External Via Diameter: 0.6mm
  - Internal Via Diameter: 0.3mm
- **Trace Widths**: 
  - Minimum Width: 0.3mm 
  - Preferred Width: 0.5mm 
  - Maximum Width: 1mm
- **Dielectric Thickness**: 1.6mm
- **Clearance**: Minimum clearance between wires and vias is 0.3mm.

## Workflow
1. **Project Setup**:
   - Create a new Altium project.
   - Add the necessary documents: schematic, PCB, schematic library, and PCB library.
   - Use the created schematic symbols and footprints for the components.
2. **Schematic Design**:
   - Place the components (amplifiers, resistors, capacitors) and interconnect them as per the ECG circuit.
3. **PCB Layout**:
   - Place the PCB footprints on the PCB layout.
   - Route the traces according to the design constraints provided.
4. **Final PCB Design**:
   - Validate the design, ensuring proper routing, via sizes, and clearance.
   - Generate the Gerber files for PCB fabrication.

## Key Circuit Components
- **AD620 Instrumentation Amplifier**: Amplifies the small ECG signals with a high common-mode rejection ratio (CMRR).
- **TLV521DCKT CMOS Op-Amp**: Used for further amplification and filtering of the ECG signal.
- **Capacitors and Resistors**: Provide the necessary filtering and biasing to condition the ECG signal for processing.

## Usage
- The designed ECG circuit is used to capture and process low-level ECG signals for further analysis.
- The PCB can be powered using a CR2032 battery, and the signal can be output via the 3.5mm stereo jack for further processing or display.

## Future Improvements
- Implement more sophisticated signal filtering techniques to reduce noise.
- Design additional stages for real-time ECG signal analysis and processing.
- Miniaturize the PCB design for wearable applications.

## Authors
- Samroz Ahmad Shoaib

---

This document was created based on the Altium PCB project workflow and component selection guidelines provided.
