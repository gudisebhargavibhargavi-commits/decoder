# Verilog Decoder

## Overview
This project implements a simple **2-to-4 Decoder** in Verilog HDL. A decoder converts binary input into one of several outputs.

## Truth Table

| A1 | A0 | Y3 | Y2 | Y1 | Y0 |
|----|----|----|----|----|----|
| 0  | 0  | 0  | 0  | 0  | 1  |
| 0  | 1  | 0  | 0  | 1  | 0  |
| 1  | 0  | 0  | 1  | 0  | 0  |
| 1  | 1  | 1  | 0  | 0  | 0  |

## Files

- `decoder.v` – Verilog source code
- `decoder_tb.v` – Testbench
- `simulation/` – Waveform and simulation files

## Tools Used

- Icarus Verilog
- GTKWave

## How to Run

Compile:

```bash
iverilog -o decoder decoder.v decoder_tb.v
```

Run:

```bash
vvp decoder
```

Open waveform:

```bash
gtkwave decoder.vcd
```

## Expected Output

The output line corresponding to the binary input becomes HIGH while all other outputs remain LOW.