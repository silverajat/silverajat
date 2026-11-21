# Rajat Gupta

Electrical Engineering @ NUS · Embedded, power & digital hardware · NUS Mars Rover

I'm a second-year Electrical Engineering student at NUS. I design my own boards, bring them up, and put real-time logic on FPGAs, and I document what broke along the way.

B.Eng. Electrical Engineering, National University of Singapore (expected 2029). Advanced Electronics · Minor in Data Science & Analytics · GPA 4.6/5.0.

## Currently building

| Project | What it is | Status |
|---|---|---|
| **Music-Sync LED Controller** | A 4-layer board I designed (Gowin GW2AR-18 FPGA + ESP32-C3) that lights my room in time with music. Verilog I2S mic input, 3-band filter bank and beat detector on the FPGA; phone and laptop control over Bluetooth. When the flash programmer failed, I wrote a JTAG loader so the ESP32 configures the FPGA at every boot | Working · moving the per-LED lighting engine onto the FPGA |
| **[Lift Tracker Wearable](https://github.com/silverajat/lift-tracker)** | Wrist motion-sensor pod and Android app that count gym reps in real time: 32 of 33 recorded sets exact, all within one rep, checked against a Python reference model in CI. Custom 4-layer pod board (nRF52840, BMI270) | In daily use with the prototype pod · custom board ordered |
| **Crypto Order-Flow Engine** | Verilog FPGA engine that turns live crypto market data into an order book and trading signals, with a RISC-V control CPU and a hardware risk gate. All 102,044 events of a 69-minute recorded stream matched a software reference exactly | RTL verified in simulation · [custom Zynq-7020 board](https://github.com/silverajat/ofe-trader-board) ordered |
| **[Protocol Emulator ASIC](https://github.com/silverajat/protocol-emulator)** | A small reprogrammable chip that speaks UART, SPI and I2C, for Jane Street's tapeout competition (Tiny Tapeout, IHP 130 nm). Prototyped on my own FPGA board against real sensor chips | In progress · due Jan 2027 |
| **NUS Mars Rover – Power Distribution Board** | Designed the rover's power distribution board (PDB v1) in KiCad: battery distribution, DC-DC converter rails, voltage and current sensing. Designed PDB v2 end to end: a 4-layer high-current board with precharge, brake chopper, eFuse protection and hardware e-stop logic | v1 designed · v2 going to fabrication |

## Earlier projects

- **CHOMS – Coral Health Monitoring System** (2023): Arduino monitor with pH, temperature and turbidity sensors. Gold Medal and Best Project, 1st of 77 teams at JISF.
- **Regenerative Braking System** (2026, NUS team project): regen braking concept for an electric bus, with a buck-boost charging stage and BMS logic.
- **Smart Solar Street Lamp** (2025, NUS team project): off-grid 24 V LiFePO4 + 200 W PV system with Arduino PWM dimming control.
- **Autonomous Obstacle-Course Robot** (2025, NUS team project): Arduino robot with H-bridge motor drive and ultrasonic sensing.

## Skills

- **Hardware:** KiCad (4-layer PCB design), power electronics, JLCPCB assembly, ESP32, nRF52, Arduino
- **Digital design:** Verilog, FPGA (Gowin, AMD Zynq), cocotb, RISC-V, Tiny Tapeout
- **Languages:** Python, C, Kotlin, R
- **Tools:** Git, Linux

## Contact

[rg192007@gmail.com](mailto:rg192007@gmail.com)
<!-- LinkedIn: add later -->
