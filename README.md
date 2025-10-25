# 3X8_DECODER_VHDL

## Overview
<br>

-A 3x8 Decoder implemented in VHDL and simulated using ModelSim.

-A Decoder is a combinational circuit that converts binary information from ‘n’ input lines to a maximum of 2ⁿ unique output lines.

-In this 3x8 Decoder, there are 3 input lines and 8 output lines.

-Only one output line is activated (logic '1') for each combination of input values.

## Truth Table
| **D2** | **D1** | **D0** | **Y0** | **Y1** | **Y2** | **Y3** | **Y4** | **Y5** | **Y6** | **Y7** |
| :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: |
|    0   |    0   |    0   |    1   |    0   |    0   |    0   |    0   |    0   |    0   |    0   |
|    0   |    0   |    1   |    0   |    1   |    0   |    0   |    0   |    0   |    0   |    0   |
|    0   |    1   |    0   |    0   |    0   |    1   |    0   |    0   |    0   |    0   |    0   |
|    0   |    1   |    1   |    0   |    0   |    0   |    1   |    0   |    0   |    0   |    0   |
|    1   |    0   |    0   |    0   |    0   |    0   |    0   |    1   |    0   |    0   |    0   |
|    1   |    0   |    1   |    0   |    0   |    0   |    0   |    0   |    1   |    0   |    0   |
|    1   |    1   |    0   |    0   |    0   |    0   |    0   |    0   |    0   |    1   |    0   |
|    1   |    1   |    1   |    0   |    0   |    0   |    0   |    0   |    0   |    0   |    1   |


## Logic Equation
<br>

Each output line can be expressed as a minterm of the inputs:
Y0 = D2'·D1'·D0'
Y1 = D2'·D1'·D0
Y2 = D2'·D1·D0'
Y3 = D2'·D1·D0
Y4 = D2·D1'·D0'
Y5 = D2·D1'·D0
Y6 = D2·D1·D0'
Y7 = D2·D1·D0

## Simulation Details

**Simulation Type:** Behavioral Simulation

**Tool Used:** ModelSim

**Language Used:** VHDL

**Inputs:** 3-bit binary vector (D2, D1, D0)

**Outputs:** 8-bit binary vector (Y7–Y0)
