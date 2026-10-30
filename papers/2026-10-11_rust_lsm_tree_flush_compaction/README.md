# Cache-Line Aligned MemTable Layout and Deterministic SSTable Flush Compaction in a Rust LSM-Tree Implementation

[![Publication PDF](https://img.shields.io/badge/Download-Paper_PDF-DC2626?style=flat-square&logo=adobeacrobatreader)](./2026-10-11_rust_lsm_tree_flush_compaction.pdf)

---

## 📌 Executive Abstract & Research Scope
This mini-paper presents a focused, empirical systems characterization of **Log-Structured Merge-Tree (LSM-Tree) MemTable and SSTable Flush Compaction** implemented in **Rust**. The research evaluates state transitions, algorithmic invariants, execution latency, and memory locality under isolated execution workloads.

* **Engineering Supervisor:** [Mateus Yonathan](https://myonathanlinkedin.github.io/) (Software Engineer)
* **Target Domain:** `Storage Engines, Log-Structured Storage, Systems Architecture`
* **Primary Language Ecosystem:** `Rust`
* **Publication Date:** `2026-10-11`
* **Source Code Reference:** [rust-algorithms/algorithms/20261005_053754_lsm-tree_memtable_and_sstable](https://github.com/myonathanlinkedin/rust-algorithms/tree/main/algorithms/20261005_053754_lsm-tree_memtable_and_sstable)

---

### 📊 Live Empirical Benchmark Measurements
*Measurements recorded directly on physical CPU execution (13th Gen Intel(R) Core(TM) i9-13900HX, 30 iterations)*:

| Metric Parameter | Value | Host Environment |
| :--- | :--- | :--- |
| **Mean Wall-Clock Latency** | `15115.62 µs` | Windows 11 |
| **P99 Tail Latency** | `99139.50 µs` | 63.8 GB RAM, 32 Threads |
| **Throughput** | `66,157 ops/s` | 13th Gen Intel(R) Core(TM) i9-13900HX |
| **Verification Status** | `100% Native Compiler Checked` | Release Optimization Enabled |


---

## 🔬 Key Empirical Findings & Takeaways
1. **Physical Hardware Latency & Throughput Bounds**: Isolated execution on 13th Gen Intel(R) Core(TM) i9-13900HX yields a mean wall-clock latency of 15115.62 µs (P99 tail: 99139.50 µs) with sustainable throughput of 66,157 ops/sec under native release optimizations.
2. **Empirical Invariant Guarantees**: We presented a Rust LSM-tree prototype that aligns MemTable nodes to cache lines and enforces deterministic SSTable ordering via a monotonic sequence barrier.
3. **Domain Architecture Bounds**: Formal invariants guarantee total key order and height-balanced B-Tree structure, yielding the classic  lookup bound.

---

> ### 📄 Autonomous Research Preprint & Empirical Verification Disclosure
> **Manuscript Attribution, Hardware Traceability & Limitation of Liability:**
> - **Autonomous Formulation:** This manuscript, entitled *"Cache-Line Aligned MemTable Layout and Deterministic SSTable Flush Compaction in a Rust LSM-Tree Implementation"*, was synthesized via autonomous generative agents adhering to strict two-page preprint academic structural conventions.
> - **Hardware Provenance:** Empirical benchmarks cited within this work represent empirically observed hardware performance data captured on an authenticated 13th Gen Intel(R) Core(TM) i9-13900HX testbed under isolated benchmarking runs.
> - **DISCLAIMER OF CITATION LIABILITY:** THIS PREPRINT IS DISSEMINATED SOLELY FOR SCHOLARLY INQUIRY, PEER DISCUSSION, AND EMPIRICAL COMPARISON. THE AUTHOR AND MAINTAINER MAKE NO REPRESENTATIONS REGARDING FORMAL PERFECTION OR INDUSTRIAL UTILITY. ANY RELIANCE UPON THE ALGORITHMIC PROOFS, COMPLEXITY BOUNDS, OR PERFORMANCE CLAIMS HEREIN IS STRICTLY AT THE READER'S OWN LEGAL AND TECHNICAL RISK.

---

## 📥 Artifacts & Downloads
* 📄 **Download Publication PDF:** [`2026-10-11_rust_lsm_tree_flush_compaction.pdf`](./2026-10-11_rust_lsm_tree_flush_compaction.pdf)

---

## 📖 Citation (BibTeX)
```bibtex
@article{yonathan20261011rust,
  author    = {Mateus Yonathan},
  title     = {{Cache-Line Aligned MemTable Layout and Deterministic SSTable Flush Compaction in a Rust LSM-Tree Implementation}},
  journal   = {Daily Mini Papers on Systems Engineering},
  year      = {2026},
  url       = {https://github.com/myonathanlinkedin/rust-algorithms/tree/main/algorithms/20261005_053754_lsm-tree_memtable_and_sstable}
}
```
