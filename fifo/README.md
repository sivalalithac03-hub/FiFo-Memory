# FIFO Memory Using Verilog

## Description

This project implements a simple FIFO (First-In First-Out) memory using Verilog HDL. Data is written into the memory in one order and read out in the same order.

## Objective

The objective is to design and simulate a basic FIFO memory using Verilog HDL and verify its read and write operations using a testbench.

## FIFO Specifications

* **Memory Depth:** 4 locations
* **Data Width:** 8 bits
* **Total Capacity:** 4 × 8 bits
* **Operation:** First-In First-Out

## Inputs

* `clk` – Clock signal
* `reset` – Reset signal
* `wr_en` – Write enable
* `rd_en` – Read enable
* `data_in[7:0]` – Input data

## Outputs

* `data_out[7:0]` – Output data
* `full` – Indicates FIFO is full
* `empty` – Indicates FIFO is empty

## Working

FIFO stands for **First-In First-Out**. The first data written into the FIFO is the first data that will be read.

Example:

```text
Write: 10 → 20 → 30

Read:
10 → 20 → 30
```

The FIFO uses a memory array, write pointer, read pointer, and counter to control the data flow.

## Project Files

* `README.md` – Project documentation
* `fifo_memory.v` – Verilog FIFO design
* `fifo_memory_tb.v` – Testbench
* `simulation_output.txt` – Simulation results

## Tools Used

* Verilog HDL
* Xilinx Vivado / ModelSim / Icarus Verilog
* GitHub

## Applications

* Data buffering
* Digital communication
* Processor data transfer
* UART systems
* Networking systems
* Embedded systems

## Conclusion

The FIFO memory was successfully designed and simulated using Verilog HDL. The simulation verifies that data is read in the same order in which it was written.
