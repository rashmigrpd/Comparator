# 2-Bit Comparator using Verilog

## Project Description

A **2-Bit Comparator** is a combinational logic circuit used to compare two 2-bit binary numbers. It determines whether the first input (A) is **greater than**, **equal to**, or **less than** the second input (B). The circuit produces three outputs:

- **A_gt_B** – HIGH when A > B
- **A_eq_B** – HIGH when A = B
- **A_lt_B** – HIGH when A < B

This project implements a 2-Bit Comparator using Verilog HDL and verifies its functionality through a comprehensive testbench.

---

## Inputs

- A[1:0] – First 2-bit input
- B[1:0] – Second 2-bit input

## Outputs

- A_gt_B
- A_eq_B
- A_lt_B

---

## Truth Table

| A | B | A>B | A=B | A<B |
|---|---|-----|-----|-----|
|00|00|0|1|0|
|00|01|0|0|1|
|01|00|1|0|0|
|01|01|0|1|0|
|10|01|1|0|0|
|10|10|0|1|0|
|11|10|1|0|0|
|11|11|0|1|0|

---

## Files

- `comparator2bit.v` – Verilog design
- `comparator2bit_tb.v` – Testbench
- `output.txt` – Expected simulation output
- `README.md` – Project documentation

---

## Software Used

- Icarus Verilog
- ModelSim
- Xilinx Vivado

---

## How to Run

Compile:

```bash
iverilog comparator2bit.v comparator2bit_tb.v
```

Run:

```bash
vvp a.out
```

---

## Expected Output

```
A  B | A>B A=B A<B
00 00 | 0   1   0
00 01 | 0   0   1
01 00 | 1   0   0
01 01 | 0   1   0
10 01 | 1   0   0
10 10 | 0   1   0
11 10 | 1   0   0
11 11 | 0   1   0
```

---

## Applications

- Arithmetic Logic Units (ALUs)
- Digital Decision-Making Circuits
- Microprocessors
- Control Systems
- Data Comparison Circuits

---

## Author

Your Name