# 🔒 FPGA Security on DE10-Nano

> A configurable system for experimenting with **trust**, **cryptography**, and **exploits** on FPGAs using the DE10-Nano development board.

## 🎯 Project Purpose

This repository contains multiple security-focused projects designed to explore various aspects of FPGA security. It leverages the **DE10-Nano** platform to experiment with **trust**, **cryptography**, and **exploitation** techniques. Each project investigates a specific security-related concept or vulnerability, enabling hands-on learning and testing. 
  
The system provides the necessary framework for building, testing, and experimenting with these concepts on an FPGA.

## 🧠 System Overview

## 🧠 System Overview

- **Platform:** DE10-Nano FPGA (Cyclone V SoC)
- **Communication:** HPS-FPGA interface, NFS and TFTP Servers over Ethernet  
- **Development Tools:** Quartus Prime, OpenSSL, Linux for HPS  
- **Userspace Languages:** C  
- **Kernel Drivers:** Custom drivers for hardware interaction and communication between HPS and FPGA  
- **IP Cores:** Includes custom FPGA IP cores developed in VHDL

## 📝 Projects

### True Random Number Generation (TRNG)

#### Overview

- [Full Writeup](docs/trng.md)  
- A system was implemented on the **DE10-Nano** to generate true random numbers on a 32-bit register, and potential exploits were explored. This 32-bit memory-mapped register was then exposed to the HPS for software interfacing.

#### Concepts Explored:
- AES-128-CBC Encryption/Decryption with OpenSSL
- NIST STS Tests
- Metastability Sampling vs Ring Oscillator TRNGs
- Von-Neumann Correction/Whitened LFSR Post-Mixing

## 💡 Acknowledgements

- Repository template provided by Trevor Vannoy of MSU Bozeman for the purposes of **EELE 467**.
- 
