# LTspice – CMOS Circuits and MOSFET Characterization

This repository contains my LTspice circuit designs and simulation results, covering transistor-level CMOS logic, combinational and sequential digital circuits, and MOSFET characteristics. The designs include schematics, symbols, test benches, and output waveforms where available.

## 1. CMOS Logic Gates

The gates in [`digilib/`](https://github.com/devaprassads/LTSpice/blob/main/digilib/) are built using CMOS transistor networks.

| Circuit | Schematic | Test bench / output |
|---|---|---|
| Inverter | [inv1x.asc](https://github.com/devaprassads/LTSpice/blob/main/digilib/inverter/schematic/inv1x.asc) · [Schematic image](https://github.com/devaprassads/LTSpice/blob/main/digilib/inverter/schematic/inverter_schematic.png) | [Test bench](https://github.com/devaprassads/LTSpice/blob/main/digilib/inverter/test%20bench/inv1x_tb_tran.asc) · [Waveform](https://github.com/devaprassads/LTSpice/blob/main/digilib/inverter/output/waveform.png) |
| NAND | [nand1x.asc](https://github.com/devaprassads/LTSpice/blob/main/digilib/nand/schematic/nand1x.asc) · [Schematic image](https://github.com/devaprassads/LTSpice/blob/main/digilib/nand/schematic/nand_schematic.png) | [Test bench](https://github.com/devaprassads/LTSpice/blob/main/digilib/nand/test%20bench/nand1x_tb_tran.asc) · [Waveform](https://github.com/devaprassads/LTSpice/blob/main/digilib/nand/test%20bench/nand_waveform.png) |
| NOR | [nor1x.asc](https://github.com/devaprassads/LTSpice/blob/main/digilib/nor/schematic/nor1x.asc) · [Schematic image](https://github.com/devaprassads/LTSpice/blob/main/digilib/nor/schematic/nor_schematic.png) | [Test bench](https://github.com/devaprassads/LTSpice/blob/main/digilib/nor/test%20bench/nor1x_tb_tran.asc) · [Output](https://github.com/devaprassads/LTSpice/blob/main/digilib/nor/test%20bench/nor_op.png) |
| AND | [and1x.asc](https://github.com/devaprassads/LTSpice/blob/main/digilib/and/schematic/and1x.asc) · [Schematic image](https://github.com/devaprassads/LTSpice/blob/main/digilib/and/schematic/and_schematic.png) | [Test bench](https://github.com/devaprassads/LTSpice/blob/main/digilib/and/test%20bench/and_tb_tran.asc) · [Waveform](https://github.com/devaprassads/LTSpice/blob/main/digilib/and/output/and_waveform.png) |
| OR | [or1x.asc](https://github.com/devaprassads/LTSpice/blob/main/digilib/or/schematic/or1x.asc) · [Schematic image](https://github.com/devaprassads/LTSpice/blob/main/digilib/or/schematic/Or_schematic.png) | [Test bench](https://github.com/devaprassads/LTSpice/blob/main/digilib/or/test%20bench/or1x_tb_tran.asc) · [Waveform](https://github.com/devaprassads/LTSpice/blob/main/digilib/or/test%20bench/or_waveform.png) |
| XOR | [xor1x.asc](https://github.com/devaprassads/LTSpice/blob/main/digilib/xor/schematic/xor1x.asc) · [Schematic image](https://github.com/devaprassads/LTSpice/blob/main/digilib/xor/schematic/xor_schematic.png) | [Test bench](https://github.com/devaprassads/LTSpice/blob/main/digilib/xor/test%20bench/xor1x_tb_tran.asc) · [Waveform](https://github.com/devaprassads/LTSpice/blob/main/digilib/xor/test%20bench/xor_waveform.png) |
| XNOR | [xnor1x.asc](https://github.com/devaprassads/LTSpice/blob/main/digilib/xnor/schematic/xnor1x.asc) · [Schematic image](https://github.com/devaprassads/LTSpice/blob/main/digilib/xnor/schematic/xnor_schematic.png) | [Test bench](https://github.com/devaprassads/LTSpice/blob/main/digilib/xnor/test%20bench/xnor1x_tb_tran.asc) · [Waveform](https://github.com/devaprassads/LTSpice/blob/main/digilib/xnor/test%20bench/xnor_waveform.png) |
| 3-input NAND | [nand3.asc](https://github.com/devaprassads/LTSpice/blob/main/nand_3/nand3.asc) · [Schematic image](https://github.com/devaprassads/LTSpice/blob/main/nand_3/nand3_schematic.png) | [Test bench](https://github.com/devaprassads/LTSpice/blob/main/nand_3/nand3_tb_tran.asc) · [Output waveform](https://github.com/devaprassads/LTSpice/blob/main/nand_3/nand3_op.png) |

The gate library also contains reusable LTspice symbols (`.asy`) and additional test-bench images.

## 2. Combinational Circuits

### Full Adder
A one-bit full adder produces a sum and carry output from inputs A, B, and carry-in.

- [Full-adder schematic](https://github.com/devaprassads/LTSpice/blob/main/FullAdder/full_adder.asc)
- [symbol](https://github.com/devaprassads/LTSpice/blob/main/FullAdder/full_adder.asy)
- [Test bench](https://github.com/devaprassads/LTSpice/blob/main/FullAdder/full_adder_tb.asc)
- [Schematic image](https://github.com/devaprassads/LTSpice/blob/main/FullAdder/fulladder_schematic.png)
- [Simulation output](https://github.com/devaprassads/LTSpice/blob/main/FullAdder/fulladder_op.png)
- [Test-bench image](https://github.com/devaprassads/LTSpice/blob/main/FullAdder/fulladder_tb.png)

### 2-to-1 Multiplexer
The select input chooses which data input is passed to the output.

- [Multiplexer schematic](https://github.com/devaprassads/LTSpice/blob/main/mux/mux21.asc)
- [symbol](https://github.com/devaprassads/LTSpice/blob/main/mux/mux21.asy)
- [Test bench](https://github.com/devaprassads/LTSpice/blob/main/mux/mux21_tb_tran.asc)
- [Schematic image](https://github.com/devaprassads/LTSpice/blob/main/mux/mux21_schematic.png)
- [Simulation output](https://github.com/devaprassads/LTSpice/blob/main/mux/mux21_op.png)
- [Test-bench image](https://github.com/devaprassads/LTSpice/blob/main/mux/mux21_tb.png)

### 2-to-4 Decoder
The two input bits select one of four output lines.

- [Decoder schematic](https://github.com/devaprassads/LTSpice/blob/main/decoder/decoder24.asc)
- [symbol](https://github.com/devaprassads/LTSpice/blob/main/decoder/decoder24.asy)
- [Test bench](https://github.com/devaprassads/LTSpice/blob/main/decoder/decoder24_tb_tran.asc)
- [Schematic image](https://github.com/devaprassads/LTSpice/blob/main/decoder/decoder24_schematic.png)
- [Simulation output](https://github.com/devaprassads/LTSpice/blob/main/decoder/decoder24_op.png)
- [Test-bench image](https://github.com/devaprassads/LTSpice/blob/main/decoder/decoder24_tb.png)

## 3. Sequential Circuits

### Latch
- [SR latch schematic](https://github.com/devaprassads/LTSpice/blob/main/latch/srlatch.asc)
- [symbol](https://github.com/devaprassads/LTSpice/blob/main/latch/srlatch.asy)
- [Test bench](https://github.com/devaprassads/LTSpice/blob/main/latch/srlatch_tb_tran.asc)
- [Schematic image](https://github.com/devaprassads/LTSpice/blob/main/latch/srlatch_schematic.png)
- [Output waveform](https://github.com/devaprassads/LTSpice/blob/main/latch/srlatch_op.png)

### Flip-Flops
The folder contains D, JK, SR, and T flip-flop designs.

| Flip-flop | Schematic | Test bench | Output |
|---|---|---|---|
| D | [D_flipflop.asc](https://github.com/devaprassads/LTSpice/blob/main/flipflops/d_flipflop/D_flipflop.asc) | [Test bench](https://github.com/devaprassads/LTSpice/blob/main/flipflops/d_flipflop/D_flipflop_tb_tran.asc) | [Waveform](https://github.com/devaprassads/LTSpice/blob/main/flipflops/d_flipflop/dff_op.png) |
| JK | [jk_flipflop.asc](https://github.com/devaprassads/LTSpice/blob/main/flipflops/jk_flipflop/jk_flipflop.asc) | [Test bench](https://github.com/devaprassads/LTSpice/blob/main/flipflops/jk_flipflop/jk_flipflop_tb_tran.asc) | [Waveform](https://github.com/devaprassads/LTSpice/blob/main/flipflops/jk_flipflop/jk_op.png) |
| SR | [sr_flipflop.asc](https://github.com/devaprassads/LTSpice/blob/main/flipflops/sr_flipflop/sr_flipflop.asc) | [Test bench](https://github.com/devaprassads/LTSpice/blob/main/flipflops/sr_flipflop/sr_flipflop_tb.asc) | [Waveform](https://github.com/devaprassads/LTSpice/blob/main/flipflops/sr_flipflop/srff_op.png) |
| T | [T_flipflop.asc](https://github.com/devaprassads/LTSpice/blob/main/flipflops/t_flipflop/T_flipflop.asc) | [Test bench](https://github.com/devaprassads/LTSpice/blob/main/flipflops/t_flipflop/T_flipflop_tb_tran.asc) | [Waveform](https://github.com/devaprassads/LTSpice/blob/main/flipflops/t_flipflop/tff_op.png) |

D flip-flop with preset/clear 

- [D flip-flop with preset/clear schematic](https://github.com/devaprassads/LTSpice/blob/main/dff%20with%20pc/Dff_with_pc.asc)
- [Test bench](https://github.com/devaprassads/LTSpice/blob/main/dff%20with%20pc/dff_with_pc_tb.asc)
- [Schematic image](https://github.com/devaprassads/LTSpice/blob/main/dff%20with%20pc/dff_pc_schematic.png)
- [Simulation output](https://github.com/devaprassads/LTSpice/blob/main/dff%20with%20pc/dff_pc_op.png)

### Up and Down Counters
Positive-edge and negative-edge versions of up,down counters

| Circuit | Schematic | Test bench | Output |
|---|---|---|---|
| Up counter, positive edge | [up_counter.asc](https://github.com/devaprassads/LTSpice/blob/main/up%20counter/pos%20edge/up_counter.asc) | [Test bench](https://github.com/devaprassads/LTSpice/blob/main/up%20counter/pos%20edge/up_counter_tb.asc) | [Waveform](https://github.com/devaprassads/LTSpice/blob/main/up%20counter/pos%20edge/up_tb.png) |
| Up counter, negative edge | [up_counter_neg.asc](https://github.com/devaprassads/LTSpice/blob/main/up%20counter/neg%20edge/up_counter_neg.asc) | [Test bench](https://github.com/devaprassads/LTSpice/blob/main/up%20counter/neg%20edge/up_counter_neg_tb.asc) | [Waveform](https://github.com/devaprassads/LTSpice/blob/main/up%20counter/neg%20edge/up_neg_tb.png) |
| Down counter, positive edge | [down_counter.asc](https://github.com/devaprassads/LTSpice/blob/main/down%20counter/pos%20edge/down_counter.asc) | [Test bench](https://github.com/devaprassads/LTSpice/blob/main/down%20counter/pos%20edge/down_counter_tb.asc) | [Waveform](https://github.com/devaprassads/LTSpice/blob/main/down%20counter/pos%20edge/down_tb.png) |
| Down counter, negative edge | [down_counter_neg.asc](https://github.com/devaprassads/LTSpice/blob/main/down%20counter/neg%20edge/down_counter_neg.asc) | [Test bench](https://github.com/devaprassads/LTSpice/blob/main/down%20counter/neg%20edge/down_counter_tb_neg.asc) | [Waveform](https://github.com/devaprassads/LTSpice/blob/main/down%20counter/neg%20edge/down_neg_tb.png) |

### Shift Registers
The folder contains serial and parallel shift-register designs.

- **Serial:** [Schematic](https://github.com/devaprassads/LTSpice/blob/main/shift%20register/series/shift_reg.asc) · [Symbol](https://github.com/devaprassads/LTSpice/blob/main/shift%20register/series/shift_reg.asy) · [Test bench](https://github.com/devaprassads/LTSpice/blob/main/shift%20register/series/shift_reg_tb.asc) · [Output](https://github.com/devaprassads/LTSpice/blob/main/shift%20register/series/series_op.png)
- **Parallel:** [Schematic](https://github.com/devaprassads/LTSpice/blob/main/shift%20register/parallel/parallel_shift_reg.asc) · [Symbol](https://github.com/devaprassads/LTSpice/blob/main/shift%20register/parallel/parallel_shift_reg.asy) · [Test bench](https://github.com/devaprassads/LTSpice/blob/main/shift%20register/parallel/parallel_shift_reg_tb.asc) · [Shift output](https://github.com/devaprassads/LTSpice/blob/main/shift%20register/parallel/parallel_shift_op.png) · [Parallel-load output](https://github.com/devaprassads/LTSpice/blob/main/shift%20register/parallel/parallel_load_op.png)

## 4. MOSFET Characterization

The [`mos chara/`](https://github.com/devaprassads/LTSpice/blob/main/mos%20chara/) folder contains LTspice studies of MOSFET behaviour and device-related parameters.

| Study | Schematic / file | Result |
|---|---|---|
| Drain current vs. drain-source voltage (\(I_D\)–\(V_DS\)) | [VdsvsId.asc](https://github.com/devaprassads/LTSpice/blob/main/mos%20chara/Id_vs_Vds/VdsvsId.asc) | [Plot](https://github.com/devaprassads/LTSpice/blob/main/mos%20chara/Id_vs_Vds/VdsvsId.png) |
| Drain current vs. gate-source voltage (\(I_D\)–\(V_GS\)) | [IdvsVgs.asc](https://github.com/devaprassads/LTSpice/blob/main/mos%20chara/Id_vs_Vgs/IdvsVgs.asc) | [Plot](https://github.com/devaprassads/LTSpice/blob/main/mos%20chara/Id_vs_Vgs/IdvsVgs.png) |
| Transconductance (\(g_m\)) | [gm.asc](https://github.com/devaprassads/LTSpice/blob/main/mos%20chara/gm/gm.asc) | [Result](https://github.com/devaprassads/LTSpice/blob/main/mos%20chara/gm/gm_op.png) |
| Threshold voltage (\(V_th\)) | [vth.asc](https://github.com/devaprassads/LTSpice/blob/main/mos%20chara/vth/vth.asc) | [Result](https://github.com/devaprassads/LTSpice/blob/main/mos%20chara/vth/vth_op.png) |
| Gate capacitance (\(C_gg\)) | [Cgg.asc](https://github.com/devaprassads/LTSpice/blob/main/mos%20chara/cgg/Cgg.asc) | [Result](https://github.com/devaprassads/LTSpice/blob/main/mos%20chara/cgg/cgg_op.png) |
| Drain capacitance (\(C_dd\)) | [Cdd.asc](https://github.com/devaprassads/LTSpice/blob/main/mos%20chara/cdd/Cdd.asc) | [Result](https://github.com/devaprassads/LTSpice/blob/main/mos%20chara/cdd/cdd_op.png) |
| Delay | [time.asc](https://github.com/devaprassads/LTSpice/blob/main/mos%20chara/delay/time.asc) | [Result](https://github.com/devaprassads/LTSpice/blob/main/mos%20chara/delay/time_op.png) |
| Parameter \(k\) | [k.asc](https://github.com/devaprassads/LTSpice/blob/main/mos%20chara/k/k.asc) | [Result](https://github.com/devaprassads/LTSpice/blob/main/mos%20chara/k/k_op.png) |
| Power | [power.asc](https://github.com/devaprassads/LTSpice/blob/main/mos%20chara/power/power.asc) | [Result](https://github.com/devaprassads/LTSpice/blob/main/mos%20chara/power/power_op.png) |
| On-resistance, triode region | [ron_triode.asc](https://github.com/devaprassads/LTSpice/blob/main/mos%20chara/ron/triode/ron_triode.asc) | [Result](https://github.com/devaprassads/LTSpice/blob/main/mos%20chara/ron/triode/ron_triode_op.png) |
| On-resistance, saturation region | [ron_saturated.asc](https://github.com/devaprassads/LTSpice/blob/main/mos%20chara/ron/saturated/ron_saturated.asc) | [Result](https://github.com/devaprassads/LTSpice/blob/main/mos%20chara/ron/saturated/ron_sat_op.png) |
| NMOS characteristics | [nmos_char.asc](https://github.com/devaprassads/LTSpice/blob/main/mos%20chara/nmos/nmos_char.asc) | [Result](https://github.com/devaprassads/LTSpice/blob/main/mos%20chara/nmos/nmos_chara.png) |

## 5. CMOS Technology Model

The designs use a **180 nm CMOS BSIM3 v3.1 model**.

- [BSIM3 180 nm model file](https://github.com/devaprassads/LTSpice/blob/main/model/bsim3_180nm.cir)
- NMOS model name: `CMOSN`
- PMOS model name: `CMOSP`
- Logic-gate supply voltage: **3.3 V**

## Tools

- **Circuit design and simulation:** LTspice
- **Device model:** BSIM3 v3.1
- **Technology node:** 180 nm CMOS

## Author

**Deva Prassad S**  
[GitHub Profile](https://github.com/devaprassads)
