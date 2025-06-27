# Adaptive Checkpointer: A √T Approach to Scalable Simulation Rollbacks

📄 **[Read the paper (PDF)](./Practical%20Sublinear%20Checkpointing%20for%20Distributed.pdf)**  
🔗 **Author**: Jean Lauro Muller  
🧪 **Domain**: Distributed Simulation • Checkpointing Systems • Compression • Systems Design

---

## 🚀 Summary

This repository contains the implementation and evaluation code for the paper:

> **"Practical Sublinear Checkpointing for Distributed Simulations"**  
> by **Jean Lauro Muller**

The work introduces a novel closed-loop adaptive checkpointing mechanism with \sqrt{T}-scaled latency, provably improving memory usage and rollback efficiency in large-scale simulation systems.

---

## 🧠 Key Contributions

- ✅ **Adaptive Checkpoint Placement** via exponential smoothing of rollback frequency.
- 📦 **Tiered Storage** strategy: RAM → PMEM → SSD → Cloud (S3).
- 🔒 **Efficient Serialization**: `dill` + `Zstandard`, with 70%+ compression.
- 📊 **Evaluation**: 89% memory reduction with only 15% latency overhead.

---

## 📁 Repository Structure

```bash
.
├── Practical Sublinear Checkpointing for Distributed.pdf   # Full article (LaTeX compiled)
├── README.md                                               # This file
├── src/                                                    # Python source code for the algorithm
├── benchmarks/                                             # Scripts and workload configurations
├── figures/                                                # Graphs and illustrations from the paper
├── requirements.txt                                        # Python dependencies
└── LICENSE                                                 # To be defined (MIT, BSD, etc.)
