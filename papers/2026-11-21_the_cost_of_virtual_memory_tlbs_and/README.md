# TLB-Aware Balanced Search Trees: Effective Memory Access Time Analysis in C

[![Publication PDF](https://img.shields.io/badge/Download-Paper_PDF-DC2626?style=flat-square&logo=adobeacrobatreader)](./2026-11-21_the_cost_of_virtual_memory_tlbs_and.pdf)

---

## 📌 Executive Abstract & Research Scope
This mini-paper presents a focused, empirical systems characterization of **The Cost of Virtual Memory: TLBs and Effective Memory Access Time** implemented in **C**. The research evaluates state transitions, algorithmic invariants, execution latency, and memory locality under isolated execution workloads.

* **Engineering Supervisor:** [Mateus Yonathan](https://myonathanlinkedin.github.io/) (Software Engineer)
* **Target Domain:** `concurrency`
* **Primary Language Ecosystem:** `C`
* **Publication Date:** `2026-11-21`
* **Source Code Reference:** [c-lowlevel-systems/algorithms/20261121_050215_the_cost_of_virtual_memory__tl](https://github.com/myonathanlinkedin/c-lowlevel-systems/tree/main/algorithms/20261121_050215_the_cost_of_virtual_memory__tl)

---

### 📊 Live Empirical Benchmark Measurements
*Measurements recorded directly on physical CPU execution (AMD EPYC 7763 64-Core Processor, 30 iterations)*:

| Metric Parameter | Value | Host Environment |
| :--- | :--- | :--- |
| **Mean Wall-Clock Latency** | `798.55 µs` | Linux 7.0.0-1017-azure |
| **P99 Tail Latency** | `2076.77 µs` | 7.7 GB RAM, 2 Threads |
| **Throughput** | `1,252,264 ops/s` | AMD EPYC 7763 64-Core Processor |
| **Verification Status** | `100% Native Compiler Checked` | Release Optimization Enabled |


---

## 🔬 Key Empirical Findings & Takeaways
1. **Physical Hardware Latency & Throughput Bounds**: Isolated execution on AMD EPYC 7763 64-Core Processor yields a mean wall-clock latency of 798.55 µs (P99 tail: 2076.77 µs) with sustainable throughput of 1,252,264 ops/sec under native release optimizations.
2. **Empirical Invariant Guarantees**: We have presented a concise analytical model for EAT in balanced search trees that incorporates TLB hit rates and page-fault overheads.
3. **Domain Architecture Bounds**: The model aligns closely with empirical measurements on a modern AMD EPYC platform, demonstrating its practical relevance.

---

> ### 📄 Autonomous Research Preprint & Empirical Verification Disclosure
> **Manuscript Attribution, Hardware Traceability & Limitation of Liability:**
> - **Autonomous Formulation:** This manuscript, entitled *"TLB-Aware Balanced Search Trees: Effective Memory Access Time Analysis in C"*, was synthesized via autonomous generative agents adhering to strict two-page preprint academic structural conventions.
> - **Hardware Provenance:** Empirical benchmarks cited within this work represent empirically observed hardware performance data captured on an authenticated AMD EPYC 7763 64-Core Processor testbed under isolated benchmarking runs.
> - **DISCLAIMER OF CITATION LIABILITY:** THIS PREPRINT IS DISSEMINATED SOLELY FOR SCHOLARLY INQUIRY, PEER DISCUSSION, AND EMPIRICAL COMPARISON. THE AUTHOR AND MAINTAINER MAKE NO REPRESENTATIONS REGARDING FORMAL PERFECTION OR INDUSTRIAL UTILITY. ANY RELIANCE UPON THE ALGORITHMIC PROOFS, COMPLEXITY BOUNDS, OR PERFORMANCE CLAIMS HEREIN IS STRICTLY AT THE READER'S OWN LEGAL AND TECHNICAL RISK.

---

## 📥 Artifacts & Downloads
* 📄 **Download Publication PDF:** [`2026-11-21_the_cost_of_virtual_memory_tlbs_and.pdf`](./2026-11-21_the_cost_of_virtual_memory_tlbs_and.pdf)

---

## 📖 Citation (BibTeX)
```bibtex
@article{yonathan20261121c,
  author    = {Mateus Yonathan},
  title     = {{TLB-Aware Balanced Search Trees: Effective Memory Access Time Analysis in C}},
  journal   = {Daily Mini Papers on Systems Engineering},
  year      = {2026},
  url       = {https://github.com/myonathanlinkedin/c-lowlevel-systems/tree/main/algorithms/20261121_050215_the_cost_of_virtual_memory__tl}
}
```
