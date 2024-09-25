# DSDV Routing Protocol with INET Framework Part - 2

This repository provides the setup and configuration for running the DSDV (Destination-Sequenced Distance-Vector) Routing Protocol simulation using OMNeT++ and the INET Framework. It also includes an additional setup for configuring and running new MANET (Mobile Ad Hoc Network) protocols.

## Table of Contents - Recap

- [Setup OMNeT++](#setup-omnet)
- [Install the INET Framework](#install-the-inet-framework)
- [Add DSDV Project and INET Configuration](#add-dsdv-project-and-inet-configuration)
- [Running the Simulation](#running-the-simulation)
- [Project Structure](#project-structure)
- [Future Enhancements](#future-enhancements)
- [License](#license)

---

## Setup OMNeT++
1. Follow the instructions to install OMNeT++ from the official website:
   - [OMNeT++ Installation Guide](https://omnetpp.org/download/)
   
2. Ensure you have set up OMNeT++ properly on your system by compiling the example projects.

## Install the INET Framework
1. Clone the INET framework from the official repository:
   ```bash
   git clone https://github.com/inet-framework/inet.git
2. Import the INET framework into the OMNeT++ IDE:

Go to File -> Import -> Existing Projects into Workspace.
Select the inet folder and import it as an existing project.
Build the INET framework by right-clicking on the project and selecting Build Project.

## Add DSDV Project and INET Configuration
After setting up the INET framework, proceed with the DSDV project setup:

   1. **Inside the INET framework**:
   - Navigate to the `examples` folder and create an additional folder named `assign`.

2. **Inside the `assign` folder**:
   - Create a new `.ned` file named `ManetProtocolShowcase.ned`.
   - Create a new `.ini` configuration file for the project.

3. **Copy and paste** the required NED and INI configuration codes into the corresponding files.

4. **Ensure the INET framework is built** before running the simulation.

## Example Folder Structure:
```plaintext
DSDV/
inet/
├── examples/
│   └── assign/
│       ├── ManetProtocolShowcase.ned   # The NED file for the MANET simulation
│       ├── omnetpp.ini                 # The INI configuration file
```
## Running the Simulation
  - Navigate to the assign folder in the INET examples directory.
  - Right-click on the omnetpp.ini file within the assign folder.
  - Select Run as OMNeT++ Simulation from the context menu.
    
## Results 
  - After the simulation runs, you can view the performance metrics and graphs in the OMNeT++ IDE, including packet delivery, delays, and throughput for the DSDV protocol.

## License
  - This project is licensed under the MIT License. See the LICENSE file for details.
  - This version includes specific instructions for running the simulation using the `omnetpp.ini` file located in the `assign` folder, ensuring the correct process for simulation execution.
