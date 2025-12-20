# Min-Conflict Heuristic for Maximum Clique Detection in Keller Graphs

This repository provides an implementation of a **Diversified Min-Conflict Heuristic** for solving the **Maximum Clique Problem (MCP)** on **Keller graphs**.

The method is described in the preprint:

**A Diversified Min-Conflict Heuristic for Finding Maximum Cliques in Keller Graphs**  
Zine El Abidine Bouneb  
Oum El Bouaghi University, Algeria

The algorithm combines a **bitwise-optimized Non-Adjacency Mask (NAM)** representation with a **stochastic multi-start Min-Conflict strategy**, enabling **O(1) adjacency checks** and robust escape from local optima.  
On **Keller-4 (G(4))**, it achieves **100% success** and **100% diversity**.

---

## 🚀 Key Features

- Bitwise Non-Adjacency Mask (NAM) for constant-time conflict checks
- Stochastic Min-Conflict descent with strict improvement rule
- Multi-start framework to avoid local minima
- 100% success rate on Keller-4 (G(4))
- Each run finds a *different* maximum clique

---

## 📊 Keller-4 (G(4)) Results

- **Maximum clique size:** 12  
- **Mean runtime:** ~0.046 s  
- **Success rate:** 100%  
- **Diversity:** 100/100 unique maximum cliques  

---

## 📁 Main Files

- `minconflictpapercode.ipynb` – Core implementation (Jupyter Notebook)
- `keller_codes_d4.data` – Precomputed Non-Adjacency Masks for G(4)
- `keller4_adjacency.txt` – Full adjacency list (verification)
- `keller4_coordinates.txt` – 4D coordinate mapping of vertices
- `ExampleofSolutionValidatedByHand.pdf` – Manually validated solution

---

## ▶️ How to Run

Requirements:
- Python 3.8+
- Jupyter Notebook / JupyterLab
- No external libraries

Run:
```bash
jupyter notebook minconflictpapercode.ipynb
---

📚 Citation

If you use this code or method, please cite:

@article{bouneb2025minconflict,
  title   = {A Diversified Min-Conflict Heuristic for Finding Maximum Cliques in Keller Graphs},
  author  = {Bouneb, Zine El Abidine},
  journal = {Preprint submitted to Discrete Applied Mathematics, Elsevier},
  year    = {2025}
}
---
🤝 Contact

Zine El Abidine Bouneb
Oum El Bouaghi University, Algeria
Email: bouneb.zineabidine@univ-oeb.dz
