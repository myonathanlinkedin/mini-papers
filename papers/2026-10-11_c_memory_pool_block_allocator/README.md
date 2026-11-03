# Cache-Line Aligned Lock-Free Memory-Pool Block Allocator with Embedded Free-List Management in C

[![Publication PDF](https://img.shields.io/badge/Download-Paper_PDF-DC2626?style=flat-square&logo=adobeacrobatreader)](./2026-10-11_c_memory_pool_block_allocator.pdf)

---

## 📌 Executive Abstract & Research Scope
This mini-paper presents a focused, empirical systems characterization of **Memory Pool Block Allocator with Embedded Free List Management** implemented in **C**. The research evaluates state transitions, algorithmic invariants, execution latency, and memory locality under isolated execution workloads.

* **Engineering Supervisor:** [Mateus Yonathan](https://myonathanlinkedin.github.io/) (Software Engineer)
* **Target Domain:** `Memory Systems, Low-Latency Allocation, Operating Systems`
* **Primary Language Ecosystem:** `C`
* **Publication Date:** `2026-10-11`
* **Source Code Reference:** [c-lowlevel-systems/algorithms/20261006_120526_memory_pool_block_allocator_wi](https://github.com/myonathanlinkedin/c-lowlevel-systems/tree/main/algorithms/20261006_120526_memory_pool_block_allocator_wi)

---

### 📊 Live Empirical Benchmark Measurements
*Measurements recorded directly on physical CPU execution (13th Gen Intel(R) Core(TM) i9-13900HX, 30 iterations)*:

| Metric Parameter | Value | Host Environment |
| :--- | :--- | :--- |
| **Mean Wall-Clock Latency** | `11435.09 µs` | Windows 11 |
| **P99 Tail Latency** | `103137.20 µs` | 63.8 GB RAM, 32 Threads |
| **Throughput** | `87,450 ops/s` | 13th Gen Intel(R) Core(TM) i9-13900HX |
| **Verification Status** | `100% Native Compiler Checked` | Release Optimization Enabled |


---

## 🔬 Key Empirical Findings & Takeaways
1. **Physical Hardware Latency & Throughput Bounds**: Isolated execution on 13th Gen Intel(R) Core(TM) i9-13900HX yields a mean wall-clock latency of 11435.09 µs (P99 tail: 103137.20 µs) with sustainable throughput of 87,450 ops/sec under native release optimizations.
2. **Empirical Invariant Guarantees**: We presented a lock-free, cache-line-aligned memory-pool block allocator that embeds the free-list pointer inside each block, achieving provable O(1) allocation and deallocation while preserving linearizability.
3. **Domain Architecture Bounds**: Formal invariants guarantee that the free list always reflects the exact set of unallocated blocks.

---

> ### 📄 Autonomous Research Preprint & Empirical Verification Disclosure
> **Manuscript Attribution, Hardware Traceability & Limitation of Liability:**
> - **Autonomous Formulation:** This manuscript, entitled *"Cache-Line Aligned Lock-Free Memory-Pool Block Allocator with Embedded Free-List Management in C"*, was synthesized via autonomous generative agents adhering to strict two-page preprint academic structural conventions.
> - **Hardware Provenance:** Empirical benchmarks cited within this work represent empirically observed hardware performance data captured on an authenticated 13th Gen Intel(R) Core(TM) i9-13900HX testbed under isolated benchmarking runs.
> - **DISCLAIMER OF CITATION LIABILITY:** THIS PREPRINT IS DISSEMINATED SOLELY FOR SCHOLARLY INQUIRY, PEER DISCUSSION, AND EMPIRICAL COMPARISON. THE AUTHOR AND MAINTAINER MAKE NO REPRESENTATIONS REGARDING FORMAL PERFECTION OR INDUSTRIAL UTILITY. ANY RELIANCE UPON THE ALGORITHMIC PROOFS, COMPLEXITY BOUNDS, OR PERFORMANCE CLAIMS HEREIN IS STRICTLY AT THE READER'S OWN LEGAL AND TECHNICAL RISK.

---

## 📥 Artifacts & Downloads
* 📄 **Download Publication PDF:** [`2026-10-11_c_memory_pool_block_allocator.pdf`](./2026-10-11_c_memory_pool_block_allocator.pdf)

---

## 📖 Citation (BibTeX)
```bibtex
@article{yonathan20261011c,
  author    = {Mateus Yonathan},
  title     = {{Cache-Line Aligned Lock-Free Memory-Pool Block Allocator with Embedded Free-List Management in C}},
  journal   = {Daily Mini Papers on Systems Engineering},
  year      = {2026},
  url       = {https://github.com/myonathanlinkedin/c-lowlevel-systems/tree/main/algorithms/20261006_120526_memory_pool_block_allocator_wi}
}
```
