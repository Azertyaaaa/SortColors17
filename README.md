# Project: Color Sorting Machine with TIA Portal V17

## Description
This project is an **automation program developed in TIA Portal V17**, enabling automatic sorting of parts based on their color. Sorting is performed using a **chromatic sensor** and **pneumatic cylinders**, which eject parts into their respective locations.

## Features
- **Color detection**: A chromatic sensor analyzes the light reflection from the parts.
- **Part transportation**: A conveyor belt feeds the system with parts to be sorted.
- **Automatic sorting**: **Pneumatic cylinders** eject parts into their corresponding locations.
- **Flow monitoring**: Light barriers ensure precise tracking of the parts' movement.
- **Adjustable calibration**: Threshold values can be modified for better sorting accuracy.

## Hardware Used
- **Siemens S7-1200 PLC** compatible with TIA Portal V17
- **Chromatic sensor** for color analysis
- **Light barriers** to detect part movement
- **Conveyor belt** driven by a 24V DC motor
- **Pneumatic cylinders** controlled by 1-way solenoids
- **Compressor** to power the pneumatic system

## Operation
1. A part is placed on the conveyor belt.
2. It passes under a **chromatic sensor**, which measures light reflection and determines its color.
3. A **light barrier** validates the presence of the part and activates the ejection system.
4. Depending on the measured color:
   - White part ➔ ejection via **Q3**
   - Red part ➔ ejection via **Q4**
   - Blue part ➔ ejection via **Q5**
5. The part is directed to the corresponding location.

## Installation
1. Open **TIA Portal V17**.
2. Import the project by loading the provided files.
3. Configure the inputs/outputs according to the hardware used.
4. Run the simulation or upload the program to the **Siemens S7-1200 PLC**.

## Included Files
- **Grafcet**: GRAFCET diagram of the system
- **TiaProject-SortColors**: Project source code
- **Docs**: Explanation of functionality and threshold values used

## Possible Improvements
- Adding an **error tracking system** to detect anomalies.
- Integrating an **HMI interface** to adjust sorting parameters.
- Automatic calibration of thresholds for improved accuracy.

**License:** This project is open source under the MIT license. You are free to modify and redistribute it.

