# Rowhammer_Capstone
Simulate Rowhammer attacks at the physical level and redesign DRAM architecture to eliminate the vulnerability, exploring prevention and scalable real-world applications.


Main Goals of the Capstone Project
1. Simulate a Rowhammer Attack at the Physical Level

  Develop a technically grounded simulation that models the physical behavior of DRAM, including charge storage, leakage, and inter‑row coupling, in order to demonstrate how repeated activation of aggressor rows can induce bit flips in adjacent victim rows. The simulation will reproduce Rowhammer as a hardware‑originating fault mechanism, independent of software vulnerabilities, and will serve as a baseline for evaluating defensive designs.

2. Eliminate the Physical Vulnerabilities Through Architectural Redesign

  Design and evaluate modified DRAM architectures that remove the underlying physical mechanisms enabling Rowhammer, such as uncontrolled capacitive coupling and charge disturbance between adjacent rows. The objective is to demonstrate, within the simulation, that no legal memory access pattern can induce bit flips, thereby achieving prevention by construction rather than probabilistic mitigation.

3. Theorize a Scalable Real‑World Application

  Extend the redesigned, Rowhammer‑resistant architecture into a real‑world deployment context, analyzing how such a design could be implemented at scale in modern memory systems. This includes theorizing its applicability to data centers, high‑assurance systems, and safety‑critical hardware, while assessing trade‑offs in performance, power consumption, cost, and manufacturability.
