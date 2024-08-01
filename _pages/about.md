---
permalink: /
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a Ph.D. candidate in Computer Science at UC San Diego advised by [Dinesh Bharadia](https://www.google.com/url?q=http%3A%2F%2Fweb.eng.ucsd.edu%2F~dineshb%2F&sa=D) and [Aaron Schulman](https://www.google.com/url?q=http%3A%2F%2Fcseweb.ucsd.edu%2F~schulman%2F&sa=D). I am a part of [Sysnet](https://www.google.com/url?q=http%3A%2F%2Fwww.sysnet.ucsd.edu%2Fsysnet%2F&sa=D), [CNS](https://www.google.com/url?q=https%3A%2F%2Fcns.ucsd.edu&sa=D) and [WCSNG](https://www.google.com/url?q=http%3A%2F%2Fwcsng.ucsd.edu%2Findex.html&sa=D) research groups. My research involves developing machine learning and signal processsing algorithms to solve different problems in wireless sensing, communication and security. My research is supported by IARPA and the Qualcomm Innovation Fellowship. I have also interned at Qualcomm for two summers, where I developed and implemented deep learning architectures and signal processing algorithms for WiFi sensing.
<br>

Before joining UCSD, I got my B.Sc. degree in Electrical Engineering (Communication Systems) from Sharif University of Technology, under the supervision of [Mohammad-Ali Maddah-Ali](https://scholar.google.com/citations?user=CFIJZwoAAAAJ&hl=en) and [Babak Khalaj](https://www.google.com/url?q=http%3A%2F%2Fsharif.edu%2F~khalaj%2F&sa=D). I worked on probabilistic modeling and designing efficient memory sharing algorithms for Big Data processing systems using information theoretic approaches.

<br>

## Publications

[**Practical Obfuscation of BLE Physical-Layer Fingerprints on Mobile Devices**](http://HadiGivehchian.github.io/files/oakland24_phyobfuscation.pdf) <br>
**Hadi Givehchian**, Nishant Bhaskar, Alexander Redding, Han Zhao, Aaron Schulman, Dinesh Bharadia <br>
2024 IEEE Symposium on Security and Privacy (SP)

[**Spoofing attack detection in the physical layer with commutative neural networks**](https://arxiv.org/pdf/2211.04269.pdf) <br>
Daniel Romero, Peter Gerstoft, **Hadi Givehchian**, Dinesh Bharadia

[**Protecting bluetooth user privacy through obfuscation of carrier frequency offset**](https://ieeexplore.ieee.org/abstract/document/9926141) <br>
Ali Nikoofard, **Hadi Givehchian**, Nishant Bhaskar, Aaron Schulman, Dinesh Bharadia, Patrick P Mercier <br>
2022 IEEE Transactions on Circuits and Systems II

[**Evaluating Physical-Layer BLE Location Tracking Attacks on Mobile Devices**](https://ieeexplore.ieee.org/abstract/document/9833758) <br>
**Hadi Givehchian**, Nishant Bhaskar, Eliana Rodriguez Herrera, Héctor Rodrigo López Soto, Christian Dameff, Dinesh Bharadia, Aaron Schulman <br>
2022 IEEE Symposium on Security and Privacy (SP) <br>
Media Coverage: [The Register](https://www.theregister.com/2021/10/22/bluetooth_tracking_device/) 
&nbsp;&nbsp;
[IEEE Spectrum](https://spectrum.ieee.org/bluetooth-security)
&nbsp;&nbsp;
[Tom's Guide](https://www.tomsguide.com/news/bluetooth-device-tracking)
&nbsp;&nbsp;
[India Today](https://www.indiatoday.in/technology/news/story/bluetooth-on-phone-can-reveal-the-location-of-a-user-a-new-study-finds-1874760-2021-11-09)

<br>

## Patents
**RF-sensing-based human identification using combined gait and shape recognition** <br>
**Hadi Givehchian**, Xiaoxin Zhang, Peyman Siyari

**Generating indoor maps based on radio frequency sensing** <br>
**Hadi Givehchian**, Xiaoxin Zhang, Peyman Siyari

<br>

## Current Projects

**Smart Radio System for Detection and Characterization of RF Anomalies**
* Data security is a vital and challenging task, specifically in the environments where the data owner does not have much control over. One possible indicator of breach or compromise of data is unexpected radio frequency (RF) transmissions. In this project, we design and implement a system that automatically detects and characterizes anomalous signals across the 6 GHz RF spectrum. To detect and separate the signals, we represent the problem as a non-negative matrix factorization problem and decompose the power spectral density (PSD) to base patterns representing different arbitrary activities in the RF spectrum. To characterize signals, we apply cyclo-stationary signal processing algorithms (e.g., spectral correlation density) to the complex RF signal and feed the resulting image as the input to a neural network. We use a transformer network trained with metric learning to infer the characteristics of the signal such as modality and modulation.

<br>

**Deep Learning Framework for RF Fingerprinting**
* Hardware imperfections caused by manufacturing process leave a unique fingerprint in the signal sent by IoT devices, making it possible to identify devices even from the same make and model. However, different wireless signals (Wi-Fi, BLE, ZigBee, etc.) demand different algorithms to estimate such imperfection from the received signal. In addition, these imperfections are usually minuscule, and hard to measure accurately and fine enough to identify a large number of devices. In this project, we develop a deep learning framework that can be trained on an arbitrary wireless technology, and extract distinguishable fingerprints from these signals to uniquely identify and/or verify a large number of transmitter devices. We use deep metric learning to learn feature embeddings with low within-class and high inter-class variance, so that we can distinguish a large number of devices. Once the network is trained on a set of devices, it can be used as a feature extractor to detect new un-seen devices. Further, we use data augmentation and ensemble of signal slices to make the embeddings robust to wireless channel conditions and packet contents, and use domain adaptation to map the learned embeddings across different receivers. We also use the perfect signal (without hardware imperfections) as the input during training so that the network can learn the hardware imperfection embeddings easier for any type of modulation and wireless protocol. The intuition is that the distortion caused by hardware imperfections  can be modeled as a function applied to the perfect signal. The network can be trained to approximate this function and estimate the hardware imperfection embeddings.

<p align="center">
 <img src="http://HadiGivehchian.github.io/images/test_tsne.jpg" alt="train_perf_fig" width="400"/>
    <br>
    <em>TSNE of the fingerprint embeddings for WiFi transmitters.</em>
</p>


<!---
## News

* July 2023: [IEEE S&P (Oakland) 2024 paper](http://HadiGivehchian.github.io/files/oakland24_phyobfuscation.pdf) accepted on Practical Obfuscation of BLE Physical-Layer Fingerprints on Mobile Devices.
* March 2023: Our team successfully passed phase 1 of [SCISRS](https://www.iarpa.gov/research-programs/scisrs) program. This was a year-long effort to build an end-to-end system to automatically detect and characterize RF anomalies in complex RF environments using machine learning and signal processing.
* Oct 2022: [TCAS-II paper](https://ieeexplore.ieee.org/abstract/document/9926141) accepted on Protecting bluetooth user privacy through obfuscation of carrier frequency offset.
* July 2021: [IEEE S&P (Oakland) 2022 paper](https://ieeexplore.ieee.org/abstract/document/9833758) accepted on Evaluating physical-layer ble location tracking attacks on mobile devices.
* June 2021: I am returning to Qualcomm for summer internship. I will work on human gait and shape recognition using Wi-Fi RF sensing and deep learning.
* May 2021: I received my master's degree.
* June 2020: I am joining Qualcomm for summer internship. I will work on indoor map generation using Wi-Fi RF sensing and deep learning.
* May 2019: We won the [Qualcomm Innovation Fellowship 2019](https://www.qualcomm.com/research/university-relations/innovation-fellowship/winners).
-->

