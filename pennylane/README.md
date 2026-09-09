# Xanadu PennyLane 0.38+ Track

This track covers differentiable quantum programming and Quantum Machine Learning (QML) using Xanadu's PennyLane framework (versions 0.38+), emphasizing analytic quantum gradients, QNodes, hybrid neural networks, and classical machine learning integrations.

---

## Syllabus Overview

| Notebook | Topic | Python Concept | Quantum Concept |
|---|---|---|---|
| [`01_Python_and_PennyLane_Basics.ipynb`](./01_Python_and_PennyLane_Basics.ipynb) | Basics and Differentiable Circuits | Functional vs imperative programming | Hybrid quantum-classical computing |
| [`02_Devices_QNodes_and_Circuits.ipynb`](./02_Devices_QNodes_and_Circuits.ipynb) | Devices and QNodes | Python decorators (`@decorator`) | `default.qubit` devices, QNodes |
| [`03_Quantum_Observables_and_Measurements.ipynb`](./03_Quantum_Observables_and_Measurements.ipynb) | Observables and Measurements | Statistical moments and metrics | `expval`, `var`, `probs`, `sample` |
| [`04_Quantum_Gradients_and_Parameter_Shift.ipynb`](./04_Quantum_Gradients_and_Parameter_Shift.ipynb) | Quantum Gradients | Calculus primer and derivatives | Parameter-shift rule, `qml.grad` |
| [`05_Circuit_Optimization_with_Gradient_Descent.ipynb`](./05_Circuit_Optimization_with_Gradient_Descent.ipynb) | Optimization Algorithms | Iterative loops and convergence | Gradient descent, Adam optimizer |
| [`06_Encoding_Classical_Data_into_Qubits.ipynb`](./06_Encoding_Classical_Data_into_Qubits.ipynb) | Feature Embedding Methods | Normalization and broadcasting | Basis, Angle, Amplitude embedding |
| [`07_Variational_Quantum_Classifier.ipynb`](./07_Variational_Quantum_Classifier.ipynb) | Variational Quantum Classifier | Loss functions and decision boundaries | Parameterized quantum classifier |
| [`08_Hybrid_Quantum_Neural_Networks_PyTorch.ipynb`](./08_Hybrid_Quantum_Neural_Networks_PyTorch.ipynb) | PyTorch QNN Integration | PyTorch modules (`nn.Module`) | `TorchLayer`, hybrid backpropagation |
| [`09_Quantum_Kernel_Methods_and_QSVM.ipynb`](./09_Quantum_Kernel_Methods_and_QSVM.ipynb) | Quantum Kernels and QSVM | Gram matrices and Scikit-Learn | Quantum feature maps, SVM classification |
| [`10_Quantum_Convolutional_Neural_Networks.ipynb`](./10_Quantum_Convolutional_Neural_Networks.ipynb) | Quantum CNN (QCNN) | Pooling and dimension reduction | Quantum convolution and pooling layers |
| [`11_Solving_MaxCut_with_PennyLane_QAOA.ipynb`](./11_Solving_MaxCut_with_PennyLane_QAOA.ipynb) | QAOA with PennyLane | Cost and mixer Hamiltonians | `qml.qaoa` layers, angle optimization |
| [`12_VQE_for_Molecular_Chemistry.ipynb`](./12_VQE_for_Molecular_Chemistry.ipynb) | Quantum Chemistry VQE | Molecular geometry definitions | Molecular Hamiltonians, H2 energy |
| [`13_Barren_Plateaus_and_Trainability.ipynb`](./13_Barren_Plateaus_and_Trainability.ipynb) | Barren Plateaus | Variance scaling and log plots | Vanishing gradients in deep circuits |
| [`14_Quantum_Generative_Adversarial_Networks.ipynb`](./14_Quantum_Generative_Adversarial_Networks.ipynb) | Quantum GANs (QGAN) | Min-max adversarial games | Quantum generator vs classical discriminator |
| [`15_End_to_End_QML_Pipeline.ipynb`](./15_End_to_End_QML_Pipeline.ipynb) | End-to-End QML Capstone | Complete data pipelines | Preprocessing, PCA, training, evaluation |

---

## Environment Setup
```bash
pip install -r requirements-pennylane.txt
jupyter lab
```
