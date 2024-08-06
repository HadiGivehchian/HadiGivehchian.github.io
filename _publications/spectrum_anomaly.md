---
title: "Smart Radio System for Detection and Characterization of RF Anomalies"
collection: publications
permalink: /projects/spectrum_anomaly
excerpt_separator: ""
---

Data security is a vital and challenging task, specifically in the environments where the data owner does not have much control over. One possible indicator of breach or compromise of data is unexpected radio frequency (RF) transmissions. In this project, we design and implement a system that automatically detects and characterizes anomalous signals across the 6 GHz RF spectrum. To detect and separate the signals, we represent the problem as a non-negative matrix factorization problem and decompose the power spectral density (PSD) to base patterns representing different arbitrary activities in the RF spectrum. To characterize signals, we apply cyclo-stationary signal processing algorithms (e.g., spectral correlation density) to the complex RF signal and feed the resulting image as the input to a neural network. We use a transformer network trained with metric learning to infer the characteristics of the signal such as modality and modulation.
