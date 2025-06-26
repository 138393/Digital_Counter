# Digital_Counter
# Digital Counter – Custom Processor in Logisim

This project implements a **2-digit digital counter** using a custom-designed **microprocessor** in **Logisim**, complete with integrated **main memory** and **I/O device support**.

---
## Features

- Counts up or down between 00 and 99
- **Resets** automatically when reaching 0 or 99 based on the system mode 
- **Mode switch**: Supports both incrementing and decrementing modes using a switch
- Displays output through **LEDs** connected to I/O ports
- Fully implemented using **Logisim circuits** and **custom assembly instructions**

---

## Architecture

- **Datapath and Control Unit** designed from scratch
- **Main Memory** stores instructions and counter logic
- **I/O Module** handles LED output
- **ROM-based FSM** used for control logic
- **16-bit Instruction Register (IR)** for operation decoding

---

## Development Details

- Built in **Logisim Evolution**
- Assembly instructions written in ARM-like syntax and tested for a custom microprocessor
- The system uses **memory-mapped I/O**, where devices like switches and LED displays are accessed via specific memory addresses:
  - `0x80000200` for switch input
  - `0x80000300` and `0x80000301` for hex display control and data
- I/O is controlled using standard memory instructions (`LDR`, `STR`), allowing seamless integration of hardware and software
- Processor supports basic conditional logic and counter manipulation

---


