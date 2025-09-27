
# Sorter

A sorting production line that classifies products according to the side of the box. The project is implemented primarily using PLCs.

---

## Table of Contents

- [Overview](#overview)  
- [Features](#features)  
- [Architecture](#architecture)  
- [How It Works](#how-it-works)  
- [Getting Started](#getting-started)  
- [Configuration & Usage](#configuration--usage)  
- [Contributing](#contributing)  
- [Contact](#contact)  

---

## Overview

**Sorter** is designed to automate the classification of products based on which side of their boxes is facing up or down. The system uses programmable logic controllers (PLCs) to make real-time decisions in a production line environment.

---

## Features

- Real-time sorting decisions using PLC logic  
- Ability to detect and classify by box side  
- Modular design to integrate with conveyor systems  
- Logging and monitoring (where supported)  

---

## Architecture

The system is composed of:

1. **Sensors / Input Modules** — detect orientation or side of the box  
2. **PLC Logic** — core decision logic that computes which direction to move the box  
3. **Actuators / Output Modules** — mechanisms (e.g. diverters) that route boxes to appropriate lanes  
4. **Auxiliary Components** — logging, diagnostics, error handling  

---

## How It Works

1. A box enters the detection zone.  
2. Sensors measure which side is facing (e.g. left side, right side, top, bottom).  
3. The PLC reads the sensor inputs and applies logic rules (if side = X then send to lane A, else lane B).  
4. The actuator responds to the PLC command, diverting the box accordingly.  
5. The system logs events (optional) and continues for subsequent boxes.

---

## Getting Started

To run or test this project:

1. Clone the repository  
   ```sh
   git clone https://github.com/georgeyaccoup/Sorter.git


2. Open your PLC development environment (e.g. Siemens TIA Portal, or other depending on target PLC).
3. Import or configure the PLC project files found under `AdditionalFiles/PLCM` (or similar folder).
4. Deploy the logic to your PLC hardware or simulator.
5. Integrate with physical sensors and actuators in the production line.

---

## Configuration & Usage

* Calibrate sensors to detect box side accurately
* Adjust timing delays and actuator response times in the PLC logic
* Monitor logs and system diagnostics to catch misclassifications
* Simulate or test with dummy boxes before running full production

---

## Contributing

Contributions, bug reports, and enhancements are welcome. If you'd like to contribute:

1. Fork the repository
2. Create a feature branch
3. Make your changes, with documentation
4. Submit a pull request

Please follow the existing coding conventions and document any new logic.

## Contact

**Author**: George Read
**LinkedIn**: [George Yaccoup](https://www.linkedin.com/in/george-yaccoup/)

::contentReference[oaicite:0]{index=0}
```
