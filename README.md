# Network Simulation using NS-3: Dijkstra Routing and Centrality Measures

This project simulates a network of clients, routers, and servers using NS-3. It implements Dijkstra's algorithm for shortest path routing, computes centrality measures (Degree, Eigenvector, Katz, and PageRank), and integrates RED Active Queue Management on the highest-centrality router.

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Repository Structure](#repository-structure)
4. [How to Run](#how-to-run)
5. [Results](#results)
6. [License](#license)
7. [Acknowledgements](#acknowledgements)

---

## Project Overview
The simulation includes:
- **Dijkstra's Algorithm:** Computes the shortest paths between clients and servers based on delay.
- **Centrality Measures:** Calculates Degree, Eigenvector, Katz, and PageRank centrality for each node.
- **RED Active Queue Management:** Installed on the router with the highest centrality.
- **Tracing and Visualization:** Logs router queue sizes and packet drops, and generates graphs using GNUplot.

---

## Features
- **Network Topology:** Clients, routers, and servers connected via point-to-point links.
- **Shortest Path Routing:** Dijkstra's algorithm ensures optimal paths for data transfer.
- **Centrality Analysis:** Identifies key routers using Degree, Eigenvector, Katz, and PageRank centrality.
- **RED Queue Management:** Improves congestion control on critical routers.
- **Automated Graph Plotting:** Converts trace files into JPEG images using GNUplot.

---

## Repository Structure
```
/Network-Simulation-NS3/
├── /src/          # Source code files
├── /results/      # Generated output files
├── /docs/         # Documentation (optional)
├── README.md      # Project overview and instructions
├── LICENSE        # License file
└── .gitignore     # Ignore unnecessary files
```

---

## How to Run
1. **Prerequisites:**
   - Install [NS-3](https://www.nsnam.org/) on your system.
   - Ensure GNUplot is installed for graph generation.

2. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-username/Network-Simulation-NS3.git
   cd Network-Simulation-NS3
   ```

3. **Build and Run the Simulation:**
   - Copy the `client_server_network25.cc` file to the `scratch/` directory of your NS-3 installation.
   - Build and run the simulation:
     ```bash
     ./waf --run scratch/client_server_network25
     ```

4. **View Results:**
   - The generated trace files (e.g., `queue_router_*.tr`, `drops_router_*.tr`) will be in the `results/` directory.
   - Graphs will be automatically generated as JPEG files.

---

## Results
The simulation generates the following outputs:
- **Trace Files:** Logs of queue sizes and packet drops for each router.
- **Graphs:** Visualizations of queue sizes and packet drops over time.

Example graphs:
- `queue_router_6.jpg`
- `drops_router_6.jpg`

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgements
- **NS-3 Development Team:** For providing the network simulation framework.
- **GNUplot:** For graph generation.
- **Open Source Community:** For inspiration and resources.

---

### LICENSE File
Create a `LICENSE` file in your repository and paste the following:

```text
MIT License

Copyright (c) 2023 Rishikesh T P

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

