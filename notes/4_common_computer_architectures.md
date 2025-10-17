# Chapter 4 – Common Computer Architectures

## Sections

1. CISC Architecture
2. RISC Architecture
3. Von Neumann Architecture
4. Harvard Architecture

---

## Summary

This chapter presents the most widely used computer architectures, focusing on their structural and conceptual differences. It discusses CISC and RISC instruction set philosophies and contrasts the Von Neumann and Harvard models of data and instruction handling. These distinctions form the foundation for understanding both historical and modern processor design.

---

## Key Concepts

### CISC Architecture

* **CISC (Complex Instruction Set Computer)** emphasizes a **large and versatile instruction set**.
* Each instruction can perform multiple low-level operations (e.g., memory access + computation).
* Features:

  * Many addressing modes.
  * Complex decoding logic.
  * Instructions of variable length and execution time.
* **Advantages**: compact code, easier assembly programming, backward compatibility.
* **Disadvantages**: slower execution pipeline, higher hardware complexity.
* **Examples**: Intel x86, VAX, IBM System/360.

---

### RISC Architecture

* **RISC (Reduced Instruction Set Computer)** simplifies the CPU by limiting instructions to a **small, fixed-size set**.
* Key characteristics:

  * Each instruction executes in one clock cycle (ideally).
  * Heavy reliance on **compiler optimization**.
  * **Load/Store** model – only specific instructions access memory.
* **Advantages**: higher speed, simpler hardware, efficient pipelining.
* **Disadvantages**: larger programs (more instructions).
* **Examples**: ARM, MIPS, SPARC, PowerPC.

---

### Von Neumann Architecture

* Classical model introduced by **John von Neumann (1945)**.
* **Single memory** stores both data and instructions.
* A shared **bus** transfers both, one at a time.
* Structure:

  * CPU ↔ Memory ↔ I/O.
* **Von Neumann bottleneck**: limited throughput because instructions and data share the same path.
* Foundation for most general-purpose computers.

---

### Harvard Architecture

* Separates **instruction memory** and **data memory**.
* Allows simultaneous access to both → improved performance.
* Often used in **microcontrollers**, **DSPs**, and embedded systems.
* Variants:

  * **Modified Harvard**: allows limited data/instruction sharing.
* **Advantages**: parallelism, higher throughput.
* **Disadvantages**: more complex memory management, less flexible programming.

---

## Notes & Reflections

* The CISC vs RISC debate represents a trade-off between **hardware complexity** and **software optimization**.
* Von Neumann and Harvard architectures show different philosophies of data flow and memory access.
* Most modern CPUs use **hybrid designs**, blending RISC-like cores with CISC instruction sets or modified Harvard memory layouts.
* Understanding these architectures is crucial for grasping processor design, compiler behavior, and system performance—topics that link directly to later study in operating systems and low-level programming.