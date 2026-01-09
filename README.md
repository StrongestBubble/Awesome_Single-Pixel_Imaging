# Awesome Single-Pixel Imaging

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)

A curated list of awesome single-pixel imaging (SPI), computational ghost imaging (CGI), and related compressed sensing (CS) resources.

Single-pixel imaging involves capturing spatial information of an object using a detector without spatial resolution (a "bucket" detector) by spatially modulating the light field. It is widely used in non-visible wavelengths (THz, IR), weak light environments, and scattering media.



## Table of Contents

- [Awesome Single-Pixel Imaging](#awesome-single-pixel-imaging)
  - [Table of Contents](#table-of-contents)
  - [Introduction](#introduction)
  - [Review Articles](#review-articles)
  - [Key Papers](#key-papers)
    - [Foundations](#foundations)
    - [Reconstruction Algorithms](#reconstruction-algorithms)
    - [Deep Learning for SPI](#deep-learning-for-spi)
  - [Books](#books)
  - [Open Source Software](#open-source-software)
    - [Simulation \& Traditional Algorithms](#simulation--traditional-algorithms)
    - [CS Solvers (Toolboxes)](#cs-solvers-toolboxes)
    - [Deep Learning](#deep-learning)
  - [Global Research Groups](#global-research-groups)
    - [🇪🇺 Europe](#-europe)
      - [🇬🇧 United Kingdom (A powerhouse in the field)](#-united-kingdom-a-powerhouse-in-the-field)
    - [🌎 North America](#-north-america)
      - [🇺🇸 United States (The birthplace of theory)](#-united-states-the-birthplace-of-theory)
    - [🌏 Asia](#-asia)
      - [🇨🇳 China (Leading in engineering applications)](#-china-leading-in-engineering-applications)
  - [Contributing](#contributing)
  - [Maintainer](#maintainer)

---

## Introduction

**Single-Pixel Imaging (SPI)** (often synonymous with or related to **Ghost Imaging**) is a technique that reconstructs images using a single-point detector and structured illumination (or structured detection). By correlating the measured light intensities with the known spatial patterns (e.g., Hadamard, Fourier, Random Speckles), an image is computationally formed.

## Review Articles

*Start here to get a comprehensive understanding of the field.*

* **Single-pixel imaging 12 years on: a review** - *Gibson, G. M. et al.* (Optics Express, 2020)
    * A comprehensive guide covering theory, experimental setups, and reconstruction techniques.
    * [DOI: 10.1364/OE.403195](https://doi.org/10.1364/OE.403195)

* **Principles and prospects of single-pixel imaging** - *Edgar, M. P. et al.* (Nature Photonics, 2019)
    * Discusses the physics, signal-to-noise ratio limits, and future applications.
    * [DOI: 10.1038/s41566-018-0300-7](https://doi.org/10.1038/s41566-018-0300-7)

* **An introduction to ghost imaging: quantum and classical** - *Padgett, M. J. & Boyd, R. W.* (Phil. Trans. R. Soc. A, 2017)
    * A fundamental overview clarifying the transition from quantum to classical descriptions.
    * [DOI: 10.1098/rsta.2016.0233](https://doi.org/10.1098/rsta.2016.0233)

## Key Papers

### Foundations

* **Optical imaging by means of two-photon quantum entanglement** - *Pittman, T. B. & Shih, Y. H.* (Physical Review A, 1995)
    * The first experimental demonstration of ghost imaging using entangled photons.
    * [DOI: 10.1103/PhysRevA.52.R3429](https://doi.org/10.1103/PhysRevA.52.R3429)

* **Computational ghost imaging** - *Shapiro, J. H.* (Physical Review A, 2008)
    * Theoretical proof that only one detector is needed if the illumination patterns are pre-calculated, birthing modern SPI.
    * [DOI: 10.1103/PhysRevA.78.061802](https://doi.org/10.1103/PhysRevA.78.061802)

* **Single-pixel imaging via compressive sampling** - *Duarte, M. F. et al.* (IEEE Signal Processing Magazine, 2008)
    * The seminal "Single Pixel Camera" paper introducing Compressed Sensing (CS) to the field.
    * [DOI: 10.1109/MSP.2007.914730](https://doi.org/10.1109/MSP.2007.914730)

### Reconstruction Algorithms

* **Differential ghost imaging (DGI)** - *Ferri, F. et al.* (Physical Review Letters, 2010)
    * Introduces differential measurements to significantly improve Signal-to-Noise Ratio (SNR).
    * [DOI: 10.1103/PhysRevLett.104.253603](https://doi.org/10.1103/PhysRevLett.104.253603)

* **Normalized ghost imaging** - *Sun, B. et al.* (Optics Express, 2012)
    * A method to normalize light intensity fluctuations for better image quality.
    * [DOI: 10.1364/OE.20.016892](https://doi.org/10.1364/OE.20.016892)

* **Single-pixel imaging by means of Fourier spectrum acquisition** - *Zhang, Z. et al.* (Nature Communications, 2015)
    * High-efficiency reconstruction using deterministic Fourier basis patterns.
    * [DOI: 10.1038/ncomms7225](https://doi.org/10.1038/ncomms7225)

### Deep Learning for SPI

* **Deep-learning-based ghost imaging** - *Lyu, M. et al.* (Scientific Reports, 2017)
    * One of the earliest works applying Deep Neural Networks (DNN) to reconstruct SPI images from bucket signals.
    * [DOI: 10.1038/s41598-017-18171-7](https://doi.org/10.1038/s41598-017-18171-7)

* **Ghost imaging based on deep learning** - *He, Y. et al.* (2018)
    * Explores CNNs for imaging at very low sampling rates.
    * [DOI: 10.1038/s41598-018-24731-2](https://doi.org/10.1038/s41598-018-24731-2)

## Books

* **A Mathematical Introduction to Compressive Sensing** - *Simon Foucart & Holger Rauhut*
    * Essential for understanding the mathematics behind CS-based reconstruction.
    * [DOI: 10.1007/978-0-8176-4948-7](https://doi.org/10.1007/978-0-8176-4948-7)

* **Quantum Imaging** - *Mikhail I. Kolobov* (Springer, 2007)
    * Contains detailed chapters on the quantum mechanical origins of ghost imaging.
    * [DOI: 10.1007/0-387-33988-4](https://doi.org/10.1007/0-387-33988-4)

* **An Introduction to Single-Pixel Imaging** - *Nicolas DUCROS* (Wiley, 2024)
    * A systematic introduction to SPI designed for new researchers.
    * [DOI: 10.1002/9781394283996.ch8](https://doi.org/10.1002/9781394283996.ch8)


## Open Source Software

### Simulation & Traditional Algorithms

* **[Hadamard-Single-Pixel-Imaging](https://github.com/aloz77/Hadamard-Single-Pixel-Imaging)**
    * Example implementation of SPI using Hadamard patterns (Basis scan).
* **[Ghost-Imaging-Simulation](https://github.com/topics/ghost-imaging)**
    * *Search Link:* A collection of various MATLAB/Python scripts available on GitHub for DGI and CGI simulations.

### CS Solvers (Toolboxes)

*These solvers are essential for Total Variation (TV) and L1-norm minimization in SPI.*

* **[TVAL3](https://github.com/bunkahle/TVAL3)** (MATLAB)
    * *Total Variation Augmented Lagrangian Alternating Direction Algorithm*. The gold standard for TV-regularized reconstruction in single-pixel cameras.
* **[NESTA](https://statweb.stanford.edu/~candes/software/nesta/)** (MATLAB)
    * A fast and accurate first-order method for sparse recovery.
* **[PyLops](https://github.com/PyLops/pylops)** (Python)
    * Linear operators library for Python, useful for implementing compressive sensing optimizations without MATLAB.

### Deep Learning

* **[CSNet-Layers](https://github.com/wuzhihua/CSNet-Layers)** (Example)
    * Implementation related to Compressed Sensing Networks.

<!-- ## Research Groups

* **Miles Padgett Group** (University of Glasgow, UK)
* **Robert Boyd Group** (University of Ottawa / Rochester)
* **Han Shensheng Group** (SIOM, CAS, China)
* **Camera Culture Group** (MIT Media Lab, USA)
* **Baoqing Sun Group** (Shandong University, China)
* **Wen Chen Group** (Hong Kong Polytechnic University, China)
* **Guohai Situ Group** (University of Chinese Academy of Sciences, China)
* **Huaxia Deng Group** (University of Science and Technology of China, China)
* **Zhaoshui He Group** (Guangdong University of Technology, China) -->

## Global Research Groups

A curated list of prominent laboratories and research groups worldwide, organized by region.

### 🇪🇺 Europe

#### 🇬🇧 United Kingdom (A powerhouse in the field)

* **Miles Padgett Group** - *University of Glasgow*
    * **Key Figures**: Miles Padgett, Matthew Edgar (now independent).
    * **Focus**: A leading group with immense influence. They have published numerous foundational reviews and innovative applications (e.g., 3D SPI, Video-rate SPI, THz SPI) in *Science* and *Nature* journals.
    * **Keywords**: Orbital Angular Momentum (OAM), 3D Imaging, Real-time SPI.

* **Daniele Faccio Group** - *University of Glasgow (formerly at Heriot-Watt)*
    * **Focus**: Specializes in extreme photonics, utilizing single-pixel detectors for Non-Line-Of-Sight (NLOS) imaging and ultrafast time-resolved imaging.
    * **Keywords**: Quantum Imaging, NLOS, Ultrafast gating.

* **Jonathan Leach Group** - *Heriot-Watt University*
    * **Focus**: Combines quantum imaging with single-pixel techniques, specifically Time-of-Flight (ToF) single-pixel imaging.
    * **Keywords**: Quantum Technology, ToF SPI.

---

### 🌎 North America

#### 🇺🇸 United States (The birthplace of theory)

* **Jeffrey Shapiro Group** - *MIT*
    * **Focus**: A pioneer of **Computational Ghost Imaging (CGI)**. He theoretically proved that ghost imaging can be achieved with classical light sources without quantum entanglement, triggering the explosion of the field.
    * **Keywords**: Quantum vs. Classical debate, Gaussian-state quantum illumination.

* **DSP Group (Rice University)**
    * **Key Figures**: Richard Baraniuk, Kevin Kelly.
    * **Focus**: The birthplace of the **Single-Pixel Camera**. They pioneered the application of **Compressed Sensing (CS)** in optical imaging and are considered the ancestors of SPI algorithms.
    * **Keywords**: Compressive Sensing, DLP/DMD architectures.

* **Robert Boyd Group** - *University of Rochester / University of Ottawa*
    * **Focus**: A renowned expert in quantum nonlinear optics. Has produced extensive classic works on the physical mechanisms of ghost imaging (quantum and classical correlations).
    * **Keywords**: Quantum Imaging, Nonlinear Optics.

* **Yanhua Shih Group** - *University of Maryland, Baltimore County*
    * **Focus**: Demonstrated the historic **first two-photon ghost imaging experiment** (1995). While primarily focused on physical mechanisms, his status in the field is foundational.

---

### 🌏 Asia

#### 🇨🇳 China (Leading in engineering applications)

* **Han Shensheng Group** - *SIOM, CAS (Shanghai)*
    * **Key Figures**: Han Shensheng, Gong Wenlin, Situ Guohai.
    * **Focus**: A premier team in China. They pioneered the engineering of **Ghost Imaging Lidar** and have deep accumulation in airborne and spaceborne applications. Prof. Situ Guohai is also highly active in **Deep Learning + Scattering Imaging**.
    * **Keywords**: Ghost Imaging Lidar, Scattering media, Deep Learning.

* **Beijing Institute of Technology (BIT)**
    * **Key Figures**: Zhao Weiqian, Chen Xiyuan.
    * **Focus**: Published numerous high-quality papers on Hyperspectral SPI, Microscopic SPI, and deep learning-based reconstruction algorithms.

* **Tsinghua University**
    * **Key Figures**: Suo Jinli, Dai Qionghai.
    * **Focus**: Focuses on **Computational Photography**, combining SPI with various novel sensors and state-of-the-art algorithms.

* **University of Science and Technology of China (USTC)**
    * **Key Figures**: Li Chuanfeng, Xu Jinshi (Quantum); Xu Feihu (Single-photon).
    * **Focus**: Focuses on single-photon imaging, Non-Line-Of-Sight (NLOS) imaging, and exploring the boundaries between quantum and classical imaging.

* **Sichuan University**
    * **Key Figures**: Wang Fei.
    * **Focus**: Highly active in **Deep Learning reconstruction networks** for SPI (e.g., applying ResNet and Autoencoders to single-pixel imaging).

* **Xi'an Jiaotong University (XJTU)**
    * **Key Figures**: Shao Xiaopeng.
    * **Focus**: A renowned expert in computational imaging, with unique insights into combining **scattering** and **polarization** imaging.

## Contributing

Contributions are welcome! Please read the contribution guidelines first.
1. Fork the project.
2. Create your branch (`git checkout -b feature/AmazingPaper`).
3. Commit your changes.
4. Push to the branch.
5. Open a Pull Request.

## Maintainer

This repository is maintained by Dr. **Wenqing Su**. If you notice any errors, broken links, or have any suggestions, please feel free to contact me via email.

* 🎓 **Google Scholar**: [Wenqing Su](https://scholar.google.com/citations?user=zGcPVn0AAAAJ)
* 🔬 **ResearchGate**: [Wenqing Su](https://www.researchgate.net/profile/Wenqing-Su?ev=hdr_xprf)
* 🆔 **ORCID**: [0009-0002-7618-1568](https://orcid.org/0009-0002-7618-1568)
* 📧 **Email**: [2111904043@mail2.gdut.edu.cn](mailto:2111904043@mail2.gdut.edu.cn)

---