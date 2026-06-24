# 🕸️ Dynamics on Scale-Free Networks

**Course: IDC621 | Term Paper 4 | Roll No: MS21107**

A computational study of complex network dynamics, exploring how four distinct mathematical models behave when simulated on **Scale-Free Networks** built using the Barabási–Albert preferential attachment mechanism.

---

## 📌 Project Overview

This project constructs scale-free networks from scratch and studies emergent collective behavior by simulating four dynamical models on top of the network structure:

1. **FitzHugh-Nagumo Model** — Neuronal excitability and spike propagation
2. **Ising Model** — Spin system and magnetic phase transitions
3. **Kuramoto Model** — Phase synchronization among coupled oscillators
4. **Coupled Map Lattice (CML)** — Chaotic dynamics and spatiotemporal patterns

Additionally, the project compares **Scale-Free** and **Small-World** network topologies.

---

## 🔷 Network Construction

### Scale-Free Network (Barabási–Albert Model)
- Built using **preferential attachment** — new nodes connect to existing nodes with probability proportional to their degree.
- Generates a **power-law degree distribution** (hubs with very high connectivity).
- Implemented both from scratch (NumPy adjacency matrix) and via NetworkX (`barabasi_albert_graph`).

### Small-World Network (Watts–Strogatz Model)
- Starts from a regular ring lattice and rewires edges with probability `p`.
- Produces short average path lengths with high clustering coefficients.

---

## 🧠 Dynamical Models

### 1. FitzHugh-Nagumo Model
Models neuronal excitability — simulates how action potentials (spikes) propagate through the network. Nodes represent neurons coupled via the network adjacency matrix.

### 2. Ising Model
A spin system where each node holds a spin (+1 or -1). Simulates magnetic phase transitions — studies how local spin interactions lead to global order or disorder depending on temperature.

### 3. Kuramoto Model
Each node is an oscillator with a natural frequency. The model tracks how coupled oscillators synchronize over time — a fundamental phenomenon in biology, neuroscience, and physics.

### 4. Coupled Map Lattice (CML)
Each node follows a chaotic logistic map, coupled to its neighbors. Explores how chaos spreads and self-organizes across the network topology.

---

## 📊 Visualizations

- **Adjacency Matrix Heatmap** — structural view of network connectivity
- **Degree Distribution (log-log)** — confirms power-law behavior of scale-free networks
- **Circular Layout** — visual layout of nodes and edges
- **Animated Network Growth** — Plotly animation showing preferential attachment step by step (both spring and circular layouts)
- **Population/State Dynamics** — time evolution plots for each dynamical model

---

## 🔑 Key Metrics

| Metric | Description |
|---|---|
| Average Path Length | Mean shortest path between all node pairs |
| Clustering Coefficient | Measure of how interconnected a node's neighbors are |
| Degree Distribution | Frequency of node degrees — power-law for scale-free |

---

## 🛠️ Tech Stack

- **Language:** Python
- **Libraries:** NumPy, NetworkX, Matplotlib, Plotly
- **Network models:** Barabási–Albert (scale-free), Watts–Strogatz (small-world)
- **Environment:** Google Colab

---

## 📁 Repository Structure

```
├── MS21107_termpaper4.ipynb   # Full simulation notebook
└── README.md
```

---

## 🚀 How to Run

1. Open `MS21107_termpaper4.ipynb` in Google Colab.
2. Run all cells sequentially.
3. Interactive Plotly animations (network growth) will render inline — click **Play** to animate.
4. Static Matplotlib plots (degree distribution, adjacency matrix, circular layout) render automatically.

---

## 👤 Author

**MS21107**
GitHub: [ritika3105](https://github.com/ritika3105)
