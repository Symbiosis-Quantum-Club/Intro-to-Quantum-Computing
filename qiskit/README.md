# IBM Qiskit 1.x / 2.x Track

This track covers quantum computing using IBM's Qiskit SDK (versions 1.2+ and 2.x), adhering strictly to modern Primitives V2 conventions (`StatevectorSampler`, `StatevectorEstimator`, and `qiskit_aer`).

---

## Syllabus Overview

| Notebook | Topic | Python Concept | Quantum Concept |
|---|---|---|---|
| [`01_Python_and_Qiskit_Setup.ipynb`](./01_Python_and_Qiskit_Setup.ipynb) | Setup and First Circuit | Variables, imports, basic functions | Qubits, QuantumCircuit, simulation |
| [`02_Single_Qubit_Superposition.ipynb`](./02_Single_Qubit_Superposition.ipynb) | Superposition and Statevectors | Lists and complex numbers | Hadamard gate, statevectors |
| [`03_Quantum_Gates_and_Rotations.ipynb`](./03_Quantum_Gates_and_Rotations.ipynb) | Single-Qubit Gates and Rotations | Math constants, function parameters | Pauli X, Y, Z, S, T, Rx, Ry, Rz |
| [`04_Entanglement_and_Bell_States.ipynb`](./04_Entanglement_and_Bell_States.ipynb) | Entanglement and Bell States | Tuples and multi-arguments | CNOT gate, 4 Bell states |
| [`05_Sampling_with_Primitives_V2.ipynb`](./05_Sampling_with_Primitives_V2.ipynb) | Measurement and Primitives V2 | Dictionaries and PUBs | Measurement, shots, SamplerV2 |
| [`06_Visualizing_Quantum_States.ipynb`](./06_Visualizing_Quantum_States.ipynb) | State Visualizations | Matplotlib figure formatting | Bloch sphere, density city plots |
| [`07_Quantum_Random_Number_Generator.ipynb`](./07_Quantum_Random_Number_Generator.ipynb) | Quantum Randomness | Loops and binary conversions | QRNG, uniform integer sampling |
| [`08_Quantum_Teleportation.ipynb`](./08_Quantum_Teleportation.ipynb) | Quantum Teleportation | Conditional branches and checks | Alice and Bob protocol, state transfer |
| [`09_Superdense_Coding.ipynb`](./09_Superdense_Coding.ipynb) | Superdense Coding | Binary encoding and decoding | Transmitting two classical bits |
| [`10_Deutsch_Jozsa_Algorithm.ipynb`](./10_Deutsch_Jozsa_Algorithm.ipynb) | Deutsch-Jozsa Algorithm | Lambda abstractions and oracles | Quantum parallelism, phase kickback |
| [`11_Quantum_Phase_Estimation_and_QFT.ipynb`](./11_Quantum_Phase_Estimation_and_QFT.ipynb) | QFT and Phase Estimation | Recursion and modular indexing | Quantum Fourier Transform, phases |
| [`12_Grovers_Search_Algorithm.ipynb`](./12_Grovers_Search_Algorithm.ipynb) | Grover's Search Algorithm | Iteration count formulas | Oracle inversion, diffusion operator |
| [`13_Shors_Factoring_Algorithm.ipynb`](./13_Shors_Factoring_Algorithm.ipynb) | Shor's Factoring Algorithm | Greatest common divisor math | Period finding, order finding |
| [`14_VQE_with_Estimator_V2.ipynb`](./14_VQE_with_Estimator_V2.ipynb) | VQE with EstimatorV2 | SciPy minimization callables | Variational ansatz, molecular ground state |
| [`15_QAOA_MaxCut_Optimization.ipynb`](./15_QAOA_MaxCut_Optimization.ipynb) | QAOA Max-Cut Optimization | Graph modeling with NetworkX | Cost and mixer unitaries, graph cuts |

---

## Environment Setup
```bash
pip install -r requirements-qiskit.txt
jupyter lab
```
