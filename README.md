# Low-Complexity Approximate DFT for Digital Beamforming

### MATLAB Simulation and FPGA-Oriented Hardware Design

## 1. Project Overview

This project investigates low-complexity Approximate Discrete Fourier Transform (ADFT) algorithms and their applications in digital beamforming for wireless communication systems.

The Discrete Fourier Transform (DFT) is widely used in digital signal processing, including OFDM communications, spectral analysis, and antenna-array processing. Although the Fast Fourier Transform (FFT) significantly reduces computational complexity compared with direct DFT computation, its hardware implementation can still require substantial arithmetic and processing resources.

Approximate DFT algorithms offer an alternative approach by simplifying the mathematical operations required to compute Fourier-like transformations. These approximations may reduce the number of multiplications and additions, potentially improving hardware efficiency at the expense of numerical accuracy.

This project focuses on evaluating the trade-offs between computational complexity, numerical accuracy, beamforming performance, and hardware implementation cost.

The initial development will be carried out in MATLAB, followed by hardware-oriented analysis and a planned FPGA implementation using Verilog.

## 2. Project Objectives

The main objectives are:

1. **Conventional DFT/FFT Implementation**
   - Implement the Discrete Fourier Transform from its mathematical definition.
   - Validate the implementation against MATLAB's built-in FFT function.
   - Establish a reference for subsequent comparisons.

2. **Approximate DFT Implementation**
   - Study and reproduce a published low-complexity ADFT algorithm.
   - Implement the proposed mathematical transformation in MATLAB.
   - Evaluate approximation errors and arithmetic complexity.

3. **Digital Beamforming Simulation**
   - Model a uniform linear antenna array.
   - Implement conventional DFT-based and approximate DFT-based beamforming.
   - Analyze spatial beam patterns, beamforming gain, and sidelobe characteristics.
   - Investigate performance under noise and interference.

4. **Hardware-Oriented Analysis**
   - Investigate fixed-point representations of the approximate transform.
   - Evaluate quantization effects and numerical limitations.
   - Develop a Verilog-based ADFT architecture.
   - Compare FPGA resource utilization, timing, and latency against a conventional FFT implementation.

## 3. Research Questions

This project aims to investigate:

- How accurately can a low-complexity approximate DFT reproduce the outputs of a conventional DFT?
- What computational savings can be achieved through multiplierless transform architectures?
- How does approximation affect digital beamforming performance?
- How robust are approximate beamforming architectures to noise, interference, and antenna imperfections?
- What hardware resource savings can be achieved when implementing approximate transforms on an FPGA?

## 4. Methodology

The project is organized into five main stages.

| Stage | Description | Primary Tools |
|---|---|---|
| 1 | Conventional DFT/FFT modeling and validation | MATLAB |
| 2 | Published ADFT algorithm reproduction and evaluation | MATLAB |
| 3 | Digital beamforming simulations | MATLAB |
| 4 | Fixed-point modeling and hardware architecture design | MATLAB, Verilog |
| 5 | FPGA synthesis and hardware performance comparison | FPGA development tools |

## 5. Technologies

**Primary environment**
- MATLAB

**Planned hardware development**
- Verilog HDL
- FPGA synthesis tools

**Version control and documentation**
- Git
- GitHub
- Markdown

## 6. Expected Outcomes

The expected deliverables include:

- MATLAB implementations of conventional and approximate DFT algorithms.
- Numerical accuracy and arithmetic-complexity comparisons.
- Digital beamforming simulations and visualization of spatial beam patterns.
- A fixed-point implementation suitable for hardware-oriented evaluation.
- A synthesizable Verilog architecture with simulation and verification tests.
- FPGA synthesis reports comparing hardware resource utilization and timing.
- A technical report documenting the methodology, experimental results, and limitations.

## 7. Project Status

**Status: In progress — Research setup and initial MATLAB development.**

The FPGA implementation and experimental evaluations are planned future stages. No performance improvements are claimed until they have been independently evaluated.

## 8. References

The initial research reference is:

Suarez et al., *Multi-Beam RF Aperture Using Multiplierless FFT Approximation*, Electronics Letters, 2014.

[Available on arXiv](https://arxiv.org/abs/1501.01946)

Additional publications, algorithms, and technical references will be added as the project develops.

## 9. Research Motivation

This project is motivated by ongoing research into hardware-efficient Fourier transform approximations for wireless communication and sensing systems, including research presented by Prof. Arjuna Madanayake at Politecnico di Milano in October 2026.

The broader aim is to explore the relationship between mathematical algorithm design, wireless signal processing, and digital hardware architectures.
