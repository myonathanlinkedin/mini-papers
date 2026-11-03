# LSM-Tree MemTable and SSTable Flush Compaction Engine in C: Structural Tree Invariants and Bounded Search Complexity

[![Publication PDF](https://img.shields.io/badge/Download-Paper_PDF-DC2626?style=flat-square&logo=adobeacrobatreader)](./2026-10-18_lsm_tree_memtable_and_sstable_flush.pdf)

---

## 📌 Executive Abstract & Research Scope
This mini-paper presents a focused, empirical systems characterization of **LSM-Tree MemTable and SSTable Flush Compaction Engine** implemented in **C**. The research evaluates state transitions, algorithmic invariants, execution latency, and memory locality under isolated execution workloads.

* **Engineering Supervisor:** [Mateus Yonathan](https://myonathanlinkedin.github.io/) (Software Engineer)
* **Target Domain:** `lsm`
* **Primary Language Ecosystem:** `C`
* **Publication Date:** `2026-10-18`
* **Source Code Reference:** [c-lowlevel-systems/algorithms/20261018_110144_lsm-tree_memtable_and_sstable](https://github.com/myonathanlinkedin/c-lowlevel-systems/tree/main/algorithms/20261018_110144_lsm-tree_memtable_and_sstable)

---

### 📊 Live Empirical Benchmark Measurements
*Measurements recorded directly on physical CPU execution (INTEL(R) XEON(R) PLATINUM 8573C, 30 iterations)*:

| Metric Parameter | Value | Host Environment |
| :--- | :--- | :--- |
| **Mean Wall-Clock Latency** | `941.79 µs` | Linux 6.17.0-1022-azure |
| **P99 Tail Latency** | `1020.90 µs` | 7.8 GB RAM, 2 Threads |
| **Throughput** | `1,061,808 ops/s` | INTEL(R) XEON(R) PLATINUM 8573C |
| **Verification Status** | `100% Native Compiler Checked` | Release Optimization Enabled |


---

## 🔬 Key Empirical Findings & Takeaways
1. **Physical Hardware Latency & Throughput Bounds**: Isolated execution on INTEL(R) XEON(R) PLATINUM 8573C yields a mean wall-clock latency of 941.79 µs (P99 tail: 1020.90 µs) with sustainable throughput of 1,061,808 ops/sec under native release optimizations.
2. **Empirical Invariant Guarantees**: We have presented a concise C implementation of an LSM-Tree engine that preserves strict ordering invariants while delivering constant-time MemTable operations and logarithmic SSTable lookups.
3. **Domain Architecture Bounds**: The empirical results demonstrate that the design meets the targeted latency and throughput goals on commodity hardware.

---

> ### 📄 Autonomous Research Preprint & Empirical Verification Disclosure
> **Manuscript Attribution, Hardware Traceability & Limitation of Liability:**
> - **Autonomous Formulation:** This manuscript, entitled *"LSM-Tree MemTable and SSTable Flush Compaction Engine in C: Structural Tree Invariants and Bounded Search Complexity"*, was synthesized via autonomous generative agents adhering to strict two-page preprint academic structural conventions.
> - **Hardware Provenance:** Empirical benchmarks cited within this work represent empirically observed hardware performance data captured on an authenticated INTEL(R) XEON(R) PLATINUM 8573C testbed under isolated benchmarking runs.
> - **DISCLAIMER OF CITATION LIABILITY:** THIS PREPRINT IS DISSEMINATED SOLELY FOR SCHOLARLY INQUIRY, PEER DISCUSSION, AND EMPIRICAL COMPARISON. THE AUTHOR AND MAINTAINER MAKE NO REPRESENTATIONS REGARDING FORMAL PERFECTION OR INDUSTRIAL UTILITY. ANY RELIANCE UPON THE ALGORITHMIC PROOFS, COMPLEXITY BOUNDS, OR PERFORMANCE CLAIMS HEREIN IS STRICTLY AT THE READER'S OWN LEGAL AND TECHNICAL RISK.

---

## 📥 Artifacts & Downloads
* 📄 **Download Publication PDF:** [`2026-10-18_lsm_tree_memtable_and_sstable_flush.pdf`](./2026-10-18_lsm_tree_memtable_and_sstable_flush.pdf)

---

## 📖 Citation (BibTeX)
```bibtex
@article{yonathan20261018c,
  author    = {Mateus Yonathan},
  title     = {{LSM-Tree MemTable and SSTable Flush Compaction Engine in C: Structural Tree Invariants and Bounded Search Complexity}},
  journal   = {Daily Mini Papers on Systems Engineering},
  year      = {2026},
  url       = {https://github.com/myonathanlinkedin/c-lowlevel-systems/tree/main/algorithms/20261018_110144_lsm-tree_memtable_and_sstable}
}
```
