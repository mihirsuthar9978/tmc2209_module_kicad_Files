# TMC2209 Custom KiCad Module

A custom-designed **TMC2209 stepper motor driver module** library for **KiCad**, including a schematic symbol, PCB footprint, and 3D model.

This repository is intended for use in custom PCB designs that integrate a TMC2209 stepper motor driver module.

## Repository Contents

```text
TMC2209-KiCad/
├── README.md
├── Symbols/
│   └── TMC2209_Module.kicad_sym
├── Footprints/
│   └── TMC2209_Module.pretty/
│       └── TMC2209_Module.kicad_mod
├── 3D_Models/
│   └── TMC2209_Module.step
├── Examples/
│   └── TMC2209_Test.kicad_sch
└── Images/
    └── TMC2209_Module.png
```

## Features

* Custom KiCad schematic symbol
* Custom PCB footprint
* TMC2209 module pinout
* Through-hole header pin configuration
* PCB mounting-hole support
* 3D model support
* Suitable for custom stepper motor controller PCBs
* Designed for easy integration into KiCad projects

## TMC2209 Module

The TMC2209 is a Trinamic stepper motor driver commonly used for controlling bipolar stepper motors.

Typical interfaces include:

* STEP
* DIR
* ENABLE
* UART
* VM
* GND
* Motor outputs
* Logic supply

> **Note:** Verify the pinout and mechanical dimensions of your specific TMC2209 module before manufacturing a PCB.

## KiCad Compatibility

The library is intended for use with modern versions of **KiCad 8/9**.

The files can be imported into a KiCad project as custom:

* Symbols
* Footprints
* 3D models

## Installation

### Symbol

Copy the `.kicad_sym` file to your preferred KiCad symbol library location and add the library through:

**KiCad → Preferences → Manage Symbol Libraries**

### Footprint

Add the `.pretty` footprint library through:

**KiCad → Preferences → Manage Footprint Libraries**

Then select:

```text
TMC2209_Module
```

from the footprint chooser.

### 3D Model

Place the 3D model in your preferred KiCad 3D model directory and configure the footprint's 3D model path if required.

## Usage

1. Add the TMC2209 symbol to your schematic.
2. Assign the custom TMC2209 footprint.
3. Connect the motor, power, control, and communication pins.
4. Open the PCB Editor.
5. Update the PCB from the schematic.
6. Verify the footprint and 3D model.
7. Run ERC and DRC before manufacturing.

## Mechanical Information

The footprint is based on the physical dimensions of the custom TMC2209 module used during the design.

Before PCB fabrication, verify:

* Header pin pitch
* Distance between header rows
* Mounting-hole diameter
* Mounting-hole center spacing
* Module dimensions
* Pin numbering
* Board outline

Mechanical dimensions may differ between TMC2209 module manufacturers.

## Disclaimer

This is a **community/custom KiCad library** and is not an official library from Trinamic, Analog Devices, or any TMC2209 module manufacturer.

Always verify the schematic symbol, footprint, pinout, dimensions, and electrical specifications against the datasheet or the exact module being used before manufacturing a PCB.

## License

This project is provided for educational and open-source hardware development purposes.

You may use, modify, and adapt the KiCad library files for your own projects, subject to the terms of the license included in this repository.

## Author

**Mihir Suthar**

Electronics Engineering
KiCad PCB Design & Embedded Systems

---

If you find this library useful, consider giving the repository a ⭐ on GitHub.
