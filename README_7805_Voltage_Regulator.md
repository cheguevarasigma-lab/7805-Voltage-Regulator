# 7805 Voltage Regulator -- PCB Design

![7805 PCB 3D View](Images/PCB_3D_View.png)

## Project Overview

This project is a 5V regulated DC power supply designed using the
LM7805T linear voltage regulator.

The PCB was designed in EasyEDA Standard using through-hole components
and a single-sided PCB layout. It demonstrates practical skills in
schematic capture, component selection, PCB layout, and
manufacturing-file preparation.

## Project Specifications

  Parameter         Specification
  ----------------- ------------------------
  Project           7805 Voltage Regulator
  Regulator IC      LM7805T
  Intended input    9--12V DC
  Nominal output    5V DC
  PCB type          Single-sided
  Component style   Through-hole
  Design software   EasyEDA Standard

*The usable output current depends on input voltage, regulator
temperature, heatsinking, PCB construction, and the actual load. Verify
thermal performance before operating at higher currents.*

## Components

  Component                 Designator   Value / Type
  ------------------------- ------------ --------------
  Voltage regulator         U1           LM7805T
  Electrolytic capacitors   C1, C2       100µF
  Ceramic capacitor         C3           330nF
  Ceramic capacitor         C4           100nF
  Resistor                  R1           1kΩ
  LED                       LED1         Red, 3mm
  Input connector           P1           2-pin
  Output connector          P2           2-pin

## Working Principle

1.  DC input is connected through P1.
2.  The LM7805T regulates the input to a nominal 5V output.
3.  The input and output capacitors provide local filtering and help
    support regulator stability.
4.  The LED and series resistor provide a visual power indication,
    according to the implemented circuit.
5.  The regulated output is available at P2.

## Design Features

-   LM7805T-based 5V linear regulator
-   Single-sided PCB layout
-   Through-hole components
-   Screw-terminal input and output connectors
-   Input and output filtering capacitors
-   LED power indication
-   EasyEDA 3D PCB view

## Project Files

Place the exported files in the folders below, then update the links if
you use different filenames.

-   [Circuit schematic](Schematic.pdf)
-   [Bill of Materials](BOM.csv)
-   [Gerber manufacturing files](Gerber/Gerber_Files.zip)
-   [PCB 3D view](Images/PCB_3D_View.png)

## Design and Verification Notes

Before ordering the PCB:

-   Verify the LM7805T footprint pin order against the datasheet for the
    exact part being used.
-   Verify electrolytic capacitor polarity and all component footprints
    against the physical parts.
-   Check input and output connector polarity markings.
-   Run EasyEDA DRC and resolve errors and unrouted connections.
-   Inspect the Gerber files in a Gerber viewer.
-   Check regulator temperature and heatsinking for the intended input
    voltage and load current.

## Learning Outcomes

This project provided practical experience with:

-   Linear voltage regulator circuits
-   Electronic component and footprint selection
-   Schematic capture
-   Single-sided PCB layout and routing
-   Design Rule Check (DRC)
-   BOM and Gerber generation
-   PCB 3D visualization

## Project Status

**PCB design and documentation prepared.**

Physical fabrication and hardware testing are not claimed here. Add
photographs, measured input/output voltage, load-test results, and
thermal observations after building and testing the board.

## Author

**cheguevarasigma-lab**

GitHub: https://github.com/cheguevarasigma-lab

------------------------------------------------------------------------

*Part of my practical Electronics and Electrical Engineering project
portfolio.*
