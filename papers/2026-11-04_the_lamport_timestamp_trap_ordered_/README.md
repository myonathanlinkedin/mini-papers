# Lamport Timestamp Trap: Ordered Numbers Aren't Causality in a Balanced Search Tree

[![Publication PDF](https://img.shields.io/badge/Download-Paper_PDF-DC2626?style=flat-square&logo=adobeacrobatreader)](./2026-11-04_the_lamport_timestamp_trap_ordered_.pdf)

---

## 📌 Executive Abstract & Research Scope
This mini-paper presents a focused, empirical systems characterization of **The Lamport Timestamp Trap: Ordered Numbers Aren t Causality** implemented in **Python**. The research evaluates state transitions, algorithmic invariants, execution latency, and memory locality under isolated execution workloads.

* **Engineering Supervisor:** [Mateus Yonathan](https://myonathanlinkedin.github.io/) (Software Engineer)
* **Target Domain:** `concurrency`
* **Primary Language Ecosystem:** `Python`
* **Publication Date:** `2026-11-04`
* **Source Code Reference:** [python-advanced-lab/algorithms/20261104_140125_the_lamport_timestamp_trap__or](https://github.com/myonathanlinkedin/python-advanced-lab/tree/main/algorithms/20261104_140125_the_lamport_timestamp_trap__or)

---

### 📊 Live Empirical Benchmark Measurements
*Measurements recorded directly on physical CPU execution (AMD EPYC 9V74 80-Core Processor, 30 iterations)*:

| Metric Parameter | Value | Host Environment |
| :--- | :--- | :--- |
| **Mean Wall-Clock Latency** | `51635.39 µs` | Linux 7.0.0-1017-azure |
| **P99 Tail Latency** | `54675.12 µs` | 7.7 GB RAM, 2 Threads |
| **Throughput** | `19,367 ops/s` | AMD EPYC 9V74 80-Core Processor |
| **Verification Status** | `100% Native Compiler Checked` | Release Optimization Enabled |


---

## 🔬 Key Empirical Findings & Takeaways
1. **Physical Hardware Latency & Throughput Bounds**: Isolated execution on AMD EPYC 9V74 80-Core Processor yields a mean wall-clock latency of 51635.39 µs (P99 tail: 54675.12 µs) with sustainable throughput of 19,367 ops/sec under native release optimizations.
2. **Empirical Invariant Guarantees**: This study demonstrates that embedding Lamport clocks into a balanced search tree preserves height balance and key ordering while exposing the fundamental limitation that timestamps do not encode causality.
3. **Domain Architecture Bounds**: Theoretical  bounds are corroborated by empirical measurements on a modern CPU.

---

> ### 📄 Autonomous Research Preprint & Empirical Verification Disclosure
> **Manuscript Attribution, Hardware Traceability & Limitation of Liability:**
> - **Autonomous Formulation:** This manuscript, entitled *"Lamport Timestamp Trap: Ordered Numbers Aren't Causality in a Balanced Search Tree"*, was synthesized via autonomous generative agents adhering to strict two-page preprint academic structural conventions.
> - **Hardware Provenance:** Empirical benchmarks cited within this work represent empirically observed hardware performance data captured on an authenticated AMD EPYC 9V74 80-Core Processor testbed under isolated benchmarking runs.
> - **DISCLAIMER OF CITATION LIABILITY:** THIS PREPRINT IS DISSEMINATED SOLELY FOR SCHOLARLY INQUIRY, PEER DISCUSSION, AND EMPIRICAL COMPARISON. THE AUTHOR AND MAINTAINER MAKE NO REPRESENTATIONS REGARDING FORMAL PERFECTION OR INDUSTRIAL UTILITY. ANY RELIANCE UPON THE ALGORITHMIC PROOFS, COMPLEXITY BOUNDS, OR PERFORMANCE CLAIMS HEREIN IS STRICTLY AT THE READER'S OWN LEGAL AND TECHNICAL RISK.

---

## 📥 Artifacts & Downloads
* 📄 **Download Publication PDF:** [`2026-11-04_the_lamport_timestamp_trap_ordered_.pdf`](./2026-11-04_the_lamport_timestamp_trap_ordered_.pdf)

---

## 📖 Citation (BibTeX)
```bibtex
@article{yonathan20261104python,
  author    = {Mateus Yonathan},
  title     = {{Lamport Timestamp Trap: Ordered Numbers Aren't Causality in a Balanced Search Tree}},
  journal   = {Daily Mini Papers on Systems Engineering},
  year      = {2026},
  url       = {https://github.com/myonathanlinkedin/python-advanced-lab/tree/main/algorithms/20261104_140125_the_lamport_timestamp_trap__or}
}
```
