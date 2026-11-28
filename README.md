<img src="banner.png" alt="Copper layers of boards I designed: Mars Rover PDB v2, Zynq-7010 trading board, FPGA LED controller, nRF52 wrist pod" width="100%">

### I design FPGA logic and the boards it runs on

Second-year Electrical Engineering student at NUS. I write Verilog, verify it bit for bit against a software golden model, and design the boards it runs on. Everything in the banner above is a real copper layer from a board I laid out.

[**Portfolio**](https://silverajat.github.io) · [LinkedIn](https://www.linkedin.com/in/rajat-gupta-ee) · [Email](mailto:rg192007@gmail.com) · Looking for summer 2027 or May to December 2027 internships in FPGA, digital design and verification

---

<table>
<tr>
<td width="50%" valign="top">
<a href="https://github.com/silverajat/ofe-trader-board"><img src="card_zynq.png" alt="Zynq-7010 trading board copper layers"></a>

**Crypto order-flow engine + Zynq-7010 board**<br>
Verilog engine that rebuilds a live order book and computes trading signals in hardware, with a PicoRV32 control CPU and a hardware risk gate.

- **102,044 / 102,044** events of a 69-minute real market stream identical to the C++ reference
- Packet-to-features latency **p50 3.4 µs, p99 7.6 µs** after a tick-ladder book redesign
- Own **6-layer Zynq-7010 board** with DDR3L · RTL verified · boards arrived, bring-up next
</td>
<td width="50%" valign="top">
<img src="card_asic.png" alt="Protocol emulator ASIC concept: 8x4 Tiny Tapeout tiles">

**Protocol emulator ASIC**<br>
A small chip that runs wire protocols as programs, so the same silicon can speak UART, SPI, I2C or CAN. Entry for Jane Street's open ASIC competition (Tiny Tapeout, IHP 130 nm).

- Being prototyped on the FPGA of my own LED-controller board
- cocotb tests against a Python reference model
- In progress · repo goes public with the submission (Jan 2027)
</td>
</tr>
<tr>
<td width="50%" valign="top">
<a href="https://github.com/silverajat/ledctl"><img src="card_led.png" alt="FPGA LED controller board copper layers"></a>

**Music-sync LED controller**<br>
My own 4-layer board (Gowin GW2AR-18 FPGA + ESP32-C3) that lights a room in time with music.

- I2S mic input, 3-band filter bank and beat detector in Verilog
- Wrote a JTAG loader so the ESP32 configures the FPGA at boot when the flash programmer failed
- **Working** · moving the per-LED engine onto the FPGA
</td>
<td width="50%" valign="top">
<a href="https://github.com/silverajat/lift-tracker"><img src="card_pod.png" alt="nRF52840 wrist pod board copper layers"></a>

**Lift tracker wearable**<br>
Fitbit-sized wrist pod and Android app that count gym reps live, grade each rep's range of motion and end the set on their own.

- **32 of 33** recorded sets counted exactly on the prototype, all within one rep
- Kotlin pipeline checked against a Python reference model in CI
- My own 4-layer nRF52840 + LSM6DSV16X board, 0.55 mm thinner than a Fitbit Air · **built, in daily use**
</td>
</tr>
</table>

<a href="https://silverajat.github.io/#rover"><img src="card_pdb.png" alt="Mars Rover power distribution board v2" width="49%" align="right"></a>

**NUS Mars Rover · power distribution**<br>
Designed the rover's PDB v1, then PDB v2 end to end: a 4-layer high-current board with precharge, brake chopper, eFuse protection and hardware e-stop logic.

<br clear="right">

**The LED controller, for real:** the strip around my pinboard synced to a song: build-up, one dark beat, then the drop.

<a href="https://github.com/silverajat/ledctl"><img src="https://raw.githubusercontent.com/silverajat/ledctl/main/docs/images/demo_music.gif" alt="My LED controller lighting the strip around a pinboard in sync with a song: build-up, one dark beat, then the drop" width="640"></a>

### Toolbox

**Digital design:** Verilog · cocotb · Vivado · Gowin EDA · Verilator · RISC-V (PicoRV32) · Tiny Tapeout<br>
**Hardware:** KiCad (4- and 6-layer) · DDR3L layout · power electronics · JLCPCB assembly · ESP32 · nRF52<br>
**Software:** Python · C / C++ · Kotlin · Git · Linux

**Earlier:** CHOMS coral-health monitor, Gold Medal and Best Project (1st of 77 teams) at JISF 2023 · VANDA International Science Competition, Gold (11th globally)
