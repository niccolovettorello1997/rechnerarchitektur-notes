# Chapter 3 – Performance and Performance Improvement

## Sections

1. Declaring Computational Performance
2. Caching

   * Read Caching
   * Write Caching
   * Cacheable Area
   * Cache Hierarchy
3. Pipelining

---

## Summary

This chapter focuses on how computer performance is measured and improved. It covers metrics for computational performance, the role of caching in speeding up memory access, and pipelining techniques in the CPU. Understanding these mechanisms is critical for designing fast and efficient computer systems.

---

## Key Concepts

### Declaring Computational Performance

* Performance is measured by:

  * **Clock frequency** (Hz) – cycles per second.
  * **MIPS/FLOPS** – instructions or floating-point operations per second.
  * **Execution time** – time to complete a task.
* Performance depends on **hardware, software, and algorithm efficiency**.
* Real-world benchmarks are necessary because raw metrics may be misleading.

### Caching

#### Read Caching

* Frequently accessed data is stored in **fast, small memory** (cache) to reduce access time.
* Reduces latency when the CPU requests the same data repeatedly.

#### Write Caching

* Updates are first written to cache, then later written back to main memory.
* Improves write performance while maintaining data consistency.

#### Cacheable Area

* Not all memory regions are cacheable.
* Regions like I/O-mapped memory may bypass cache to avoid inconsistencies.

#### Cache Hierarchy

* **Multiple levels of cache**:

  * L1: smallest and fastest, close to CPU.
  * L2: larger but slower.
  * L3 (if present): even larger, shared among cores.
* Hierarchy balances speed and storage capacity.

### Pipelining

* CPU executes instructions in **stages**, similar to an assembly line:

  1. Fetch
  2. Decode
  3. Execute
  4. Memory access
  5. Write back
* **Increases throughput** without increasing clock frequency.
* Hazards can occur:

  * Data hazards (dependencies between instructions)
  * Control hazards (branches and jumps)
  * Structural hazards (resource conflicts)
* Techniques like forwarding and branch prediction reduce hazards.

---

## Notes & Reflections

* Performance is not just about clock speed; memory latency and instruction execution order are equally critical.
* Caching and pipelining are complementary techniques that dramatically improve efficiency.
* Understanding these mechanisms is essential for optimizing software and designing hardware that meets real-world performance demands.
* For OS development, knowledge of cache behavior and pipelining helps write efficient low-level code.