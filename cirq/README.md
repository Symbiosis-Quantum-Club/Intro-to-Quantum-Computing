# Google Cirq 1.4+ Track

This track covers quantum computing using Google Quantum AI's Cirq framework (versions 1.4+), focusing on time-sliced moment architectures, 2D grid topologies, noise channels, and hardware constraints.

---

## Syllabus Overview

| Notebook | Topic | Python Concept | Quantum Concept |
|---|---|---|---|
| [`01_Python_and_Cirq_Architecture.ipynb`](./01_Python_and_Cirq_Architecture.ipynb) | Architecture and Qubit Models | Classes and instances | LineQubit, GridQubit, NamedQubit |
| [`02_Qubits_Moments_and_Circuits.ipynb`](./02_Qubits_Moments_and_Circuits.ipynb) | Moments and Circuits | Iterables and formatting | Moments (time-slices), circuit assembly |
| [`03_Single_Qubit_Gates_and_Operations.ipynb`](./03_Single_Qubit_Gates_and_Operations.ipynb) | Single Qubit Operations | Exponentiation overloading | Fractional powers, phased operators |
| [`04_Multi_Qubit_Gates_and_Entanglement.ipynb`](./04_Multi_Qubit_Gates_and_Entanglement.ipynb) | Multi-Qubit Entanglement | Coordinate systems and pairs | CNOT, CZ, SWAP, ISWAP, Bell states |
| [`05_Simulating_Circuits_and_Sampling.ipynb`](./05_Simulating_Circuits_and_Sampling.ipynb) | Simulation vs Sampling | Return structures and dataframes | `simulate()` versus `run()` |
| [`06_Parameterized_Circuits_and_Sweeps.ipynb`](./06_Parameterized_Circuits_and_Sweeps.ipynb) | Parameter Sweeps with SymPy | Symbolic variables (`Symbol`) | Parameterized circuits, `cirq.Sweep` |
| [`07_Quantum_Teleportation_in_Cirq.ipynb`](./07_Quantum_Teleportation_in_Cirq.ipynb) | Quantum Teleportation | Control flow and assertions | Teleportation protocol and fidelity |
| [`08_Grovers_Algorithm_in_Cirq.ipynb`](./08_Grovers_Algorithm_in_Cirq.ipynb) | Grover's Search in Cirq | Modular function decomposition | Oracle sub-circuits, diffusion moments |
| [`09_Quantum_Fourier_Transform.ipynb`](./09_Quantum_Fourier_Transform.ipynb) | Quantum Fourier Transform | Nested loops and exponent math | QFT implementation, circuit inversion |
| [`10_Simulating_Noisy_Quantum_Channels.ipynb`](./10_Simulating_Noisy_Quantum_Channels.ipynb) | Noisy Quantum Channels | Probability models and channels | Bit-flip, phase-flip, depolarizing noise |
| [`11_Quantum_Error_Detection_Bit_Flip.ipynb`](./11_Quantum_Error_Detection_Bit_Flip.ipynb) | Quantum Error Detection | Bitwise logic and parity | 3-qubit repetition code, syndrome extraction |
| [`12_Compiling_for_Google_Hardware.ipynb`](./12_Compiling_for_Google_Hardware.ipynb) | Target Hardware Compilation | Graph topology and target sets | Sycamore gate set, compilation passes |
| [`13_QAOA_Optimization_in_Cirq.ipynb`](./13_QAOA_Optimization_in_Cirq.ipynb) | QAOA in Cirq | Graph edge traversal | Alternating cost and mixer unitaries |
| [`14_Variational_Algorithms_with_SciPy.ipynb`](./14_Variational_Algorithms_with_SciPy.ipynb) | Variational Algorithms with SciPy | SciPy optimization interfaces | Hybrid classical-quantum optimization |
| [`15_Quantum_Supremacy_and_XEB_Intuition.ipynb`](./15_Quantum_Supremacy_and_XEB_Intuition.ipynb) | Quantum Supremacy and XEB | Statistical sampling distributions | Random circuit sampling, cross-entropy |

---

## Environment Setup
```bash
pip install -r requirements-cirq.txt
jupyter lab
```
