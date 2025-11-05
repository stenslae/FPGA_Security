# FPGA Security

This repository holds a configurable system for the DE10-Nano to explore trust, cryptography, and hardware/IoT hacking on FPGAs.

# Projects

## True Random Number Generation (TRNG)

### Overview

- [Full Writeup](docs/trng.md)
- A system was implemented on a DE10-Nano to generate true random numbers on a 32 bit register, and potential exploits were explored. This 32 bit memory-mapped register was then exposed to the HPS for software interfacing.

### Concepts

>- AES-128-CBC Encryption/Decrypton with OpenSSL
>- NIST STS Tests and Fuzzing
>- Metastability Sampling vs Ring Oscillator TRNGs
>- Von-Neumann correction/Whitened LFSR post-mixing

# Acknowledgements

- Repository template provided by Trevor Vannoy of MSU Bozeman for the purposes of EELE 467.
