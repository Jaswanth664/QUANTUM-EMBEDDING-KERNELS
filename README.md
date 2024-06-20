# QUANTUM-EMBEDDING-KERNELS
Here's the revised README file content for the `JassuQCG_2.ipynb` file, updated to reflect the use of the Iris dataset.

---

# Quantum Machine Learning: SVM with Quantum Kernel Embedding

## Overview

This project demonstrates the implementation of a quantum machine learning model using Quantum Embedding Kernels (QEKs) for a binary classification task. The model employs a parameterized quantum circuit to embed data into quantum states, computes the QEK matrix, optimizes the variational parameters, and trains a support vector machine (SVM) classifier using the optimized QEK matrix. The example dataset used here is the Iris dataset from scikit-learn, focusing on a binary classification task.

## Features

- Implementation of a parameterized quantum circuit for embedding data into quantum states.
- Computation of the Quantum Embedding Kernel (QEK) matrix for the dataset.
- Optimization of the variational parameters by maximizing the kernel-target alignment.
- Application of an SVM classifier using the optimized QEK matrix.
- Visualization of the decision boundary generated by the SVM classifier.

## Requirements

- Python 3.x
- Pennylane
- Pennylane-Lightning
- NumPy
- Scikit-learn
- SciPy
- Joblib
- Matplotlib

## Installation

To install the required packages, run:

```bash
pip install pennylane pennylane-lightning numpy scikit-learn scipy joblib matplotlib
```

## Usage

1. Clone the repository or download the `JassuQCG_2.ipynb` file.
2. Open the notebook file in Jupyter Notebook or JupyterLab.
3. Run the cells sequentially to execute the code.

## Code Explanation

### Loading the Dataset

The Iris dataset is loaded using scikit-learn. Only samples from two classes (class 0 and class 1) are selected for the binary classification task.

### Quantum Feature Map and Variational Circuit

A parameterized quantum circuit is defined using Pennylane, where each feature is encoded using rotation gates.

### Optimization

The variational parameters of the quantum circuit are optimized to maximize the kernel-target alignment, which measures the agreement between the kernel matrix and the target labels.

### Training and Evaluation

An SVM classifier is trained using the optimized QEK matrix. The dataset is split into training and testing sets, and the model is evaluated on the test set.

### Visualization

The decision boundary of the SVM classifier is visualized using a mesh grid, and the classification accuracy is displayed.

## Visualization

A contour plot is generated to visualize the decision boundary of the SVM classifier. Different colors are used to represent different classes, and the data points are plotted with edge colors to highlight the class labels.

## Results

The classification accuracy is printed, and the decision boundary is visualized to demonstrate the effectiveness of the quantum kernel embedding for the binary classification task.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes.


---

This README file provides a comprehensive overview of the project, including installation instructions, usage details, and an explanation of the code and its features. It also highlights the visualization and results obtained from the quantum machine learning model using the Iris dataset.
