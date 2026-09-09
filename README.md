# Introduction to Quantum Computing and Quantum Machine Learning
### A Multi-Framework Curriculum: IBM Qiskit, Google Cirq, and Xanadu PennyLane

[![License: Apache 2.0](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](./LICENSE)
[![Python Versions](https://img.shields.io/badge/Python-3.10%20%7C%203.11-brightgreen.svg)](https://www.python.org/)
[![Qiskit Version](https://img.shields.io/badge/Qiskit-1.x%20(Primitives%20V2)-purple.svg)](https://qiskit.org/)
[![Cirq Version](https://img.shields.io/badge/Cirq-1.4+-yellow.svg)](https://quantumai.google/cirq)
[![PennyLane Version](https://img.shields.io/badge/PennyLane-0.38+-teal.svg)](https://pennylane.ai/)

This repository provides an educational curriculum in quantum computing and quantum machine learning (QML) designed specifically for Python beginners. The curriculum is partitioned into three independent, comprehensive tracks focusing on the industry's primary open-source quantum programming frameworks.

---

## Architectural Comparison of Frameworks

| Framework | Primary Focus | Distinctive Architectural Paradigm | Target Use Case |
|---|---|---|---|
| **IBM Qiskit** | Gate-level circuits & cloud hardware | Primitives V2 (`SamplerV2`, `EstimatorV2`) and pass managers | General-purpose quantum algorithms, chemistry, and IBM hardware |
| **Google Cirq** | NISQ hardware & pulse/moment control | Time-sliced `Moment` architecture and 2D `GridQubit` topologies | Direct hardware control, noise modeling, and Google Sycamore architectures |
| **Xanadu PennyLane** | Differentiable quantum programming & QML | `@qml.qnode` decorators and parameter-shift differentiation | Variational classifiers, quantum neural networks, and PyTorch/JAX integration |

---

## Curriculum Overview

Each track contains 15 sequentially structured Jupyter Notebooks progressing from foundational programming concepts to advanced variational algorithms.

### Track 1: IBM Qiskit 1.x / 2.x ([`qiskit/`](./qiskit))

1. **`01_Python_and_Qiskit_Setup.ipynb`**: Python fundamentals, installing Qiskit 1.x, and first circuit construction.
2. **`02_Single_Qubit_Superposition.ipynb`**: Computational basis states, Hadamard transformation, and statevector inspection.
3. **`03_Quantum_Gates_and_Rotations.ipynb`**: Pauli operators (X, Y, Z), phase gates (S, T), and arbitrary rotation angles (Rx, Ry, Rz).
4. **`04_Entanglement_and_Bell_States.ipynb`**: Multi-qubit registers, Controlled-NOT (CNOT) operation, and Bell state preparation.
5. **`05_Sampling_with_Primitives_V2.ipynb`**: Measurement mechanics, finite-shot sampling, and `StatevectorSampler` with Primitive Unified Blocs (PUBs).
6. **`06_Visualizing_Quantum_States.ipynb`**: Circuit schematics, Bloch sphere projections, and state density plots.
7. **`07_Quantum_Random_Number_Generator.ipynb`**: Intrinsic quantum non-determinism, multi-bit sampling, and integer generation.
8. **`08_Quantum_Teleportation.ipynb`**: Teleportation protocol, Bell basis measurement, and feed-forward state reconstruction.
9. **`09_Superdense_Coding.ipynb`**: Transmission of two classical bits using a single entangled qubit.
10. **`10_Deutsch_Jozsa_Algorithm.ipynb`**: Quantum parallelism, black-box oracles, and phase kickback analysis.
11. **`11_Quantum_Phase_Estimation_and_QFT.ipynb`**: Quantum Fourier Transform decomposition and unitary eigenvalue extraction.
12. **`12_Grovers_Search_Algorithm.ipynb`**: Unstructured search, oracle construction, and amplitude amplification iterations.
13. **`13_Shors_Factoring_Algorithm.ipynb`**: Order-finding modular arithmetic and RSA factorization reduction.
14. **`14_VQE_with_Estimator_V2.ipynb`**: Rayleigh-Ritz variational principle, molecular Hamiltonians, and ground state optimization via `EstimatorV2`.
15. **`15_QAOA_MaxCut_Optimization.ipynb`**: Combinatorial optimization on graphs using alternating cost and mixer Hamiltonians.

---

### Track 2: Google Cirq 1.4+ ([`cirq/`](./cirq))

1. **`01_Python_and_Cirq_Architecture.ipynb`**: Cirq hardware abstractions, `LineQubit`, `GridQubit`, and `NamedQubit` structures.
2. **`02_Qubits_Moments_and_Circuits.ipynb`**: Temporal time-slice organization (`Moment`) and circuit assembly patterns.
3. **`03_Single_Qubit_Gates_and_Operations.ipynb`**: Fractional gate powers, phased operators, and unitary matrix conversions.
4. **`04_Multi_Qubit_Gates_and_Entanglement.ipynb`**: Two-qubit gates (CNOT, CZ, SWAP, ISWAP) and state representations.
5. **`05_Simulating_Circuits_and_Sampling.ipynb`**: Pure-state simulation (`simulate()`) versus shot-based hardware execution (`run()`).
6. **`06_Parameterized_Circuits_and_Sweeps.ipynb`**: Symbolic parameters with SymPy and multi-dimensional parameter sweeps.
7. **`07_Quantum_Teleportation_in_Cirq.ipynb`**: Classical feed-forward conditioning and fidelity verification in Cirq.
8. **`08_Grovers_Algorithm_in_Cirq.ipynb`**: Modular oracle sub-circuits and diffusion moments.
9. **`09_Quantum_Fourier_Transform.ipynb`**: Recursive QFT implementation and automated circuit inversion.
10. **`10_Simulating_Noisy_Quantum_Channels.ipynb`**: Bit-flip, phase-flip, and depolarizing noise with `DensityMatrixSimulator`.
11. **`11_Quantum_Error_Detection_Bit_Flip.ipynb`**: Three-qubit repetition code, ancilla syndrome extraction, and error correction.
12. **`12_Compiling_for_Google_Hardware.ipynb`**: Grid connectivity constraints, Sycamore gate set decomposition, and circuit optimization passes.
13. **`13_QAOA_Optimization_in_Cirq.ipynb`**: Graph problem formulation and alternating unitary dynamics in Cirq.
14. **`14_Variational_Algorithms_with_SciPy.ipynb`**: Hybrid quantum-classical optimization interfacing Cirq with SciPy solvers.
15. **`15_Quantum_Supremacy_and_XEB_Intuition.ipynb`**: Random circuit sampling benchmarks and Cross-Entropy Benchmarking (XEB) principles.

---

### Track 3: Xanadu PennyLane 0.38+ ([`pennylane/`](./pennylane))

1. **`01_Python_and_PennyLane_Basics.ipynb`**: Differentiable quantum programming paradigms and framework architecture.
2. **`02_Devices_QNodes_and_Circuits.ipynb`**: Device initializations and the `@qml.qnode` functional decorator.
3. **`03_Quantum_Observables_and_Measurements.ipynb`**: Expectation values (`expval`), variances (`var`), probabilities (`probs`), and sampling.
4. **`04_Quantum_Gradients_and_Parameter_Shift.ipynb`**: Analytic quantum gradients via the parameter-shift rule and `qml.grad`.
5. **`05_Circuit_Optimization_with_Gradient_Descent.ipynb`**: Gradient descent and Adam optimization of parameterized circuits.
6. **`06_Encoding_Classical_Data_into_Qubits.ipynb`**: Classical-to-quantum embeddings: Basis, Angle, and Amplitude embeddings.
7. **`07_Variational_Quantum_Classifier.ipynb`**: Complete binary classifier pipeline using strongly entangling layers.
8. **`08_Hybrid_Quantum_Neural_Networks_PyTorch.ipynb`**: Direct integration of QNodes into PyTorch architectures using `TorchLayer`.
9. **`09_Quantum_Kernel_Methods_and_QSVM.ipynb`**: Quantum feature spaces, kernel matrices, and scikit-learn Support Vector Machines.
10. **`10_Quantum_Convolutional_Neural_Networks.ipynb`**: Hierarchical quantum convolutional and pooling layers for dimensional reduction.
11. **`11_Solving_MaxCut_with_PennyLane_QAOA.ipynb`**: Automated cost and mixer Hamiltonian generation with `qml.qaoa`.
12. **`12_VQE_for_Molecular_Chemistry.ipynb`**: Electronic structure calculations and molecular ground state energy estimation.
13. **`13_Barren_Plateaus_and_Trainability.ipynb`**: Gradient variance scaling in deep parameterized circuits and mitigation techniques.
14. **`14_Quantum_Generative_Adversarial_Networks.ipynb`**: Quantum generator and classical discriminator architectures for distribution learning.
15. **`15_End_to_End_QML_Pipeline.ipynb`**: Capstone classification pipeline: feature scaling, PCA, training, and classical benchmarking.

---

## Environment Configuration & Setup

Python 3.10 or 3.11 is recommended.

### Unified Environment
```bash
# Create and activate virtual environment
python -m venv .venv
# On Windows:
.venv\Scripts\activate
# On Linux/macOS:
source .venv/bin/activate

# Install all dependencies
pip install -r requirements.txt

# Launch JupyterLab
jupyter lab
```

### Track-Specific Environments
To install dependencies for a single framework:
```bash
# IBM Qiskit:
pip install -r qiskit/requirements-qiskit.txt

# Google Cirq:
pip install -r cirq/requirements-cirq.txt

# Xanadu PennyLane:
pip install -r pennylane/requirements-pennylane.txt
```

---

## Automated Test Suite

To verify that all 45 notebooks execute without warnings or errors:
```bash
python scripts/run_notebook_tests.py
```

---

## License

This project is licensed under the Apache 2.0 License. See the [LICENSE](./LICENSE) file for details.
