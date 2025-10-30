# Chapter 5 – Basic Boolean Associations

## Sections

1. Boolean Algebra and Digital Technology
2. Gates

   * Drivers and Identity
   * Inverter and Negation
   * AND Gate and Conjunction
   * NAND
   * OR Gate and Disjunction
   * NOR
   * XOR and Antivalence
   * XNOR and Equivalence
3. Laws of Boolean Algebra

---

## Summary

This chapter introduces the logical foundations of digital systems through **Boolean algebra** and **logic gates**. It explains how binary logic operations form the basis of all digital circuits and computing devices. The chapter concludes with the fundamental laws of Boolean algebra used to simplify and design logical expressions and circuits.

---

## Key Concepts

### Boolean Algebra and Digital Technology

* Boolean algebra operates with **two values**: `0` (false) and `1` (true).
* Every digital circuit is a physical implementation of Boolean expressions.
* Basic operations:

  * **AND (·)** → logical multiplication.
  * **OR (+)** → logical addition.
  * **NOT (‾)** → logical inversion.
* Used for designing and optimizing **combinational and sequential circuits**.
* Digital technology translates Boolean logic into voltage levels (e.g., 0V = 0, +5V = 1).

---

### Gates

#### Drivers and Identity

* A **driver** reproduces an input signal at its output; it performs the **identity function**.
* Used for buffering or amplifying signals without logical modification.

#### Inverter and Negation

* Implements logical **NOT**: output is the opposite of input.
* Symbol: a triangle with a small circle at the output.
* Expression:

  ```
  Y = ¬A
  ```

  or equivalently `Y = A'`.

#### AND Gate and Conjunction

* Output is `1` **only if all inputs are 1**.
* Expression: `Y = A · B`.
* Corresponds to logical multiplication.

#### NAND

* Combination of AND followed by NOT:
  `Y = ¬(A · B)`.
* Universally functional: any Boolean function can be built from NAND gates alone.

#### OR Gate and Disjunction

* Output is `1` **if at least one input is 1**.
* Expression: `Y = A + B`.

#### NOR

* Combination of OR followed by NOT:
  `Y = ¬(A + B)`.
* Also functionally complete (can build any logic circuit using only NOR).

#### XOR and Antivalence

* **Exclusive OR**: output is `1` if inputs differ.
* Expression: `Y = A ⊕ B = (A · ¬B) + (¬A · B)`.
* Represents **inequality** between inputs.

#### XNOR and Equivalence

* **Exclusive NOR**: output is `1` if inputs are equal.
* Expression: `Y = ¬(A ⊕ B)`.
* Represents **equality** (logical equivalence).

---

### Laws of Boolean Algebra

* Core rules used to simplify logic expressions:

  * **Commutative**: `A + B = B + A`, `A · B = B · A`
  * **Associative**: `(A + B) + C = A + (B + C)`
  * **Distributive**: `A · (B + C) = (A · B) + (A · C)`
  * **Identity**: `A + 0 = A`, `A · 1 = A`
  * **Null/Zero**: `A + 1 = 1`, `A · 0 = 0`
  * **Idempotent**: `A + A = A`, `A · A = A`
  * **Complement**: `A + ¬A = 1`, `A · ¬A = 0`
  * **De Morgan’s Theorems**:

    * `¬(A · B) = ¬A + ¬B`
    * `¬(A + B) = ¬A · ¬B`
* These rules allow complex circuits to be simplified into minimal forms.

---

## Notes & Reflections

* Boolean algebra is the **mathematical backbone** of all digital hardware.
* Understanding how logical operations map to physical gates is crucial for circuit design and CPU architecture.
* NAND and NOR gates’ universality shows how simplicity can yield full computational power.