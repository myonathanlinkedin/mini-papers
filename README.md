# 📄 Mini Papers — Computer Science & Systems Research Journal

<p align="center">
  <a href="https://myonathanlinkedin.github.io/"><img src="https://img.shields.io/badge/Author-Mateus_Yonathan-blue.svg?style=for-the-badge&logo=github" alt="Author" /></a>
  <img src="https://img.shields.io/badge/Cadence-Daily_Publication-00C853.svg?style=for-the-badge" alt="Daily" />
  <img src="https://img.shields.io/badge/Benchmarks-Live_Execution-00C853.svg?style=for-the-badge" alt="Live Benchmarks" />
</p>

---

## 🏛️ About This Journal

This repository publishes daily empirical mini-papers exploring computer systems, algorithmic complexity, memory management, and concurrency architectures across **14 programming languages** (Rust, C++, C, Zig, Swift, Go, Haskell, Kotlin, Java, TypeScript, Python, Ruby, C#, PHP).

### 🔬 Core Methodology:
1. **Empirical Benchmarks**: Performance measurements executed on real hardware/VM runners with mean latencies and throughput.
2. **Systems Architecture**: Detailed breakdown of memory safety, data layouts, lock-free synchronization, and distributed consensus.
3. **Reproducible Code**: Every paper evaluates verified, working algorithmic implementations.

---

## 📑 Published Mini Papers Catalog

| PDF | Folder | Date | Paper Title | Language | Latency / Bounds | Description |
| :---: | :---: | :---: | :--- | :---: | :---: | :--- |
| [📄 PDF](papers/2026-10-10_test_zig_bounded_queue/2026-10-10_test_zig_bounded_queue.pdf) | [📁 Folder](papers/2026-10-10_test_zig_bounded_queue/) | `2026-10-10` | **Cache-Line Contention and Atomic Synchronization in a Lock-Free Memory-Pool Block Allocator with Embedded Free List** | `C` | `10259.6 µs` | Dynamic memory allocation is a fundamental bottleneck in high-throughput multithreaded applications, especially when contention on the global heap leads to c... |
| [📄 PDF](papers/2026-10-10_test_php_stack_vm/2026-10-10_test_php_stack_vm.pdf) | [📁 Folder](papers/2026-10-10_test_php_stack_vm/) | `2026-10-10` | **Layered Distance Propagation and Cache-Line Locality in Zig-Based Hopcroft-Karp Matching** | `Zig` | `AST Bounds` | We present a systems-level implementation of the Hopcroft-Karp maximum bipartite matching algorithm in the Zig programming language, focusing on memory layou... |
| [📄 PDF](papers/2026-10-10_test_cpp_btree_splitter/2026-10-10_test_cpp_btree_splitter.pdf) | [📁 Folder](papers/2026-10-10_test_cpp_btree_splitter/) | `2026-10-10` | **Cache-Friendly Memory Layout and Frequency-Weighted Traversal in Ruby Trie Prefix Trees for Auto-Completion** | `Ruby` | `215508.6 µs` | Auto-completion services rely on prefix trees (tries) to retrieve candidate strings with sub-millisecond latency. Existing designs focus on character-level b... |
| [📄 PDF](papers/2026-10-08_lock_free_concurrent_ring_buffer_da/2026-10-08_lock_free_concurrent_ring_buffer_da.pdf) | [📁 Folder](papers/2026-10-08_lock_free_concurrent_ring_buffer_da/) | `2026-10-08` | **Cache-Line Contention and Atomic Synchronization in a Lock-Free Ring Buffer: An Empirical C Characterization**<br>📄 *[Published Research Paper](papers/2026-10-08_lock_free_concurrent_ring_buffer_da/README.md)* | `C` | `AST Bounds` | Lock-free ring buffers are a cornerstone of high-throughput producer-consumer pipelines, yet their performance on modern x86 cores is tightly coupled to cach... |

---

## 📂 Repository Layout
```
mini-papers/
├── README.md               # Journal Overview & Searchable Catalog
└── papers/
    └── YYYY-MM-DD_<topic>/
        ├── README.md       # Concise Technical Breakdown (Invariants, Benchmarks, RQs)
        └── paper.pdf       # Compiled High-Resolution Publication PDF
```

---

## 👨‍💻 Principal Investigator & Citation
* **Author & Lead Researcher:** [Mateus Yonathan](https://myonathanlinkedin.github.io/)
* **Journal Repository:** [myonathanlinkedin/mini-papers](https://github.com/myonathanlinkedin/mini-papers)
* **License:** MIT Open Research
