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
/Network-Simulation-NS3/
├── /src/ # Source code files
├── /results/ # Generated output files
├── /docs/ # Documentation (optional)
├── README.md # Project overview and instructions
├── LICENSE # License file
└── .gitignore # Ignore unnecessary file
