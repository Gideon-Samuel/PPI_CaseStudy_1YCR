# Residue-Level Analysis of p53–MDM2 Interaction (PDB: 1YCR)

## Background
The p53 tumor suppressor regulates the cell cycle and apoptosis. MDM2 binds the N-terminal domain of p53, promoting its degradation. Disrupting this interaction is a key strategy in cancer therapeutics.

This study computationally analyzes the interface residues between p53 and MDM2, identifies critical hotspots, and simulates a mutation (Trp23 → Ala) to assess its effect on the interaction network.

---

## Objectives
- Identify interface residues between p53 (chain B) and MDM2 (chain A)
- Construct a residue–residue interaction network
- Compute network centrality metrics (degree, betweenness) to detect hubs and bottlenecks
- Simulate a point mutation at p53 residue Trp23 and analyze its effect
- Save node and edge metrics for reproducibility

---

## Methodology
1. **Data Acquisition**
   - PDB: `1YCR`
   - Chains: `A` (MDM2), `B` (p53 peptide)

2. **Interface Detection**
   - Distance cutoff: 5 Å
   - Identify residues in chains A and B in contact

3. **Network Construction**
   - Nodes: interface residues
   - Edges: atom–atom contacts within cutoff
   - Visualization: 2D plots (matplotlib) and optional 3D (Py3Dmol)

4. **Centrality Analysis**
   - Metrics: degree and betweenness centrality
   - Identify hubs (high degree) and bottlenecks (high betweenness)

5. **Mutation Simulation**
   - Remove residue B23 (Trp23 → Ala) from the network
   - Recompute centrality metrics to assess impact

---

## Results
- **Interface Residues**
  - Chain A (MDM2): [example residues]
  - Chain B (p53): [example residues]

- **Top Residues by Degree (Hubs)**
  - [List top hubs before mutation]

- **Top Residues by Betweenness (Bottlenecks)**
  - [List top bottlenecks before mutation]

- **Outputs**
  - `outputs/1YCR_PPI_nodes.csv`
  - `outputs/1YCR_PPI_edges.csv`
---

## How to Run
## Installation

1. **Clone the repository:**

```bash
git clone https://github.com/YOUR_USERNAME/PPI_CaseStudy_1YCR.git
cd PPI_CaseStudy_1YCR
```

2. **Installation Dependencies**

```bash
pip install -r requirements.txt
```
