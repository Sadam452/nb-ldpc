# Non-Binary Low-Density Parity-Check

This repository contains an implementation of Non-Binary Low-Density Parity-Check (NB-LDPC) codes along with tools for encoding, decoding, and analyzing performance over an Additive White Gaussian Noise (AWGN) channel.

## Overview
Non-Binary LDPC codes are a class of linear block error-correcting codes used for forward error correction in various communication systems. Unlike traditional LDPC codes, NB-LDPC codes operate over finite fields, making them suitable for applications where non-binary symbols are more efficient or natural, such as in wireless communication systems.

This implementation includes:
- Encoding and decoding algorithms for NB-LDPC codes.
- Methods for simulating transmission over an AWGN channel and evaluating Bit Error Rate (BER) performance.
- Tools for generating random NB-LDPC parity-check matrices and Gaussian noise samples.

## Requirements
- Python 3.x
- NumPy
- pyfinite
- commPy
- tqdm (optional, for progress bars)
- matplotlib (optional, for visualization)

## How to Run
1. Clone or download this repository to your local machine.
3. Ensure that the `H.txt` file containing the parity-check matrix is available in the repository directory.
4. Run the desired Python scripts from the terminal or a Python environment.
5. Installation commands are written in python jupyter file. If you run it from the terminal, you may need to write installation commands separately(if any error occurs without installation).

### Encoding and Decoding
The whole script for encoding and decoding NB-LDPC codes is `nb-ldpc.py`. You can customize the parameters, such as the size of the LDPC code, number of iterations, and noise levels, within the script itself. Execute the script as follows:
```
python nb-ldpc.py
```

### BER Performance Analysis
This script simulates transmission over a range of Signal-to-Noise Ratio (SNR) values and plots the BER curve.`

### Parity-Check Matrix Analysis
The script analyzes the properties of the LDPC parity-check matrix, such as checking for unsatisfied checks or decoding failures.

## Acknowledgments
- This implementation is based on research and algorithms developed by various researchers in the field of digital communication.
- The `pyfinite` library is used for finite field arithmetic operations.
- The `commPy` library provides modulation and demodulation functionalities.

## License
This implementation is provided under the [MIT License](LICENSE).

For any questions or issues, please open an [issue](https://github.com/Sadam452/nb-ldpc/issues) on GitHub.