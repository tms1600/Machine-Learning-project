Antihydrogen Annihilation Detection with Deep Neural Networks
Overview

This project focuses on improving the detection of antihydrogen annihilation events recorded by detectors surrounding an antimatter trap using Deep Neural Networks (DNNs). The analysis supports experiments testing fundamental CPT symmetry.

The dataset is generated using Monte Carlo simulations to reflect realistic conditions of the ASACUSA experiment. The DNN processes the data through multiple separate paths, which are later fused via convolution in the hidden layers. Each path alternates 1D convolutional layers and max-pooling, accounting for the detector’s translational invariances.

Method

Data: Simulated Monte Carlo datasets replicating ASACUSA experimental conditions.

Model Architecture: Multi-path Convolutional Neural Network (CNN) with fused hidden layers.

Training Objective: Detect antihydrogen annihilation events from raw detector data.

Results

The DNN significantly outperforms the traditional Vertex Finding (VF) algorithm.

Raw data binary classification: AUC = 0.868 (two-channel CNN).

Two-channel subdataset: AUC = 0.881 for events hitting both detector layers.

End-to-end deep learning extracts more statistical information from raw data, improving coverage of critical event types.

Key Features

Application of deep learning to fundamental physics experiments.

Multi-path CNN architecture respecting detector geometry and invariances.

Comprehensive comparison with classical analysis methods.

Fully reproducible with simulated datasets.

Requirements

Python 3.x

TensorFlow or PyTorch

NumPy, Pandas

Matplotlib / Seaborn for visualization
