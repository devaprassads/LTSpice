# LTSpice

A library of CMOS logic gates built in LTspice using a 180 nm BSIM3 model, each with its schematic, symbol, test bench and simulation output.

## Contents

- [`digilib/`](digilib) — logic gate library
  - [`inverter/`](digilib/inverter)
  - [`and/`](digilib/and)
  - [`nand/`](digilib/nand)
  - [`nor/`](digilib/nor)
  - [`or/`](digilib/or)
  - [`xor/`](digilib/xor)
  - [`xnor/`](digilib/xnor)
- [`model/`](model) — device model
  - [`bsim3_180nm.cir`](model/bsim3_180nm.cir)

### `model/`

[`bsim3_180nm.cir`](model/bsim3_180nm.cir) has the BSIM3 v3.1 (Level 8) models `CMOSN` (NMOS) and `CMOSP` (PMOS) for a 180 nm process.

### `digilib/`

| Gate | Folder | Symbol | Built from |
| ---- | ------ | ------ | ---------- |
| Inverter | [`inverter`](digilib/inverter) | [`inv1x`](digilib/inverter/symbol/inv1x.asy) | 1 PMOS + 1 NMOS |
| NAND | [`nand`](digilib/nand) | [`nand1x`](digilib/nand/symbol/nand1x.asy) | 2 PMOS + 2 NMOS |
| NOR | [`nor`](digilib/nor) | [`nor1x`](digilib/nor/symbol/nor1x.asy) | 2 PMOS + 2 NMOS |
| AND | [`and`](digilib/and) | [`and1x`](digilib/and/symbol/and1x.asy) | NAND stage + `inv1x` |
| OR | [`or`](digilib/or) | [`or1x`](digilib/or/symbol/or1x.asy) | NOR stage + `inv1x` |
| XOR | [`xor`](digilib/xor) | [`xor1x`](digilib/xor/symbol/xor1x.asy) | 6 PMOS + 6 NMOS + `inv1x` |
| XNOR | [`xnor`](digilib/xnor) | [`xnor1x`](digilib/xnor/symbol/xnor1x.asy) | 6 PMOS + 6 NMOS |

Each gate folder contains the schematic,symbol,testbench and output waveforms of the gates. 

### Schematics, test benches and waveforms

| Gate | Schematic | Test bench | Waveform |
| ---- | --------- | ---------- | -------- |
| Inverter | [`inv1x.asc`](digilib/inverter/schematic/inv1x.asc) | [`inv1x_tb_tran.asc`](digilib/inverter/test%20bench/inv1x_tb_tran.asc) | [`waveform.png`](digilib/inverter/output/waveform.png) |
| NAND | [`nand1x.asc`](digilib/nand/schematic/nand1x.asc) | [`nand1x_tb_tran.asc`](digilib/nand/test%20bench/nand1x_tb_tran.asc) | [`nand_waveform.png`](digilib/nand/test%20bench/nand_waveform.png) |
| NOR | [`nor1x.asc`](digilib/nor/schematic/nor1x.asc) | [`nor1x_tb_tran.asc`](digilib/nor/test%20bench/nor1x_tb_tran.asc) | [`nor_op.png`](digilib/nor/test%20bench/nor_op.png) |
| AND | [`and1x.asc`](digilib/and/schematic/and1x.asc) | [`and_tb_tran.asc`](digilib/and/test%20bench/and_tb_tran.asc) | [`and_waveform.png`](digilib/and/output/and_waveform.png) |
| OR | [`or1x.asc`](digilib/or/schematic/or1x.asc) | [`or1x_tb_tran.asc`](digilib/or/test%20bench/or1x_tb_tran.asc) | [`or_waveform.png`](digilib/or/test%20bench/or_waveform.png) |
| XOR | [`xor1x.asc`](digilib/xor/schematic/xor1x.asc) | [`xor1x_tb_tran.asc`](digilib/xor/test%20bench/xor1x_tb_tran.asc) | [`xor_waveform.png`](digilib/xor/test%20bench/xor_waveform.png) |
| XNOR | [`xnor1x.asc`](digilib/xnor/schematic/xnor1x.asc) | [`xnor1x_tb_tran.asc`](digilib/xnor/test%20bench/xnor1x_tb_tran.asc) | [`xnor_waveform.png`](digilib/xnor/test%20bench/xnor_waveform.png) |

## Design Parameters

- Technology: 180 nm (`ln = 180nm`)
- Supply: `VDD = 3.3 V`
- Pull-up/pull-down sizing: `wp = wn * br`, with `br = 2.23612`
- Transistors are parameterised with `l`, `w`, `ad`, `as`, `pd`, `ps` derived from `ln/lp/wn/wp`
- Test benches: pulse inputs `a`, `b` (0 to 3.3 V) with `.tran` analysis

## Author

Deva Prassad S — [@devaprassads](https://github.com/devaprassads)
