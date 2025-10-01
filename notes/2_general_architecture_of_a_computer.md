# Chapter 2 – General Architecture of a Computer

## Sections

1. Basic Diagram and Execution
2. Detailed Computer Model
3. Memory and I/O Components
4. CPU and Bus
5. Taxonomies

---

## Summary

This chapter explains the overall organization of a computer system. It starts from a high-level block diagram, introduces a more detailed structural model, explores memory and input/output components, and examines the role of the CPU and communication buses. The chapter concludes with taxonomies that classify computer architectures according to their structural and functional characteristics.

---

## Key Concepts

### Basic Diagram and Execution

* A computer can be represented in terms of three main components: **CPU, memory, and input/output devices**.
* The CPU executes a repetitive cycle:

  1. **Fetch** instruction from memory.
  2. **Decode** instruction to identify the operation.
  3. **Execute** the operation using the ALU and registers.
* This “instruction cycle” is the heartbeat of a computer.

### Detailed Computer Model

* Adds refinement to the basic diagram by splitting components:

  * Control Unit (CU) and Arithmetic Logic Unit (ALU) inside the CPU.
  * Separate hierarchies of memory (registers, cache, RAM, secondary storage).
  * Communication lines via **bus structures**.
* Highlights interactions between software (instructions) and hardware (components).

### Memory and I/O Components

* **Memory hierarchy**: registers → cache → main memory → secondary storage.
* **Input/Output** devices: keyboards, displays, disks, networks.
* Role of **controllers** and **interfaces** that mediate between CPU and external devices.
* Importance of buffering and direct memory access (DMA) for efficiency.

### CPU and Bus

* CPU is divided into:

  * **Control unit** – orchestrates instruction flow.
  * **ALU** – executes arithmetic and logic.
  * **Registers** – small, fast storage close to execution.
* **Bus systems**:

  * Data bus → transfers data.
  * Address bus → specifies memory locations.
  * Control bus → manages timing and control signals.
* Explains bottlenecks (e.g., Von Neumann bottleneck where CPU and I/O share the same path).

### Taxonomies

* Different ways to classify computer architectures:

  * **Von Neumann vs. Harvard** architectures (shared vs. separate memory for instructions and data).
  * **CISC vs. RISC** processors (complex vs. reduced instruction sets).
  * **Flynn’s taxonomy**: SISD, SIMD, MISD, MIMD, based on instruction and data streams.
* Taxonomies help compare architectures and understand design trade-offs.

---

## Notes & Reflections

* The chapter bridges abstract concepts (like the instruction cycle) with physical organization (CPU, memory, buses).
* Understanding the memory hierarchy and I/O mechanisms is crucial for later topics such as performance and operating system interaction.
* Taxonomies provide a useful lens to evaluate both historical and modern computer designs.
* This foundation is essential for anyone aiming to design CPUs or study operating systems in depth.