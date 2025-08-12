# Round Robin Arbiter – Verilog Implementation

**Overview**

This project implements a **Round Robin Arbiter** in **Verilog HDL** to provide fair and cyclic access control among multiple requesters. The arbiter ensures that each requester gets an equal opportunity to access a shared resource without any one requester monopolizing it, thereby avoiding **starvation**. The design follows a **rotating priority scheme**, where the grant signal shifts to the next requester after each successful allocation.

**Key Features**

* **Fairness**: Each requester gets an equal chance to access the resource.
* **No Starvation**: All requests are served in a cyclic sequence.
* **Scalable Design**: Number of requesters can be easily increased by modifying parameters.
* **Clock-Driven Operation**: Synchronous logic for predictable behavior.
* **Verilog Testbench**: Provided to verify correct operation under various request patterns.

**Visualization**

The arbiter cycles through requests in the following order:
`REQ0 → REQ1 → REQ2 → ... → REQn → back to REQ0`

Only one **grant** signal is active at a time, and after each grant, the **priority pointer** moves to the next requester in line.

**Project Features**

* **Verilog RTL Design** of the Round Robin Arbiter.
* **Testbench** for simulation and verification.
* Designed for use in **bus arbitration**, **multi-core processors**, and **SoC interconnects**.
* Simulated on **EDA Playground** using Verilog.

**How to Use the Project**

1. Go to **[EDA Playground](https://www.edaplayground.com/)**.
2. Select **Verilog** as the language.
3. Paste the **RTL code** and **testbench** into separate files.
4. Choose **Icarus Verilog** or another simulator.
5. Run the simulation and analyze the waveform output.

**Requirements**

* Basic understanding of Verilog HDL.
* Knowledge of bus arbitration and digital logic design.
* EDA Playground (or any Verilog simulation tool).

**Objective**

The objective of this project is to design a **fair, efficient, and scalable Round Robin Arbiter** using Verilog HDL that can be applied in real-world digital systems requiring shared resource allocation among multiple requesters.


