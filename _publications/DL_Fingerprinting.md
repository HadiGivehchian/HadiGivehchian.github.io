---
title: "Deep Learning Framework for RF Fingerprinting"
collection: publications
permalink: /projects/DL_Fingerprinting
excerpt_separator: ""
---
Hardware imperfections caused by manufacturing process leave a unique fingerprint in the signal sent by IoT devices, making it possible to identify devices even from the same make and model. However, different wireless signals (Wi-Fi, BLE, ZigBee, etc.) demand different algorithms to estimate such imperfection from the received signal. In addition, these imperfections are usually minuscule, and hard to measure accurately and fine enough to identify a large number of devices. In this project, we develop a deep learning framework that can be trained on an arbitrary wireless technology, and extract distinguishable fingerprints from these signals to uniquely identify and/or verify a large number of transmitter devices. We use deep metric learning to learn feature embeddings with low within-class and high inter-class variance, so that we can distinguish a large number of devices. Once the network is trained on a set of devices, it can be used as a feature extractor to detect new un-seen devices. Further, we use data augmentation and ensemble of signal slices to make the embeddings robust to wireless channel conditions and packet contents, and use domain adaptation to map the learned embeddings across different receivers. We also use the perfect signal (without hardware imperfections) as the input during training so that the network can learn the hardware imperfection embeddings easier for any type of modulation and wireless protocol. The intuition is that the distortion caused by hardware imperfections  can be modeled as a function applied to the perfect signal. The network can be trained to approximate this function and estimate the hardware imperfection embeddings.

<p align="center">
 <img src="http://HadiGivehchian.github.io/images/test_tsne.jpg" alt="train_perf_fig" width="400"/>
    <br>
    <em>TSNE of the fingerprint embeddings for WiFi transmitters.</em>
</p>
