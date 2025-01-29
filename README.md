<!-- markdownlint-disable first-line-h1 -->
<!-- markdownlint-disable html -->
<!-- markdownlint-disable no-duplicate-header -->

<a name="top"></a>
<div align="center">
  <img src="./equal1.png" style="width: 200px;"/>
</div>

---

<div align="center">
   <a href="mailto:erik.staszewski@gmail.com"><b>Email Me</b></a> | <a href="https://www.linkedin.com/in/estaszewski/"><b>My LinkedIn</b></a> | <a href="https://equal1.com/"><b>Equal1 Site</b></a>
</div>

## 1. Introduction

This project, by Erik Staszewski under the supervision of David Redmond for Equal1, seeks to implement and extend quantum computing techniques for credit card fraud detection.

The project focuses on constructing a Graph Neural Network (GNN) and Quantum Graph Neural Network (QGNN) for binary classification of fraudulent and non-fraudulent credit card transactions. Results are measured and compared using precision, recall, and $F_1$-scores, and plotted using Receiver Operating Characteristic and Precision-Recall Curves.

## 2. Model Summary

**Architecture**

- The model is based on GNNs, using GraphSAGE and GCN/SGConv for neighborhood aggregation and feature learning.
- Quantum Computing is integrated through a QGNN, which incorporates a quantum processing layer to explore potential advantages in feature transformations and data entanglement.
- The quantum layer uses parameterized quantum circuits (PQC) with RX and RY gates to encode features.

**Training Pipeline**

- GNN Model:
  - Uses GraphSAGE as the main convolutional layer.
  - Trained for 100 epochs, optimizing with Adam optimizer and BCELoss for fraud detection.
  - Employs batch normalization and adaptive pooling to stabilize training and ensure scalability.
- QGNN Model:
  - Uses Quantum Circuits with 1-qubit RX, RY gates.
  - Training uses gradient-based updates using the parameter shift rule, allowing backpropagation through quantum gates.
  - Explores quantum entanglement and multi-qubit extensions to test their impact on learning performance.

