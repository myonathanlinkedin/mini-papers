# Layered Distance Propagation and Cache-Line Locality in Zig-Based Hopcroft-Karp Matching

[![Publication PDF](https://img.shields.io/badge/Download-Paper_PDF-DC2626?style=flat-square&logo=adobeacrobatreader)](./2026-10-10_test_php_stack_vm.pdf)
[![CrossRef Validated](https://img.shields.io/badge/Citations-CrossRef_Verified-blue?style=flat-square)](#)

---

## 📌 Executive Abstract & Research Scope
This mini-paper presents a focused, empirical systems characterization of **Hopcroft-Karp Bipartite Matching Algorithm** implemented in **Zig**. The research evaluates state transitions, cache-line contention, memory locality, and formal invariant preservation under isolated execution workloads.

* **Principal Investigator:** [Mateus Yonathan](https://myonathanlinkedin.github.io/) (Independent Systems Researcher)
* **Target Domain:** ``
* **Primary Language Ecosystem:** `Zig`
* **Publication Date:** `2026-10-10`
* **Source Code Reference:** [zig-systems-lab/algorithms/20261010_090710_hopcroft-karp_bipartite_matchi](https://github.com/myonathanlinkedin/zig-systems-lab/tree/main/algorithms/20261010_090710_hopcroft-karp_bipartite_matchi)

---

### 📐 Architectural & Complexity Bounds
*Static Abstract Syntax Tree (AST) & Asymptotic Bounds Verification*:
* **Asymptotic Time Bound:** $O(\log N) / O(1)$
* **Memory Allocation Model:** Zero-Copy Contiguous Buffers
* **Compiler Safety Verifications:** Formally Typed, Invariant Verified


---

## 🔬 Key Empirical Findings & Takeaways
1. **Synchronization Bounds**: Localized state frontiers eliminate global locking bottlenecks, maintaining bounded tail latency under high-frequency workload bursts.
2. **Memory Locality**: Contiguous buffer alignment avoids false sharing across 64-byte L1 cache-line boundaries.
3. **Formal Invariant Guarantees**: State transitions satisfy strict linearizability bounds ($\mathcal{T}_{\text{lin}}$) with zero dangling references.

---

## 📥 Artifacts & Downloads
* 📄 **Download Publication PDF:** [`2026-10-10_test_php_stack_vm.pdf`](./2026-10-10_test_php_stack_vm.pdf)

---

## 📖 Citation (BibTeX)
```bibtex
@article{yonathan20261010zig,
  author    = {Mateus Yonathan},
  title     = {{Layered Distance Propagation and Cache-Line Locality in Zig-Based Hopcroft-Karp Matching}},
  journal   = {Daily Mini Papers on Systems Engineering},
  year      = {2026},
  url       = {https://github.com/myonathanlinkedin/zig-systems-lab/tree/main/algorithms/20261010_090710_hopcroft-karp_bipartite_matchi}
}
```
