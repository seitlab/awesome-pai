<div align="center">
# Physical AI: A Comprehensive Survey of Enabling Technologies From
A Systems Perspective

[![arXiv](https://img.shields.io/badge/arXiv-coming_soon-b31b1b.svg)](#)
[![Hugging Face](https://img.shields.io/badge/🤗_Hugging_Face-Paper-yellow.svg)](#)
[![Website](https://img.shields.io/badge/Website-Link-0A66C2.svg)](#)
[![GitHub](https://img.shields.io/badge/GitHub-Repo-181717.svg?logo=github)](#)

Shengding Liu<sup>1</sup>, Zhanwei Zhang<sup>1</sup>, Zhiying Li<sup>1</sup>, Yudi Lin<sup>2</sup>, Ruxin Lin<sup>1</sup>, Xiaoqun Liu<sup>1</sup>, Khang Nguyen<sup>1</sup>, Ziran Gao<sup>1</sup>, Guopeng Liao<sup>3</sup>, Jingxiang Mo<sup>4</sup>, Linshan Jiang<sup>2</sup>, Jianfei Yang<sup>2</sup>, Osher Azulay<sup>5</sup>, Stella X. Yu<sup>5</sup>, Philip S. Yu<sup>6</sup>, Qiben Yan<sup>1,†</sup>

<sup>1</sup>Michigan State University, <sup>2</sup>Nanyang Technological University,
<sup>3</sup>Meta, <sup>4</sup>Gradient Robotics,
<sup>5</sup>University of Michigan, <sup>6</sup>University of Illinois Chicago

<sup>†</sup>Corresponding Author

</div>

This repository accompanies our survey **Physical AI: A Comprehensive Survey** — a system-level survey of Physical AI (PAI) that connects multimodal physical perception, embodied cognition, real-world actuation, and the simulators, data, and digital twins required to build and evaluate such systems.

- 📄 We maintain a curated list of papers, code, websites, models, benchmarks, and datasets covering the full PAI loop: **Perception → Cognition → Actuation & Execution → Building Blocks (Simulators, Data, Benchmarks, Digital Twins).**
- 🤖 The list is organized around the four pillars used in the survey, with each section grouped by the methodological theme (e.g., physics-informed perception, world models, motion planning, simulation-based data generation).
- 💛 If you find missing papers, outdated links, or incorrect metadata, feel free to open an issue or submit a pull request!

---

## Table of Contents

- [1. Physical Perception](#1-physical-perception)
  - [Perception Modalities](#perception-modalities)
  - [Physics-Informed Perception](#physics-informed-perception)
  - [Data-Driven Perception](#data-driven-perception)
  - [Generative Perception](#generative-perception)
  - [Sensor Fusion and Multimodal Perception](#sensor-fusion-and-multimodal-perception)
  - [Perception Tasks](#perception-tasks)
- [2. Physical Cognition](#2-physical-cognition)
  - [State Representation and Abstraction](#state-representation-and-abstraction)
  - [World Models](#world-models)
  - [Reasoning and Planning](#reasoning-and-planning)
  - [Memory](#memory)
  - [Alignment](#alignment)
  - [Future Directions (Cognition)](#future-directions-cognition)
- [3. Physical Actuation and Execution](#3-physical-actuation-and-execution)
- [4. Building PAI](#4-building-pai)
  - [Simulators](#simulators)
  - [Data Collection](#data-collection)
  - [Simulation Benchmarks](#simulation-benchmarks)
  - [Real-World Validation Protocols](#real-world-validation-protocols)
  - [Digital Twin](#digital-twin)

---

## 1. Physical Perception

<a id="perception-modalities"></a>

### Perception Modalities

#### Optical
- **[MobiCom'21]** *Shrimp: a robust underwater visible light communication system*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)]()
- **[MobiCom'22]** *MobiDepth: Real-Time Depth Estimation Using On-Device Dual Cameras*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)]()
- **[MobiCom'23]** *MobiSpectral: Hyperspectral Imaging on Mobile Devices*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)](https://doi.org/10.1145/3570361.3613296)
- **[MobiSys'24]** *Practical Optical Camera Communication Behind Unseen and Complex Backgrounds*
  [![Paper](https://img.shields.io/badge/Paper-MobiSys-4B5D67.svg)](https://doi.org/10.1145/3643832.3661866)
- **[MobiSys'25]** *MobiChem: A Ubiquitous Smartphone-Based Toolkit for Practical Fruit Monitoring and Analysis*
  [![Paper](https://img.shields.io/badge/Paper-MobiSys-4B5D67.svg)](https://doi.org/10.1145/3711875.3729135)

#### Acoustic
- **[IMWUT'22]** *Enabling Contact-free Acoustic Sensing under Device Motion*
  [![Paper](https://img.shields.io/badge/Paper-IMWUT-4B5D67.svg)](https://doi.org/10.1145/3550329)
- **[IPSN'23]** *Addressing Practical Challenges in Acoustic Sensing To Enable Fast Motion Tracking*
  [![Paper](https://img.shields.io/badge/Paper-IPSN-4B5D67.svg)](https://doi.org/10.1145/3583120.3586954)
- **[MobiSys'23]** *DF-Sense: Multi-user Acoustic Sensing for Heartbeat Monitoring with Dualforming*
  [![Paper](https://img.shields.io/badge/Paper-MobiSys-4B5D67.svg)](https://doi.org/10.1145/3581791.3596867)
- **[MobiSys'24]** *Enabling 6D Pose Tracking on Your Acoustic Devices*
  [![Paper](https://img.shields.io/badge/Paper-MobiSys-4B5D67.svg)](https://doi.org/10.1145/3643832.3661875)
- **[SenSys'25]** *RAM-Hand: Robust Acoustic Multi-Hand Pose Reconstruction Using a Microphone Array*
  [![Paper](https://img.shields.io/badge/Paper-SenSys-4B5D67.svg)](https://doi.org/10.1145/3715014.3722055)

#### Tactile
- **[Frontiers in Robotics and AI'24]** *Soft touchless sensors and touchless sensing for soft robots*
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.3389/frobt.2024.1224216)
- **[Sensors'20]** *PeriSense: Ring-Based Multi-Finger Gesture Interaction Utilizing Capacitive Proximity Sensing*
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.3390/s20143990)
- **[Frontiers in Robotics and AI'22]** *Tactile Sensing for Minimally Invasive Surgery: Conventional Methods and Potential Emerging Tactile Technologies*
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.3389/frobt.2021.705662)
- **[UIST'24]** *HandPad: Make Your Hand an On-the-go Writing Pad via Human Capacitance*
  [![Paper](https://img.shields.io/badge/Paper-UIST-4B5D67.svg)](https://doi.org/10.1145/3654777.3676328)
- **[IMWUT'23]** *Mocapose: Motion capturing with textile-integrated capacitive sensors in loose-fitting smart garments*
  [![Paper](https://img.shields.io/badge/Paper-IMWUT-4B5D67.svg)]()

#### RF
- **[MobiCom'20]** *Towards 3D human pose construction using wifi*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)](https://doi.org/10.1145/3372224.3380900)
- **[MobiCom'21]** *Millimetro: mmWave retro-reflective tags for accurate, long range localization*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)]()
- **[MobiCom'24]** *Around the Corner mmWave Imaging in Practical Environments*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)](https://doi.org/10.1145/3636534.3690671)
- **[MobiCom'24]** *Fine-grained Textile Moisture Sensing with Commodity UWB*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)](https://doi.org/10.1145/3636534.3690679)
- **[SenSys'25]** *Proteus: Enhanced mmWave Leaf Wetness Detection with Cross-Modality Knowledge Transfer*
  [![Paper](https://img.shields.io/badge/Paper-SenSys-4B5D67.svg)](https://doi.org/10.1145/3715014.3722052)

#### Thermal
- **[IMWUT'23]** *Feeling the temperature of the room: Unobtrusive thermal display of engagement during group communication*
  [![Paper](https://img.shields.io/badge/Paper-IMWUT-4B5D67.svg)]()
- **[IMWUT'23]** *Feverphone: Accessible core-body temperature sensing for fever monitoring using commodity smartphones*
  [![Paper](https://img.shields.io/badge/Paper-IMWUT-4B5D67.svg)]()
- **[IPSN'20]** *LOCI: Privacy-aware, Device-free, Low-power Localization of Multiple Persons using IR Sensors*
  [![Paper](https://img.shields.io/badge/Paper-IPSN-4B5D67.svg)](https://doi.org/10.1109/ipsn48710.2020.00018)
- **[CHI'23]** *HotFoot: Foot-Based User Identification Using Thermal Imaging*
  [![Paper](https://img.shields.io/badge/Paper-CHI-4B5D67.svg)](https://doi.org/10.1145/3544548.3580924)

#### Magnetic
- **[IMWUT'24]** *MagDesk: Interactive Tabletop Workspace Based on Passive Magnetic Tracking*
  [![Paper](https://img.shields.io/badge/Paper-IMWUT-4B5D67.svg)](https://doi.org/10.1145/3699756)
- **[MobiCom'23]** *Magnetic Backscatter for In-body Communication and Localization*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)](https://doi.org/10.1145/3570361.3613301)
- **[MobiCom'22]** *Automatic calibration of magnetic tracking*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)](https://doi.org/10.1145/3495243.3567653)
- **[MobiCom'24]** *Polaris: Accurate, Vision-free Fiducials for Mobile Robots with Magnetic Constellation*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)](https://doi.org/10.1145/3636534.3690711)
- **[IMWUT'24]** *MagDot: Drift-free, wearable joint angle tracking at low cost*
  [![Paper](https://img.shields.io/badge/Paper-IMWUT-4B5D67.svg)]()

#### Inertial
- **[IMWUT'23]** *SparseIMU: Computational Design of Sparse IMU Layouts for Sensing Fine-grained Finger Microgestures*
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1145/3569894)
- **[UIST'23]** *SmartPoser: Arm Pose Estimation with a Smartphone and Smartwatch Using UWB and IMU Data*
  [![Paper](https://img.shields.io/badge/Paper-UIST-4B5D67.svg)](https://doi.org/10.1145/3586183.3606821)
- **[IMWUT'23]** *Optimization-Free Test-Time Adaptation for Cross-Person Activity Recognition*
  [![Paper](https://img.shields.io/badge/Paper-IMWUT-4B5D67.svg)](https://doi.org/10.1145/3631450)
- **[IMWUT'24]** *SF-Adapter: Computational-efficient source-free domain adaptation for human activity recognition*
  [![Paper](https://img.shields.io/badge/Paper-IMWUT-4B5D67.svg)]()

<a id="physics-informed-perception"></a>

### Physics-Informed Perception

#### Signal Propagation Modeling
- **[MobiCom'20]** *Voice localization using nearby wall reflections*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)](https://doi.org/10.1145/3372224.3380884)
- **[MobiCom'21]** *Millimetro: mmWave retro-reflective tags for accurate, long range localization*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)]()
- **[MobiSys'23]** *Hawkeye: Hectometer-range Subcentimeter Localization for Large-scale mmWave Backscatter*
  [![Paper](https://img.shields.io/badge/Paper-MobiSys-4B5D67.svg)](https://doi.org/10.1145/3581791.3596869)
- **[MobiSys'24]** *Enabling 6D Pose Tracking on Your Acoustic Devices*
  [![Paper](https://img.shields.io/badge/Paper-MobiSys-4B5D67.svg)](https://doi.org/10.1145/3643832.3661875)
- **[SenSys'24]** *Locating Your Smart Devices with a Single Speaker*
  [![Paper](https://img.shields.io/badge/Paper-SenSys-4B5D67.svg)](https://doi.org/10.1145/3666025.3699320)
- **[MobiCom'25]** *Scalable and Low Power Localization for Underwater Robots*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)](https://doi.org/10.1145/3680207.3765265)

#### Phase and Frequency Dynamics Modeling
- **[MobiCom'20]** *mmVib: micrometer-level vibration measurement with mmwave radar*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)]()
- **[IMWUT'22]** *Enabling Contact-free Acoustic Sensing under Device Motion*
  [![Paper](https://img.shields.io/badge/Paper-IMWUT-4B5D67.svg)](https://doi.org/10.1145/3550329)
- **[IPSN'23]** *Addressing Practical Challenges in Acoustic Sensing To Enable Fast Motion Tracking*
  [![Paper](https://img.shields.io/badge/Paper-IPSN-4B5D67.svg)](https://doi.org/10.1145/3583120.3586954)
- **[IPSN'23]** *Platypus: Sub-mm Micro-Displacement Sensing with Passive Millimeter-wave Tags As "Phase Carriers"*
  [![Paper](https://img.shields.io/badge/Paper-IPSN-4B5D67.svg)](https://doi.org/10.1145/3583120.3586965)
- **[MobiSys'23]** *DF-Sense: Multi-user Acoustic Sensing for Heartbeat Monitoring with Dualforming*
  [![Paper](https://img.shields.io/badge/Paper-MobiSys-4B5D67.svg)](https://doi.org/10.1145/3581791.3596867)

#### Physical Interaction and Transduction Modeling
- **[NSDI'21]** *WiForce: Wireless Sensing and Localization of Contact Forces on a Space Continuum*
  [![Paper](https://img.shields.io/badge/Paper-NSDI-4B5D67.svg)](https://www.usenix.org/conference/nsdi21/presentation/gupta)
- **[MobiCom'23]** *AgriTera: Accurate Non-Invasive Fruit Ripeness Sensing via Sub-Terahertz Wireless Signals*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)](https://doi.org/10.1145/3570361.3613275)
- **[MobiCom'24]** *Fine-grained Textile Moisture Sensing with Commodity UWB*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)](https://doi.org/10.1145/3636534.3690679)
- **[MobiCom'24]** *Around the Corner mmWave Imaging in Practical Environments*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)](https://doi.org/10.1145/3636534.3690671)
- **[MobiSys'25]** *Non-Line-of-Sight 3D Object Reconstruction via mmWave Surface Normal Estimation*
  [![Paper](https://img.shields.io/badge/Paper-MobiSys-4B5D67.svg)](https://doi.org/10.1145/3711875.3729138)

<a id="data-driven-perception"></a>

### Data-Driven Perception

#### Task-Specific Discriminative Perception
- **[IMWUT'20]** *DeepRange: Acoustic ranging via deep learning*
  [![Paper](https://img.shields.io/badge/Paper-IMWUT-4B5D67.svg)]()
- **[MobiCom'20]** *Towards 3D human pose construction using wifi*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)](https://doi.org/10.1145/3372224.3380900)
- **[SenSys'22]** *SiFall: Practical online fall detection with RF sensing*
  [![Paper](https://img.shields.io/badge/Paper-SenSys-4B5D67.svg)]()
- **[MobiSys'23]** *mm3DFace: Nonintrusive 3D Facial Reconstruction Leveraging mmWave Signals*
  [![Paper](https://img.shields.io/badge/Paper-MobiSys-4B5D67.svg)](https://doi.org/10.1145/3581791.3596839)
- **[SenSys'23]** *Egocentric Human Pose Estimation using Head-mounted mmWave Radar*
  [![Paper](https://img.shields.io/badge/Paper-SenSys-4B5D67.svg)](https://doi.org/10.1145/3625687.3625799)
- **[SenSys'25]** *Improving mmWave based Hand Hygiene Monitoring through Beam Steering and Combining Techniques*
  [![Paper](https://img.shields.io/badge/Paper-SenSys-4B5D67.svg)](https://doi.org/10.1145/3715014.3722085)
- **[SenSys'25]** *RAM-Hand: Robust Acoustic Multi-Hand Pose Reconstruction Using a Microphone Array*
  [![Paper](https://img.shields.io/badge/Paper-SenSys-4B5D67.svg)](https://doi.org/10.1145/3715014.3722055)

#### Data-Efficient Perception
- **[SenSys'20]** *RF-net: A unified meta-learning framework for RF-enabled one-shot human activity recognition*
  [![Paper](https://img.shields.io/badge/Paper-SenSys-4B5D67.svg)]()
- **[SenSys'21]** *OneFi: One-shot recognition for unseen gesture via cots wifi*
  [![Paper](https://img.shields.io/badge/Paper-SenSys-4B5D67.svg)]()
- **[MobiCom'22]** *Cosmo: contrastive fusion learning with small data for multimodal human activity recognition*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)]()
- **[SenSys'23]** *Construct 3D Hand Skeleton with Commercial WiFi*
  [![Paper](https://img.shields.io/badge/Paper-SenSys-4B5D67.svg)](https://doi.org/10.1145/3625687.3625812)
- **[MobiCom'24]** *ADMarker: A Multi-Modal Federated Learning System for Monitoring Digital Biomarkers of Alzheimer's Disease*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)](https://doi.org/10.1145/3636534.3649370)
- **[SenSys'24]** *BSENSE: In-vehicle Child Detection and Vital Sign Monitoring with a Single mmWave Radar and Synthetic Reflectors*
  [![Paper](https://img.shields.io/badge/Paper-SenSys-4B5D67.svg)](https://doi.org/10.1145/3666025.3699352)
- **[SenSys'25]** *mmET: mmWave Radar-Based Eye Tracking on Smart Glasses*
  [![Paper](https://img.shields.io/badge/Paper-SenSys-4B5D67.svg)](https://doi.org/10.1145/3715014.3722050)

<a id="generative-perception"></a>

### Generative Perception

#### Semantic World Understanding
- **[ACL'24]** *Penetrative AI: Making LLMs Comprehend the Physical World*
  [![Paper](https://img.shields.io/badge/Paper-ACL-4B5D67.svg)](https://doi.org/10.18653/v1/2024.findings-acl.437)
- **[HotMobile'25]** *ContextLLM: Meaningful Context Reasoning from Multi-Sensor and Multi-Device Data Using LLMs*
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1145/3708468.3711892)
- **[arXiv'24.06]** *LLaSA: A Sensor-Aware LLM for Natural Language Reasoning of Human Activity from IMU Data*
  [![arXiv](https://img.shields.io/badge/arXiv-2406.14498-b31b1b.svg)](https://arxiv.org/abs/2406.14498)
- **[MobiSys'25]** *High-resolution mmWave Imaging using Metasurface and Diffusion*
  [![Paper](https://img.shields.io/badge/Paper-MobiSys-4B5D67.svg)](https://doi.org/10.1145/3711875.3729162)
- **[CVPR'24]** *DiffusionPoser: Real-Time Human Motion Reconstruction From Arbitrary Sparse Sensors Using Autoregressive Diffusion*
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)](https://doi.org/10.1109/cvpr52733.2024.00243)
- **[ECCV'24]** *Diffusion model is a good pose estimator from 3D RF-Vision*
  [![Paper](https://img.shields.io/badge/Paper-ECCV-4B5D67.svg)]()

#### Sensor-grounded Reasoning
- **[FMSys'24]** *HARGPT: Are LLMs Zero-Shot Human Activity Recognizers?*
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1109/fmsys62467.2024.00011)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/aiot-lab/HARGPT)
- **[arXiv'24.03]** *LLMSense: Harnessing LLMs for High-level Reasoning Over Spatiotemporal Sensor Traces*
  [![arXiv](https://img.shields.io/badge/arXiv-2403.19857-b31b1b.svg)](https://arxiv.org/abs/2403.19857)
- **[ACL'25]** *RAVEN: Query-Guided Representation Alignment for Question Answering over Audio, Video, Embedded Sensors, and Natural Language*
  [![Paper](https://img.shields.io/badge/Paper-ACL-4B5D67.svg)](https://doi.org/10.18653/v1/2025.emnlp-main.96)
- **[IMWUT'25]** *SensorChat: Answering Qualitative and Quantitative Questions during Long-term Multimodal Sensor Interactions*
  [![Paper](https://img.shields.io/badge/Paper-IMWUT-4B5D67.svg)](https://doi.org/10.1145/3749496)
- **[Patterns'26]** *IoT-LLM: A framework for enhancing large language model reasoning from real-world sensor data*
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1016/j.patter.2025.101429)

#### Sensor Data Synthesis
- **[IMWUT'24]** *IMUGPT 2.0: Language-Based Cross Modality Transfer for Sensor-Based Human Activity Recognition*
  [![Paper](https://img.shields.io/badge/Paper-IMWUT-4B5D67.svg)](https://doi.org/10.1145/3678545)
- **[MobiCom'24]** *RF-Diffusion: Radio Signal Generation via Time-Frequency Diffusion*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)](https://doi.org/10.1145/3636534.3649348)
- **[SenSys'23]** *RF Genesis: Zero-Shot Generalization of mmWave Sensing through Simulation-Based Data Synthesis and Generative Diffusion Models*
  [![Paper](https://img.shields.io/badge/Paper-SenSys-4B5D67.svg)](https://doi.org/10.1145/3625687.3625798)
- **[IEEE Access'23]** *Synthetic ECG Signal Generation Using Probabilistic Diffusion Models*
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1109/access.2023.3296542)
- **[ICASSP'25]** *RF Distillation Diffusion Model: An Efficient RFF Data Augmentation Method*
  [![Paper](https://img.shields.io/badge/Paper-ICASSP-4B5D67.svg)](https://doi.org/10.1109/icassp49660.2025.10889299)

<a id="sensor-fusion-and-multimodal-perception"></a>

### Sensor Fusion and Multimodal Perception

#### Architectural Fusion Strategies
- **[CVPR'18]** *PointFusion: Deep Sensor Fusion for 3D Bounding Box Estimation*
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)]()
- **[CVPR'20]** *PointPainting: Sequential Fusion for 3D Object Detection*
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)]()
- **[NeurIPS'21]** *Multimodal Virtual Point 3D Detection*
  [![Paper](https://img.shields.io/badge/Paper-NeurIPS-4B5D67.svg)]()
- **[CVPR'22]** *DeepFusion: LiDAR-Camera Deep Fusion for Multi-Modal 3D Object Detection*
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)]()
- **[WACV'21]** *CenterFusion: Center-Based Radar and Camera Fusion for 3D Object Detection*
  [![Paper](https://img.shields.io/badge/Paper-WACV-4B5D67.svg)]()
- **[CVPR'21]** *PointAugmenting: Cross-Modal Augmentation for 3D Object Detection*
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)]()
- **[IROS'18]** *Joint 3D Proposal Generation and Object Detection from View Aggregation*
  [![Paper](https://img.shields.io/badge/Paper-IROS-4B5D67.svg)]()
- **[CVPR'22]** *TransFusion: Robust LiDAR-Camera Fusion for 3D Object Detection with Transformers*
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)]()
- **[ICRA'19]** *MVX-Net: Multimodal VoxelNet for 3D Object Detection*
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)]()
- **[ECCV'18]** *Deep Continuous Fusion for Multi-Sensor 3D Object Detection*
  [![Paper](https://img.shields.io/badge/Paper-ECCV-4B5D67.svg)]()
- **[CVPR'17]** *Multi-View 3D Object Detection Network for Autonomous Driving*
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)]()
- **[CVPR'18]** *Frustum PointNets for 3D Object Detection from RGB-D Data*
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)]()
- **[IROS'19]** *Frustum ConvNet: Sliding frustums to aggregate local point-wise features for amodal 3D object detection*
  [![Paper](https://img.shields.io/badge/Paper-IROS-4B5D67.svg)]()

#### Cross-Modal Association and Robustness
- **[IPSN'22]** *Vi-Fi: Associating Moving Subjects across Vision and Wireless Sensors*
  [![Paper](https://img.shields.io/badge/Paper-IPSN-4B5D67.svg)](https://doi.org/10.1109/ipsn54338.2022.00024)
- **[IPSN'23]** *CMA: Cross-Modal Association Between Wearable and Structural Vibration Signal Segments for Indoor Occupant Sensing*
  [![Paper](https://img.shields.io/badge/Paper-IPSN-4B5D67.svg)](https://doi.org/10.1145/3583120.3586960)
- **[SenSys'24]** *Mission: mmWave Radar Person Identification with RGB Cameras*
  [![Paper](https://img.shields.io/badge/Paper-SenSys-4B5D67.svg)](https://doi.org/10.1145/3666025.3699340)
- **[MobiSys'21]** *Low-latency speculative inference on distributed multi-modal data streams*
  [![Paper](https://img.shields.io/badge/Paper-MobiSys-4B5D67.svg)](https://doi.org/10.1145/3458864.3467884)
- **[SenSys'23]** *XGait: Cross-Modal Translation via Deep Generative Sensing for RF-based Gait Recognition*
  [![Paper](https://img.shields.io/badge/Paper-SenSys-4B5D67.svg)](https://doi.org/10.1145/3625687.3625792)
- **[SenSys'25]** *Proteus: Enhanced mmWave Leaf Wetness Detection with Cross-Modality Knowledge Transfer*
  [![Paper](https://img.shields.io/badge/Paper-SenSys-4B5D67.svg)](https://doi.org/10.1145/3715014.3722052)
- **[IPSN'22]** *VMA: Domain Variance- and Modality-Aware Model Transfer for Fine-Grained Occupant Activity Recognition*
  [![Paper](https://img.shields.io/badge/Paper-IPSN-4B5D67.svg)](https://doi.org/10.1109/ipsn54338.2022.00028)
- **[MobiCom'21]** *RFID and camera fusion for recognition of human-object interactions*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)](https://doi.org/10.1145/3447993.3483244)

#### Spatiotemporal, Collaborative, and Foundation-Model Fusion
- **[ECCV'20]** *V2VNet: Vehicle-to-Vehicle Communication for Joint Perception and Prediction*
  [![Paper](https://img.shields.io/badge/Paper-ECCV-4B5D67.svg)]()
- **[CoRL'22]** *CoBEVT: Cooperative Bird's Eye View Semantic Segmentation with Sparse Transformers*
  [![Paper](https://img.shields.io/badge/Paper-CoRL-4B5D67.svg)]()
- **[ICCV'23]** *HM-ViT: Hetero-Modal Vehicle-to-Vehicle Cooperative Perception with Vision Transformer*
  [![Paper](https://img.shields.io/badge/Paper-ICCV-4B5D67.svg)]()
- **[CVPR'20]** *When2com: Multi-Agent Perception via Communication Graph Grouping*
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)]()
- **[ICRA'20]** *Who2com: Collaborative Perception via Learnable Handshake Communication*
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)]()
- **[ECCV'22]** *BEVFormer: Learning Bird's-Eye-View Representation from Multi-Camera Images via Spatiotemporal Transformers*
  [![arXiv](https://img.shields.io/badge/arXiv-2203.17270-b31b1b.svg)](https://arxiv.org/abs/2203.17270)
- **[ICCV'23]** *Exploring Object-Centric Temporal Modeling for Efficient Multi-View 3D Object Detection*
  [![Paper](https://img.shields.io/badge/Paper-ICCV-4B5D67.svg)]()
- **[arXiv'23.11]** *Sparse4D v3: Advancing End-to-End 3D Detection and Tracking*
  [![arXiv](https://img.shields.io/badge/arXiv-2311.11722-b31b1b.svg)](https://arxiv.org/abs/2311.11722)
- **[arXiv'22.12]** *Planning-oriented Autonomous Driving*
  [![arXiv](https://img.shields.io/badge/arXiv-2212.10156-b31b1b.svg)](https://arxiv.org/abs/2212.10156)
- **[arXiv'23.08]** *FusionAD: Multi-Modality Fusion for Prediction and Planning Tasks of Autonomous Driving*
  [![arXiv](https://img.shields.io/badge/arXiv-2308.01006-b31b1b.svg)](https://arxiv.org/abs/2308.01006)
- **[CVPR'24]** *RCBEVDet: Radar-Camera Fusion in Bird's Eye View for 3D Object Detection*
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)]()
- **[arXiv'23.12]** *DriveLM: Driving with Graph Visual Question Answering*
  [![arXiv](https://img.shields.io/badge/arXiv-2312.14150-b31b1b.svg)](https://arxiv.org/abs/2312.14150)
- **[AAAI'25]** *LiDAR-LLM: Exploring the Potential of Large Language Models for 3D LiDAR Understanding*
  [![Paper](https://img.shields.io/badge/Paper-AAAI-4B5D67.svg)]()
- **[ICLR'25]** *X-Fi: A Modality-Invariant Foundation Model for Multimodal Human Sensing*
  [![Paper](https://img.shields.io/badge/Paper-ICLR-4B5D67.svg)]()
- **[NeurIPS'23]** *MM-Fi: Multi-Modal Non-Intrusive 4D Human Dataset for Versatile Wireless Sensing*
  [![Paper](https://img.shields.io/badge/Paper-NeurIPS-4B5D67.svg)](https://doi.org/10.52202/075280-0822)
- **[Patterns'23]** *SenseFi: A library and benchmark on deep-learning-empowered WiFi human sensing*
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1016/j.patter.2023.100703)

<a id="perception-tasks"></a>

### Perception Tasks

#### Object Perception
- **[arXiv'25.10]** *Towards 3D Objectness Learning in an Open World*
  [![arXiv](https://img.shields.io/badge/arXiv-2510.17686-b31b1b.svg)](https://arxiv.org/abs/2510.17686)
- **[CVPR'22]** *Multimodal Material Segmentation*
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)](https://doi.org/10.1109/cvpr52688.2022.01918)
- **[MobiCom'21]** *RFID and camera fusion for recognition of human-object interactions*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)](https://doi.org/10.1145/3447993.3483244)
- **[MobiCom'23]** *MobiSpectral: Hyperspectral Imaging on Mobile Devices*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)](https://doi.org/10.1145/3570361.3613296)
- **[ICML'21]** *Learning Transferable Visual Models From Natural Language Supervision (CLIP)*
  [![Paper](https://img.shields.io/badge/Paper-ICML-4B5D67.svg)](https://proceedings.mlr.press/v139/radford21a.html)
- **[MobiSys'23]** *Contactless Material Identification with Millimeter Wave Vibrometry*
  [![Paper](https://img.shields.io/badge/Paper-MobiSys-4B5D67.svg)](https://doi.org/10.1145/3581791.3596850)
- **[ICLR'26]** *RF-MatID: Dataset and Benchmark for Radio Frequency Material Identification*
  [![Paper](https://img.shields.io/badge/Paper-ICLR-4B5D67.svg)]()
- **[Paper'21]** *milliEye: A Lightweight mmWave Radar and Camera Fusion System for Robust Object Detection*
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)]()
- **[SenSys'21]** *RFusion: Robotic Grasping via RF-Visual Sensing and Learning*
  [![Paper](https://img.shields.io/badge/Paper-SenSys-4B5D67.svg)]()

#### Scene Perception
- **[Entropy'23]** *A Survey on Deep Learning Based Segmentation, Detection and Classification for 3D Point Clouds*
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.3390/e25040635)
- **[CACM'22]** *NeRF: Representing Scenes as Neural Radiance Fields for View Synthesis*
  [![Paper](https://img.shields.io/badge/Paper-CACM-4B5D67.svg)]()
- **[SIGGRAPH'23]** *3D Gaussian Splatting for Real-Time Radiance Field Rendering*
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1145/3592433)
- **[arXiv'24.04]** *PhyScene: Physically Interactable 3D Scene Synthesis for Embodied AI*
  [![arXiv](https://img.shields.io/badge/arXiv-2404.09465-b31b1b.svg)](https://arxiv.org/abs/2404.09465)
- **[ECCV'24]** *OccWorld: Learning a 3D Occupancy World Model for Autonomous Driving*
  [![arXiv](https://img.shields.io/badge/arXiv-2311.16038-b31b1b.svg)](https://arxiv.org/abs/2311.16038)
- **[CVPR'20]** *REVERIE: Remote Embodied Visual Referring Expression in Real Indoor Environments*
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)](https://doi.org/10.1109/cvpr42600.2020.01000)
- **[MobiCom'24]** *Enabling Visual Recognition at Radio Frequency*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)](https://doi.org/10.1145/3636534.3649369)
- **[MobiCom'22]** *VIPS: Real-Time Perception Fusion for Infrastructure-Assisted Autonomous Driving*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)]()
- **[SenSys'24]** *Boosting Collaborative Vehicular Perception on the Edge with Vehicle-to-Vehicle Communication*
  [![Paper](https://img.shields.io/badge/Paper-SenSys-4B5D67.svg)](https://doi.org/10.1145/3666025.3699328)
- **[arXiv'24.09]** *Generative AI-Enhanced Multi-Modal Semantic Communication in Internet of Vehicles*
  [![arXiv](https://img.shields.io/badge/arXiv-2409.15642-b31b1b.svg)](https://arxiv.org/abs/2409.15642)

#### Human Perception
- **[CVPR'25]** *DynPose: Largely Improving the Efficiency of Human Pose Estimation by a Simple Dynamic Framework*
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)](https://doi.org/10.1109/cvpr52734.2025.00116)
- **[CVPR'23]** *SVFormer: Semi-supervised Video Transformer for Action Recognition*
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)](https://doi.org/10.1109/cvpr52729.2023.01804)
- **[MobiCom'22]** *MobiDepth: Real-Time Depth Estimation Using On-Device Dual Cameras*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)]()
- **[MobiCom'21]** *RFID and camera fusion for recognition of human-object interactions*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)](https://doi.org/10.1145/3447993.3483244)
- **[MobiCom'23]** *AccessWear: Making Smartphone Applications Accessible to Blind Users*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)](https://doi.org/10.1145/3570361.3592495)
- **[SenSys'24]** *BSENSE: In-vehicle Child Detection and Vital Sign Monitoring with a Single mmWave Radar and Synthetic Reflectors*
  [![Paper](https://img.shields.io/badge/Paper-SenSys-4B5D67.svg)](https://doi.org/10.1145/3666025.3699352)
- **[MobiCom'23]** *SignQuery: A Natural User Interface and Search Engine for Sign Languages with Wearable Sensors*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)](https://doi.org/10.1145/3570361.3613286)
- **[MobiCom'23]** *Sign-to-911: Emergency Call Service for Sign Language Users with Assistive AR Glasses*
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)](https://doi.org/10.1145/3570361.3613260)
- **[FMSys'24]** *HARGPT: Are LLMs Zero-Shot Human Activity Recognizers?*
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1109/fmsys62467.2024.00011)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/aiot-lab/HARGPT)
- **[HotMobile'25]** *ContextLLM: Meaningful Context Reasoning from Multi-Sensor and Multi-Device Data Using LLMs*
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1145/3708468.3711892)
- **[arXiv'24.06]** *LLaSA: A Sensor-Aware LLM for Natural Language Reasoning of Human Activity from IMU Data*
  [![arXiv](https://img.shields.io/badge/arXiv-2406.14498-b31b1b.svg)](https://arxiv.org/abs/2406.14498)
- **[ACL'25]** *ProMind-LLM: Proactive Mental Health Care via Causal Reasoning with Sensor Data*
  [![Paper](https://img.shields.io/badge/Paper-ACL-4B5D67.svg)](https://doi.org/10.18653/v1/2025.findings-acl.1033)
- **[ACL'25]** *MEIT: Multimodal Electrocardiogram Instruction Tuning on Large Language Models for Report Generation*
  [![Paper](https://img.shields.io/badge/Paper-ACL-4B5D67.svg)](https://doi.org/10.18653/v1/2025.findings-acl.749)

---

## 2. Physical Cognition

#### Surveys and Position Papers

- **[arXiv'25.01]** *Physical AI Agents: Integrating Cognitive Intelligence with Real-World Action*
  [![arXiv](https://img.shields.io/badge/arXiv-2501.08944-b31b1b.svg)](https://arxiv.org/abs/2501.08944)
- **[arXiv'25.10]** *Aligning Perception, Reasoning, Modeling and Interaction: A Survey on Physical AI*
  [![arXiv](https://img.shields.io/badge/arXiv-2510.04978-b31b1b.svg)](https://arxiv.org/abs/2510.04978)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/AI4Phys/Awesome-AI-for-Physics)
- **[arXiv'25.07]** *A Survey: Learning Embodied Intelligence from Physical Simulators and World Models*
  [![arXiv](https://img.shields.io/badge/arXiv-2507.00917-b31b1b.svg)](https://arxiv.org/abs/2507.00917)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/NJU3DV-LoongGroup/Embodied-World-Models-Survey)
- **[arXiv'25.03]** *World Models in Artificial Intelligence: Sensing, Learning, and Reasoning Like a Child*
  [![arXiv](https://img.shields.io/badge/arXiv-2503.15168-b31b1b.svg)](https://arxiv.org/abs/2503.15168)

<a id="state-representation-and-abstraction"></a>

### State Representation and Abstraction

#### State Abstraction
- **[ICML'19]** *Learning Latent Dynamics for Planning from Pixels (PlaNet)*
  [![Paper](https://img.shields.io/badge/Paper-ICML-4B5D67.svg)](https://proceedings.mlr.press/v97/hafner19a.html)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/google-research/planet)
  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://planetrl.github.io/)
- **[ICLR'20]** *Dream to Control: Learning Behaviors by Latent Imagination (Dreamer)*
  [![Paper](https://img.shields.io/badge/Paper-ICLR-4B5D67.svg)](https://openreview.net/forum?id=S1lOTC4tDS)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/google-research/dreamer)
- **[ICML'20]** *CURL: Contrastive Unsupervised Representations for Reinforcement Learning*
  [![Paper](https://img.shields.io/badge/Paper-ICML-4B5D67.svg)](https://proceedings.mlr.press/v119/laskin20a.html)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/MishaLaskin/curl)
- **[ICML'21]** *Learning Transferable Visual Models From Natural Language Supervision (CLIP)*
  [![Paper](https://img.shields.io/badge/Paper-ICML-4B5D67.svg)](https://proceedings.mlr.press/v139/radford21a.html)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/openai/CLIP)
- **[CVPR'23]** *Self-Supervised Learning from Images with a Joint-Embedding Predictive Architecture (I-JEPA)*
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)](https://doi.org/10.1109/cvpr52729.2023.01499)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/facebookresearch/ijepa)
- **[CVPR'20]** *VectorNet: Encoding HD Maps and Agent Dynamics From Vectorized Representation*
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)](https://doi.org/10.1109/cvpr42600.2020.01154)
- **[CVPR'21]** *MP3: A Unified Model to Map, Perceive, Predict and Plan*
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)](https://doi.org/10.1109/cvpr46437.2021.01417)
  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://sergiocasas.github.io/publication/mp3/)
- **[arXiv'23.07]** *VoxPoser: Composable 3D Value Maps for Robotic Manipulation with Language Models*
  [![arXiv](https://img.shields.io/badge/arXiv-2307.05973-b31b1b.svg)](https://arxiv.org/abs/2307.05973)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/huangwl18/VoxPoser)
  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://voxposer.github.io/)

#### Structured World Representations
- **[ECCV'22]** *BEVFormer: Learning Bird's-Eye-View Representation from Multi-Camera Images via Spatiotemporal Transformers*
  [![arXiv](https://img.shields.io/badge/arXiv-2203.17270-b31b1b.svg)](https://arxiv.org/abs/2203.17270)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/fundamentalvision/BEVFormer)
- **[CVPR'23]** *Implicit Occupancy Flow Fields for Perception and Prediction in Self-Driving*
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)](https://doi.org/10.1109/CVPR52729.2023.00139)
  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://waabi.ai/research/implicito)
- **[ECCV'24]** *OccWorld: Learning a 3D Occupancy World Model for Autonomous Driving*
  [![Paper](https://img.shields.io/badge/Paper-ECCV-4B5D67.svg)](https://doi.org/10.1007/978-3-031-72624-8_4)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/wzzheng/OccWorld)
  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://wzzheng.net/OccWorld/)

<a id="world-models"></a>

### World Models

#### Foundations and Surveys
- **[ACM CSUR'26]** *Understanding World or Predicting Future? A Comprehensive Survey of World Models*
  [![Paper](https://img.shields.io/badge/Paper-ACM%20CSUR-4B5D67.svg)](https://doi.org/10.1145/3746449)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/tsinghua-fib-lab/World-Model)
- **[arXiv'18.03]** *World Models*
  [![arXiv](https://img.shields.io/badge/arXiv-1803.10122-b31b1b.svg)](https://arxiv.org/abs/1803.10122)
  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://worldmodels.github.io/)
- **[OpenReview'22]** *A Path Towards Autonomous Machine Intelligence*
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://openreview.net/forum?id=BZ5a1r-kVsf)

#### Latent Predictive World Models
- **[ICML'19]** *Learning Latent Dynamics for Planning from Pixels (PlaNet)*
  [![Paper](https://img.shields.io/badge/Paper-ICML-4B5D67.svg)](https://proceedings.mlr.press/v97/hafner19a.html)
- **[ICLR'20]** *Dream to Control: Learning Behaviors by Latent Imagination (Dreamer)*
  [![Paper](https://img.shields.io/badge/Paper-ICLR-4B5D67.svg)](https://openreview.net/forum?id=S1lOTC4tDS)
- **[CoRL'22]** *DayDreamer: World Models for Physical Robot Learning*
  [![Paper](https://img.shields.io/badge/Paper-CoRL-4B5D67.svg)](https://proceedings.mlr.press/v205/wu23c.html)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/danijar/daydreamer)
- **[CVPR'23]** *I-JEPA: Self-Supervised Learning from Images with a Joint-Embedding Predictive Architecture*
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)](https://doi.org/10.1109/cvpr52729.2023.01499)
- **[arXiv'24.04]** *V-JEPA: Revisiting Feature Prediction for Learning Visual Representations from Video*
  [![arXiv](https://img.shields.io/badge/arXiv-2404.08471-b31b1b.svg)](https://arxiv.org/abs/2404.08471)
- **[arXiv'25.06]** *V-JEPA 2: Self-Supervised Video Models Enable Understanding, Prediction and Planning*
  [![arXiv](https://img.shields.io/badge/arXiv-2506.09985-b31b1b.svg)](https://arxiv.org/abs/2506.09985)
  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://ai.meta.com/research/vjepa/)

#### Generative and Interactive World Models
- **[Tech Report'24]** *Video Generation Models as World Simulators*
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://openai.com/index/video-generation-models-as-world-simulators/)
- **[ICML'24]** *Genie: Generative Interactive Environments*
  [![Paper](https://img.shields.io/badge/Paper-ICML-4B5D67.svg)](https://proceedings.mlr.press/v235/bruce24a.html)
- **[arXiv'24.08]** *GameNGen: Diffusion Models Are Real-Time Game Engines*
  [![arXiv](https://img.shields.io/badge/arXiv-2408.14837-b31b1b.svg)](https://arxiv.org/abs/2408.14837)
  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://gamengen.github.io/)
- **[arXiv'23.09]** *GAIA-1: A Generative World Model for Autonomous Driving*
  [![arXiv](https://img.shields.io/badge/arXiv-2309.17080-b31b1b.svg)](https://arxiv.org/abs/2309.17080)
  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://anthonyhu.github.io/gaia1)
- **[arXiv'23.09]** *DriveDreamer: Towards Real-world-driven World Models for Autonomous Driving*
  [![arXiv](https://img.shields.io/badge/arXiv-2309.09777-b31b1b.svg)](https://arxiv.org/abs/2309.09777)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/JeffWang987/DriveDreamer)
- **[arXiv'25.01]** *Cosmos World Foundation Model Platform for Physical AI*
  [![arXiv](https://img.shields.io/badge/arXiv-2501.03575-b31b1b.svg)](https://arxiv.org/abs/2501.03575)
  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://www.nvidia.com/en-us/ai/cosmos/)

#### Geometric and Structured World Models
- **[ECCV'24]** *OccWorld: Learning a 3D Occupancy World Model for Autonomous Driving*
  [![Paper](https://img.shields.io/badge/Paper-ECCV-4B5D67.svg)](https://doi.org/10.1007/978-3-031-72624-8_4)
- **[AAAI'25]** *Drive-OccWorld: Vision-Centric 4D Occupancy Forecasting and Planning via World Models for Autonomous Driving*
  [![Paper](https://img.shields.io/badge/Paper-AAAI-4B5D67.svg)](https://doi.org/10.1609/aaai.v39i9.33230)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/yuyang-cloud/Drive-OccWorld)
- **[arXiv'25.05]** *Occupancy World Model for Robots (RoboOccWorld)*
  [![arXiv](https://img.shields.io/badge/arXiv-2505.05512-b31b1b.svg)](https://arxiv.org/abs/2505.05512)
- **[ICML'24]** *3D-VLA: A 3D Vision-Language-Action Generative World Model*
  [![Paper](https://img.shields.io/badge/Paper-ICML-4B5D67.svg)](https://proceedings.mlr.press/v235/zhen24a.html)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/UMass-Embodied-AGI/3D-VLA)

<a id="reasoning-and-planning"></a>

### Reasoning and Planning

#### Task Specification and Problem Formulation
- **[AI'71]** *STRIPS: A New Approach to the Application of Theorem Proving to Problem Solving*
  [![Paper](https://img.shields.io/badge/Paper-AI-4B5D67.svg)](https://doi.org/10.1016/0004-3702(71)90010-5)
- **[Book'06]** *Planning Algorithms*
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](http://planning.cs.uiuc.edu/)
- **[AI'98]** *Planning and Acting in Partially Observable Stochastic Domains*
  [![Paper](https://img.shields.io/badge/Paper-AI-4B5D67.svg)](https://doi.org/10.1016/S0004-3702(98)00023-X)
- **[CoRL'22]** *SayCan: Do As I Can, Not As I Say — Grounding Language in Robotic Affordances*
  [![Paper](https://img.shields.io/badge/Paper-CoRL-4B5D67.svg)](https://proceedings.mlr.press/v205/ichter23a.html)
  [![arXiv](https://img.shields.io/badge/arXiv-2204.01691-b31b1b.svg)](https://arxiv.org/abs/2204.01691)
  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://say-can.github.io/)
- **[arXiv'23.07]** *VoxPoser: Composable 3D Value Maps for Robotic Manipulation with Language Models*
  [![arXiv](https://img.shields.io/badge/arXiv-2307.05973-b31b1b.svg)](https://arxiv.org/abs/2307.05973)
- **[Annu. Rev. Control Robot. Auton. Syst.'21]** *Integrated Task and Motion Planning*
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1146/annurev-control-091420-084139)

#### Motion Planning — Sampling-Based
- **[Tech Report'98]** *Rapidly-Exploring Random Trees: A New Tool for Path Planning (RRT)*
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://msl.cs.uiuc.edu/~lavalle/papers/Lav98c.pdf)
- **[IJRR'11]** *Sampling-Based Algorithms for Optimal Motion Planning (RRT\*)*
  [![Paper](https://img.shields.io/badge/Paper-IJRR-4B5D67.svg)](https://doi.org/10.1177/0278364911406761)
- **[T-RA'96]** *Probabilistic Roadmaps for Path Planning in High-Dimensional Configuration Spaces (PRM)*
  [![Paper](https://img.shields.io/badge/Paper-IEEE-4B5D67.svg)](https://doi.org/10.1109/70.508439)
- **[JOSER'14]** *Reducing the Barrier to Entry of Complex Robotic Software: A MoveIt! Case Study*
  [![Paper](https://img.shields.io/badge/Paper-JOSER-4B5D67.svg)](https://doi.org/10.6092/JOSER_2014_05_01_p3)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/moveit/moveit)

#### Motion Planning — Optimization-Based
- **[ICRA'09]** *CHOMP: Gradient Optimization Techniques for Efficient Motion Planning*
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)](https://doi.org/10.1109/ROBOT.2009.5152817)
- **[IJRR'14]** *TrajOpt: Motion Planning with Sequential Convex Optimization and Convex Collision Checking*
  [![Paper](https://img.shields.io/badge/Paper-IJRR-4B5D67.svg)](https://doi.org/10.1177/0278364914528132)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/joschu/trajopt)
- **[RSS'18]** *Differentiable Physics and Stable Modes for Tool-Use and Manipulation Planning*
  [![Paper](https://img.shields.io/badge/Paper-RSS-4B5D67.svg)](https://doi.org/10.15607/rss.2018.xiv.044)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/MarcToussaint/18-RSS-PhysicalManipulation)

#### Motion Planning — Task-and-Motion Planning
- **[ICAPS'20]** *PDDLStream: Integrating Symbolic Planners and Blackbox Samplers via Optimistic Adaptive Planning*
  [![Paper](https://img.shields.io/badge/Paper-ICAPS-4B5D67.svg)](https://doi.org/10.1609/ICAPS.V30I1.6739)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/caelan/pddlstream)
- **[RSS'20]** *Deep Visual Reasoning: Learning to Predict Action Sequences for Task and Motion Planning from an Initial Scene Image*
  [![Paper](https://img.shields.io/badge/Paper-RSS-4B5D67.svg)](https://doi.org/10.15607/rss.2020.xvi.003)
- **[CoRL'22]** *Inner Monologue: Embodied Reasoning through Planning with Language Models*
  [![Paper](https://img.shields.io/badge/Paper-CoRL-4B5D67.svg)](https://proceedings.mlr.press/v205/huang23c.html)
  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://innermonologue.github.io/)
- **[IJRR'25]** *LLM-GROP: Visually Grounded Robot Task and Motion Planning with Large Language Models*
  [![Paper](https://img.shields.io/badge/Paper-IJRR-4B5D67.svg)](https://doi.org/10.1177/02783649251378196)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/bu-air-lab/llm-grop)
- **[arXiv'25.10]** *Manual2Skill++: Connector-Aware General Robotic Assembly from Instruction Manuals via Vision-Language Models*
  [![arXiv](https://img.shields.io/badge/arXiv-2510.16344-b31b1b.svg)](https://arxiv.org/abs/2510.16344)

#### Motion Planning — Learning-Based
- **[ICRA'19]** *Motion Planning Networks*
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)](https://doi.org/10.1109/ICRA.2019.8793889)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/ahq1993/MPNet)
- **[ICML'22]** *Diffuser: Planning with Diffusion for Flexible Behavior Synthesis*
  [![Paper](https://img.shields.io/badge/Paper-ICML-4B5D67.svg)](https://proceedings.mlr.press/v162/janner22a.html)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/jannerm/diffuser)
- **[ICRA'21]** *RelMoGen: Leveraging Motion Generation in Reinforcement Learning for Mobile Manipulation*
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)](https://ieeexplore.ieee.org/document/9561234)
- **[ICRA'25]** *PRESTO: Fast Motion Planning Using Diffusion Models Based on Key-Configuration Environment Representation*
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)](https://doi.org/10.1109/ICRA55743.2025.11128590)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/kiwi-sherbet/PRESTO)
- **[arXiv'25.11]** *RRT\*former: Environment-Aware Sampling-Based Motion Planning using Transformer*
  [![arXiv](https://img.shields.io/badge/arXiv-2511.15414-b31b1b.svg)](https://arxiv.org/abs/2511.15414)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/fengmingyang666/RRTformer)
- **[arXiv'25.04]** *SafeFlow: Safe Robot Motion Planning with Flow Matching via Control Barrier Functions*
  [![arXiv](https://img.shields.io/badge/arXiv-2504.08661-b31b1b.svg)](https://arxiv.org/abs/2504.08661)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/SafeFlowMatching/SafeFlow)
- **[CoRL'25]** *ManiFlow: A General Robot Manipulation Policy via Consistency Flow Training*
  [![Paper](https://img.shields.io/badge/Paper-CoRL-4B5D67.svg)](https://openreview.net/forum?id=a6I9P5V6u7)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/geyan21/ManiFlow_Policy)
- **[arXiv'25.03]** *FRMD: Fast Robot Motion Diffusion with Consistency-Distilled Movement Primitives*
  [![arXiv](https://img.shields.io/badge/arXiv-2503.02048-b31b1b.svg)](https://arxiv.org/abs/2503.02048)

#### Vision-Language-Action and Action Representations
- **[NeurIPS'24]** *RoboMamba: Efficient Vision-Language-Action Model for Robotic Reasoning and Manipulation*
  [![arXiv](https://img.shields.io/badge/arXiv-2406.04339-b31b1b.svg)](https://arxiv.org/abs/2406.04339)
- **[NeurIPS'24]** *BricksRL: A Platform for Democratizing Robotics and Reinforcement Learning Research and Education with LEGO*
  [![arXiv](https://img.shields.io/badge/arXiv-2406.17490-b31b1b.svg)](https://arxiv.org/abs/2406.17490)
- **[CoRL'23]** *RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control*
  [![Paper](https://img.shields.io/badge/Paper-CoRL-4B5D67.svg)](https://proceedings.mlr.press/v229/zitkovich23a.html)
  [![arXiv](https://img.shields.io/badge/arXiv-2307.15818-b31b1b.svg)](https://arxiv.org/abs/2307.15818)
- **[CoRL'24]** *OpenVLA: An Open-Source Vision-Language-Action Model*
  [![Paper](https://img.shields.io/badge/Paper-CoRL-4B5D67.svg)](https://openreview.net/forum?id=ZMnD6QZAE6)
  [![arXiv](https://img.shields.io/badge/arXiv-2406.09246-b31b1b.svg)](https://arxiv.org/abs/2406.09246)
- **[Blog'24]** *MiniVLA: A Better VLA with a Smaller Footprint*
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://ai.stanford.edu/blog/minivla/)
- **[arXiv'24.10]** *π₀: A Vision-Language-Action Flow Model for General Robot Control*
  [![arXiv](https://img.shields.io/badge/arXiv-2410.24164-b31b1b.svg)](https://arxiv.org/abs/2410.24164)
- **[arXiv'25.04]** *π₀.₅: A Vision-Language-Action Model with Open-World Generalization*
  [![arXiv](https://img.shields.io/badge/arXiv-2504.16054-b31b1b.svg)](https://arxiv.org/abs/2504.16054)
- **[arXiv'25.11]** *π\*₀.₆: a VLA That Learns From Experience*
  [![arXiv](https://img.shields.io/badge/arXiv-2511.14759-b31b1b.svg)](https://arxiv.org/abs/2511.14759)
- **[arXiv'25.03]** *GR00T N1: An Open Foundation Model for Generalist Humanoid Robots*
  [![arXiv](https://img.shields.io/badge/arXiv-2503.14734-b31b1b.svg)](https://arxiv.org/abs/2503.14734)
- **[arXiv'25.11]** *Alpamayo-R1: Bridging Reasoning and Action Prediction for Generalizable Autonomous Driving in the Long Tail*
  [![arXiv](https://img.shields.io/badge/arXiv-2511.00088-b31b1b.svg)](https://arxiv.org/abs/2511.00088)
- **[RSS'23]** *Diffusion Policy: Visuomotor Policy Learning via Action Diffusion*
  [![Paper](https://img.shields.io/badge/Paper-RSS-4B5D67.svg)](https://doi.org/10.15607/rss.2023.xix.026)
- **[RSS'23]** *Learning Fine-Grained Bimanual Manipulation with Low-Cost Hardware (ACT)*
  [![Paper](https://img.shields.io/badge/Paper-RSS-4B5D67.svg)](https://doi.org/10.15607/RSS.2023.XIX.016)
- **[arXiv'25.01]** *FAST: Efficient Action Tokenization for Vision-Language-Action Models*
  [![arXiv](https://img.shields.io/badge/arXiv-2501.09747-b31b1b.svg)](https://arxiv.org/abs/2501.09747)
- **[arXiv'24.05]** *A Survey on Vision-Language-Action Models for Embodied AI*
  [![arXiv](https://img.shields.io/badge/arXiv-2405.14093-b31b1b.svg)](https://arxiv.org/abs/2405.14093)

#### Computational Brain Models
- **[Science'12]** *A Large-Scale Model of the Functioning Brain*
  [![Paper](https://img.shields.io/badge/Paper-Science-4B5D67.svg)](https://doi.org/10.1126/science.1225266)
- **[Frontiers in Neurorobotics'24]** *Brain-inspired biomimetic robot control: a review*
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.3389/fnbot.2024.1395617)
- **[Eng. App. AI'23]** *Neuromorphic electronics for robotic perception, navigation and control: A survey*
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1016/j.engappai.2023.106838)
- **[Book'82]** *Vision: A Computational Investigation into the Human Representation and Processing of Visual Information*
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://mitpress.mit.edu/9780262514620/vision/)
- **[Phil. Trans. R. Soc. B'86]** *The Structure of the Nervous System of the Nematode Caenorhabditis elegans*
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1098/rstb.1986.0056)
- **[Nat. Rev. Neurosci.'06]** *The Blue Brain Project*
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1038/nrn1848)
- **[PLOS Biology'19]** *The Human Brain Project — Synergy between neuroscience, computing, informatics, and brain-inspired technologies*
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1371/journal.pbio.3000344)
- **[Nature'24]** *Neuronal wiring diagram of an adult brain*
  [![Paper](https://img.shields.io/badge/Paper-Nature-4B5D67.svg)](https://doi.org/10.1038/s41586-024-07558-y)
- **[Nature'24]** *A Drosophila Computational Brain Model Reveals Sensorimotor Processing*
  [![Paper](https://img.shields.io/badge/Paper-Nature-4B5D67.svg)](https://doi.org/10.1038/s41586-024-07763-9)
- **[Nature'24]** *Connectome-Constrained Networks Predict Neural Activity Across the Fly Visual System*
  [![Paper](https://img.shields.io/badge/Paper-Nature-4B5D67.svg)](https://doi.org/10.1038/s41586-024-07939-3)
- **[Science Robotics'23]** *Brain-Inspired Multimodal Hybrid Neural Network for Robot Place Recognition*
  [![Paper](https://img.shields.io/badge/Paper-Science%20Robotics-4B5D67.svg)](https://doi.org/10.1126/scirobotics.abm6996)

<a id="memory"></a>

### Memory

#### Memory — Surveys and Foundations
- **[arXiv'25.05]** *AI Agents vs. Agentic AI: A Conceptual Taxonomy, Applications and Challenges*
  [![arXiv](https://img.shields.io/badge/arXiv-2505.10468-b31b1b.svg)](https://arxiv.org/abs/2505.10468)
- **[TOIS'25]** *A Survey on the Memory Mechanism of Large Language Model-based Agents*
  [![Paper](https://img.shields.io/badge/Paper-TOIS-4B5D67.svg)](https://doi.org/10.1145/3748302)
- **[arXiv'25.07]** *State and Memory is All You Need for Robust and Reliable AI Agents*
  [![arXiv](https://img.shields.io/badge/arXiv-2507.00081-b31b1b.svg)](https://arxiv.org/abs/2507.00081)
- **[PLOS ONE'21]** *Embodied Working Memory During Ongoing Input Streams*
  [![Paper](https://img.shields.io/badge/Paper-PLOS%20ONE-4B5D67.svg)](https://doi.org/10.1371/journal.pone.0244822)
- **[HRI'25]** *From Interaction to Relationship: The Role of Memory, Learning, and Emotional Intelligence in AI-Embodied Human Engagement*
  [![Paper](https://img.shields.io/badge/Paper-HRI-4B5D67.svg)](https://doi.org/10.1109/hri61500.2025.10973813)
- **[arXiv'24.01]** *Memory, Space, and Planning: Multiscale Predictive Representations*
  [![arXiv](https://img.shields.io/badge/arXiv-2401.09491-b31b1b.svg)](https://arxiv.org/abs/2401.09491)
- **[Humanoids'24]** *Robots Can Multitask Too: Integrating a Memory Architecture and LLMs for Enhanced Cross-Task Robot Action Generation*
  [![Paper](https://img.shields.io/badge/Paper-Humanoids-4B5D67.svg)](https://doi.org/10.1109/humanoids58906.2024.10769803)
- **[Nat. Mach. Intell.'25]** *Embodied Large Language Models Enable Robots to Complete Complex Tasks in Unpredictable Environments*
  [![Paper](https://img.shields.io/badge/Paper-Nat.%20Mach.%20Intell.-4B5D67.svg)](https://doi.org/10.1038/s42256-025-01005-x)

#### Short-Term Memory
- **[Psych. Bull.'18]** *Benchmarks for Models of Short-Term and Working Memory*
  [![Paper](https://img.shields.io/badge/Paper-Psych.%20Bull.-4B5D67.svg)](https://doi.org/10.1037/bul0000153)
- **[Front. Comput. Neurosci.'24]** *Design and Evaluation of a Global Workspace Agent Embodied in a Realistic Multimodal Environment*
  [![Paper](https://img.shields.io/badge/Paper-Front.%20Comput.%20Neurosci.-4B5D67.svg)](https://doi.org/10.3389/fncom.2024.1352685)
- **[Cell'20]** *A Thalamic Orphan Receptor Drives Variability in Short-Term Memory*
  [![Paper](https://img.shields.io/badge/Paper-Cell-4B5D67.svg)](https://doi.org/10.1016/j.cell.2020.09.011)
- **[bioRxiv'25.05]** *Synergistic Short-Term Synaptic Plasticity Mechanisms for Working Memory*
  [![Paper](https://img.shields.io/badge/Paper-bioRxiv-b31b1b.svg)](https://doi.org/10.1101/2025.05.07.652583)
- **[PLOS Comput. Biol.'22]** *Robust and Brain-Like Working Memory Through Short-Term Synaptic Plasticity*
  [![Paper](https://img.shields.io/badge/Paper-PLOS%20Comput.%20Biol.-4B5D67.svg)](https://doi.org/10.1371/journal.pcbi.1010776)
- **[Commun. Biol.'25]** *Recurrent Neural Networks with Transient Trajectory Explain Working Memory Encoding Mechanisms*
  [![Paper](https://img.shields.io/badge/Paper-Commun.%20Biol.-4B5D67.svg)](https://doi.org/10.1038/s42003-024-07282-3)
- **[J. Neurosci.'17]** *A Spiking Working Memory Model Based on Hebbian Short-Term Potentiation*
  [![Paper](https://img.shields.io/badge/Paper-J.%20Neurosci.-4B5D67.svg)](https://doi.org/10.1523/jneurosci.1989-16.2016)
- **[Sensors'21]** *Spatial Memory in a Spiking Neural Network with Robot Embodiment*
  [![Paper](https://img.shields.io/badge/Paper-Sensors-4B5D67.svg)](https://doi.org/10.3390/s21082678)
- **[Eng. App. AI'22]** *Compound Short- and Long-Term Memory for Memory Augmented Neural Networks*
  [![Paper](https://img.shields.io/badge/Paper-Eng.%20App.%20AI-4B5D67.svg)](https://doi.org/10.1016/j.engappai.2022.105450)

#### Long-Term Memory — Foundations
- **[arXiv'24.11]** *Human-Inspired Perspectives: A Survey on AI Long-Term Memory*
  [![arXiv](https://img.shields.io/badge/arXiv-2411.00489-b31b1b.svg)](https://arxiv.org/abs/2411.00489)
- **[Neural Networks'19]** *Continual Lifelong Learning with Neural Networks: A Review*
  [![Paper](https://img.shields.io/badge/Paper-Neural%20Networks-4B5D67.svg)](https://doi.org/10.1016/j.neunet.2019.01.012)
- **[arXiv'25.04]** *Personalized Artificial General Intelligence (AGI) via Neuroscience-Inspired Continuous Learning Systems*
  [![arXiv](https://img.shields.io/badge/arXiv-2504.20109-b31b1b.svg)](https://arxiv.org/abs/2504.20109)
- **[Nat. Commun.'25]** *Hybrid Neural Networks for Continual Learning Inspired by Corticohippocampal Circuits*
  [![Paper](https://img.shields.io/badge/Paper-Nat.%20Commun.-4B5D67.svg)](https://doi.org/10.1038/s41467-025-56405-9)

#### Long-Term Memory — Episodic
- **[arXiv'20.05]** *A Proposal for Intelligent Agents with Episodic Memory*
  [![arXiv](https://img.shields.io/badge/arXiv-2005.03182-b31b1b.svg)](https://arxiv.org/abs/2005.03182)
- **[RA-L'18]** *Deep Episodic Memory: Encoding, Recalling, and Predicting Episodic Experiences for Robot Action Execution*
  [![Paper](https://img.shields.io/badge/Paper-RA--L-4B5D67.svg)](https://doi.org/10.1109/lra.2018.2860057)
- **[Nat. Commun.'21]** *Robust High-Dimensional Memory-Augmented Neural Networks*
  [![Paper](https://img.shields.io/badge/Paper-Nat.%20Commun.-4B5D67.svg)](https://doi.org/10.1038/s41467-021-22364-0)
- **[IEEE TAI'24]** *Memory-Augmented Graph Neural Networks: A Brain-Inspired Review*
  [![Paper](https://img.shields.io/badge/Paper-IEEE%20TAI-4B5D67.svg)](https://doi.org/10.1109/tai.2023.3329454)
- **[eLife'22]** *A Neural Network Model of When to Retrieve and Encode Episodic Memories*
  [![Paper](https://img.shields.io/badge/Paper-eLife-4B5D67.svg)](https://doi.org/10.7554/eLife.74445)
- **[Sci. Rep.'25]** *A Scalable Reinforcement Learning Framework Inspired by Hippocampal Memory Mechanisms for Efficient Contextual and Sequential Decision Making*
  [![Paper](https://img.shields.io/badge/Paper-Sci.%20Rep.-4B5D67.svg)](https://doi.org/10.1038/s41598-025-10586-x)
- **[arXiv'26.03]** *Chameleon: Episodic Memory for Long-Horizon Robotic Manipulation*
  [![arXiv](https://img.shields.io/badge/arXiv-2603.24576-b31b1b.svg)](https://arxiv.org/abs/2603.24576)

#### Long-Term Memory — Semantic
- **[arXiv'25.04]** *Decentralizing AI Memory: SHIMI, a Semantic Hierarchical Memory Index for Scalable Agent Reasoning*
  [![arXiv](https://img.shields.io/badge/arXiv-2504.06135-b31b1b.svg)](https://arxiv.org/abs/2504.06135)
- **[arXiv'25.07]** *Hierarchical Memory for High-Efficiency Long-Term Reasoning in LLM Agents*
  [![arXiv](https://img.shields.io/badge/arXiv-2507.22925-b31b1b.svg)](https://arxiv.org/abs/2507.22925)
- **[IJCAI'25]** *AriGraph: Learning Knowledge Graph World Models with Episodic Memory for LLM Agents*
  [![Paper](https://img.shields.io/badge/Paper-IJCAI-4B5D67.svg)](https://doi.org/10.24963/ijcai.2025/2)
- **[arXiv'25.07]** *MIRIX: Multi-Agent Memory System for LLM-Based Agents*
  [![arXiv](https://img.shields.io/badge/arXiv-2507.07957-b31b1b.svg)](https://arxiv.org/abs/2507.07957)
- **[arXiv'25.04]** *Mem0: Building Production-Ready AI Agents with Scalable Long-Term Memory*
  [![arXiv](https://img.shields.io/badge/arXiv-2504.19413-b31b1b.svg)](https://arxiv.org/abs/2504.19413)
- **[arXiv'25.06]** *PersonalAI: A Systematic Comparison of Knowledge Graph Storage and Retrieval Approaches for Personalized LLM Agents*
  [![arXiv](https://img.shields.io/badge/arXiv-2506.17001-b31b1b.svg)](https://arxiv.org/abs/2506.17001)

#### Long-Term Memory — Memory Access and Retrieval (RAG)
- **[NeurIPS'20]** *Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks*
  [![Paper](https://img.shields.io/badge/Paper-NeurIPS-4B5D67.svg)](https://proceedings.neurips.cc/paper/2020/hash/6b493230205f780e1bc26945df7481e5-Abstract.html)
- **[arXiv'25.04]** *Context-Guided Dynamic Retrieval for Improving Generation Quality in RAG Models*
  [![arXiv](https://img.shields.io/badge/arXiv-2504.19436-b31b1b.svg)](https://arxiv.org/abs/2504.19436)
- **[ACL'25]** *Towards Adaptive Memory-Based Optimization for Enhanced Retrieval-Augmented Generation*
  [![Paper](https://img.shields.io/badge/Paper-ACL-4B5D67.svg)](https://doi.org/10.18653/v1/2025.findings-acl.418)
- **[arXiv'25.03]** *Retrieval-Augmented Generation with Hierarchical Knowledge*
  [![arXiv](https://img.shields.io/badge/arXiv-2503.10150-b31b1b.svg)](https://arxiv.org/abs/2503.10150)
- **[ICT'25]** *Enhancing Retrieval Augmented Generation with Hierarchical Text Segmentation Chunking*
  [![Paper](https://img.shields.io/badge/Paper-Springer-4B5D67.svg)](https://link.springer.com/chapter/10.1007/978-981-96-3026-9_16)
- **[JAMIA'25]** *MMRAG: Multi-Mode Retrieval-Augmented Generation with Large Language Models for Biomedical In-Context Learning*
  [![Paper](https://img.shields.io/badge/Paper-JAMIA-4B5D67.svg)](https://doi.org/10.1093/jamia/ocaf128)

#### Long-Term Memory — Procedural
- **[JINT'24]** *A Procedural Constructive Learning Mechanism with Deep Reinforcement Learning for Cognitive Agents*
  [![Paper](https://img.shields.io/badge/Paper-JINT-4B5D67.svg)](https://doi.org/10.1007/s10846-024-02064-9)
- **[Topics Cogn. Sci.'21]** *Reinforcement Learning for Production-Based Cognitive Models*
  [![Paper](https://img.shields.io/badge/Paper-Topics%20Cogn.%20Sci.-4B5D67.svg)](https://doi.org/10.1111/tops.12546)
- **[Sci. Rep.'23]** *A Generalized Reinforcement Learning Based Deep Neural Network Agent Model for Diverse Cognitive Constructs*
  [![Paper](https://img.shields.io/badge/Paper-Sci.%20Rep.-4B5D67.svg)](https://doi.org/10.1038/s41598-023-32234-y)
- **[npj Digit. Med.'22]** *Continuous Monitoring of Surgical Bimanual Expertise Using Deep Neural Networks in Virtual Reality Simulation*
  [![Paper](https://img.shields.io/badge/Paper-npj%20Digit.%20Med.-4B5D67.svg)](https://doi.org/10.1038/s41746-022-00596-8)
- **[Front. Neurorobot.'18]** *Lifelong Learning of Spatiotemporal Representations with Dual-Memory Recurrent Self-Organization*
  [![Paper](https://img.shields.io/badge/Paper-Front.%20Neurorobot.-4B5D67.svg)](https://doi.org/10.3389/fnbot.2018.00078)

<a id="alignment"></a>

### Alignment

#### Alignment with Physical World
- **[ICRA'24]** *Open X-Embodiment: Robotic Learning Datasets and RT-X Models*
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)](https://doi.org/10.1109/ICRA57147.2024.10611477)
  [![arXiv](https://img.shields.io/badge/arXiv-2310.08864-b31b1b.svg)](https://arxiv.org/abs/2310.08864)
- **[CoRL'23]** *RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control*
  [![Paper](https://img.shields.io/badge/Paper-CoRL-4B5D67.svg)](https://proceedings.mlr.press/v229/zitkovich23a.html)
- **[ICML'24]** *3D-VLA: A 3D Vision-Language-Action Generative World Model*
  [![Paper](https://img.shields.io/badge/Paper-ICML-4B5D67.svg)](https://proceedings.mlr.press/v235/zhen24a.html)
  [![arXiv](https://img.shields.io/badge/arXiv-2403.09631-b31b1b.svg)](https://arxiv.org/abs/2403.09631)
- **[arXiv'24.04]** *V-JEPA: Revisiting Feature Prediction for Learning Visual Representations from Video*
  [![arXiv](https://img.shields.io/badge/arXiv-2404.08471-b31b1b.svg)](https://arxiv.org/abs/2404.08471)
- **[arXiv'25.06]** *V-JEPA 2: Self-Supervised Video Models Enable Understanding, Prediction and Planning*
  [![arXiv](https://img.shields.io/badge/arXiv-2506.09985-b31b1b.svg)](https://arxiv.org/abs/2506.09985)
- **[ICML'24]** *RoboDreamer: Learning Compositional World Models for Robot Imagination*
  [![Paper](https://img.shields.io/badge/Paper-ICML-4B5D67.svg)](https://proceedings.mlr.press/v235/zhou24l.html)
  [![arXiv](https://img.shields.io/badge/arXiv-2404.12377-b31b1b.svg)](https://arxiv.org/abs/2404.12377)
- **[CoRL'22]** *SayCan: Do As I Can, Not As I Say — Grounding Language in Robotic Affordances*
  [![Paper](https://img.shields.io/badge/Paper-CoRL-4B5D67.svg)](https://proceedings.mlr.press/v205/ichter23a.html)
- **[ICRA'23]** *ProgPrompt: Generating Situated Robot Task Plans Using Large Language Models*
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)](https://doi.org/10.1109/icra48891.2023.10161317)
- **[CVPR'24]** *Retrieval-Augmented Embodied Agents*
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)](https://doi.org/10.1109/cvpr52733.2024.01703)
- **[arXiv'24.10]** *EmbodiedRAG: Dynamic 3D Scene Graph Retrieval for Efficient and Scalable Robot Task Planning*
  [![arXiv](https://img.shields.io/badge/arXiv-2410.23968-b31b1b.svg)](https://arxiv.org/abs/2410.23968)
- **[arXiv'24.09]** *P-RAG: Progressive Retrieval Augmented Generation For Planning on Embodied Everyday Task*
  [![arXiv](https://img.shields.io/badge/arXiv-2409.11279-b31b1b.svg)](https://arxiv.org/abs/2409.11279)
- **[ICLR'23]** *Mind's Eye: Grounded Language Model Reasoning through Simulation*
  [![Paper](https://img.shields.io/badge/Paper-ICLR-4B5D67.svg)](https://openreview.net/forum?id=4rXMRuoJlai)
  [![arXiv](https://img.shields.io/badge/arXiv-2210.05359-b31b1b.svg)](https://arxiv.org/abs/2210.05359)

#### Alignment with Human Value
- **[arXiv'25.03]** *SafeVLA: Towards Safety Alignment of Vision-Language-Action Model via Constrained Learning*
  [![arXiv](https://img.shields.io/badge/arXiv-2503.03480-b31b1b.svg)](https://arxiv.org/abs/2503.03480)
- **[arXiv'24.11]** *GRAPE: Generalizing Robot Policy via Preference Alignment*
  [![arXiv](https://img.shields.io/badge/arXiv-2411.19309-b31b1b.svg)](https://arxiv.org/abs/2411.19309)
- **[arXiv'25.06]** *HAPO: Human-Assisted Robotic Policy Refinement via Action Preference Optimization*
  [![arXiv](https://img.shields.io/badge/arXiv-2506.07127-b31b1b.svg)](https://arxiv.org/abs/2506.07127)
- **[ICML'23]** *Constrained Decision Transformer for Offline Safe Reinforcement Learning*
  [![Paper](https://img.shields.io/badge/Paper-ICML-4B5D67.svg)](https://proceedings.mlr.press/v202/liu23m.html)
- **[arXiv'24.01]** *AutoRT: Embodied Foundation Models for Large Scale Orchestration of Robotic Agents*
  [![arXiv](https://img.shields.io/badge/arXiv-2401.12963-b31b1b.svg)](https://arxiv.org/abs/2401.12963)
- **[arXiv'25.03]** *Generating Robot Constitutions & Benchmarks for Semantic Safety*
  [![arXiv](https://img.shields.io/badge/arXiv-2503.08663-b31b1b.svg)](https://arxiv.org/abs/2503.08663)
- **[arXiv'25.10]** *ARRC: Advanced Reasoning Robot Control — Knowledge-Driven Autonomous Manipulation Using Retrieval-Augmented Generation*
  [![arXiv](https://img.shields.io/badge/arXiv-2510.05547-b31b1b.svg)](https://arxiv.org/abs/2510.05547)
- **[Auton. Robots'23]** *Text2Motion: From Natural Language Instructions to Feasible Plans*
  [![Paper](https://img.shields.io/badge/Paper-Auton.%20Robots-4B5D67.svg)](https://doi.org/10.1007/s10514-023-10131-7)
- **[ICRA'23]** *Code as Policies: Language Model Programs for Embodied Control*
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)](https://doi.org/10.1109/icra48891.2023.10160591)

<a id="future-directions-cognition"></a>

### Future Directions (Cognition)

Looking forward, we identify the following future directions for Physical Cognition in PAI:

- **Prediction before execution remains central.** World models supporting counterfactual reasoning and imagination are essential for reducing costly and unsafe real-world trial-and-error.
- **Cognition remains hybrid rather than purely end-to-end.** Foundation models offer scale and semantic flexibility, but explicit geometry, structured memory, and control-aware constraints are still required for executability.
- **Memory becomes native infrastructure for long-horizon autonomy.** Episodic, semantic, and procedural memory are not auxiliary add-ons but substrates for continual adaptation, personalization, and skill reuse.
- **Alignment must remain dual and continuous.** Future cognitive systems must be aligned with both the physical world and human values, and this alignment must be enforced at both training and inference time.

---

## 3. Physical Actuation and Execution

> 🚧 This section is under active construction. We are curating papers covering low-level control, learning-based actuation policies, real-world deployment of VLA models, dexterous manipulation, locomotion, and human–robot physical interaction. Contributions are welcome.

---

## 4. Building PAI

This section catalogs the *infrastructure* that enables Physical AI: simulators, data acquisition pipelines, benchmarks, real-world validation protocols, and digital twins. We follow the same `[Venue/Year] — Title` format used throughout the rest of this list.

<a id="simulators"></a>

### Simulators

#### General-Purpose Simulators
- **[Software'23]** — *NVIDIA Isaac Sim: Robotics Simulation and Synthetic Data*
  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://developer.nvidia.com/isaac/sim)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/isaac-sim/IsaacSim)
- **[arXiv'21]** — *Isaac Gym: High Performance GPU-Based Physics Simulation For Robot Learning*
  [![Paper](https://img.shields.io/badge/Paper-OpenReview-4B5D67.svg)](https://openreview.net/forum?id=fgFBtYgJQX_)
  [![arXiv](https://img.shields.io/badge/arXiv-2108.10470-b31b1b.svg)](https://arxiv.org/abs/2108.10470)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/isaac-sim/IsaacGymEnvs)
- **[IROS'04]** — *Design and use paradigms for Gazebo, an open-source multi-robot simulator*
  [![Paper](https://img.shields.io/badge/Paper-IEEE-4B5D67.svg)](https://doi.org/10.1109/iros.2004.1389727)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/gazebosim/gz-sim)
  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://gazebosim.org/)
- **[Software'16]** — *PyBullet: A Python module for physics simulation for games, robotics and machine learning*
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/bulletphysics/bullet3)
  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://pybullet.org/wordpress/)
- **[IROS'12]** — *MuJoCo: A physics engine for model-based control*
  [![Paper](https://img.shields.io/badge/Paper-IROS-4B5D67.svg)](https://doi.org/10.1109/IROS.2012.6386109)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/google-deepmind/mujoco)
  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://mujoco.org/)
- **[arXiv'04]** — *Webots: Professional Mobile Robot Simulation*
  [![arXiv](https://img.shields.io/badge/arXiv-cs/0412052-b31b1b.svg)](https://arxiv.org/abs/cs/0412052)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/cyberbotics/webots)
- **[arXiv'17]** — *AirSim: High-Fidelity Visual and Physical Simulation for Autonomous Vehicles*
  [![arXiv](https://img.shields.io/badge/arXiv-1705.05065-b31b1b.svg)](https://arxiv.org/abs/1705.05065)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/microsoft/AirSim)
- **[arXiv'18]** — *Unity: A General Platform for Intelligent Agents*
  [![arXiv](https://img.shields.io/badge/arXiv-1809.02627-b31b1b.svg)](https://arxiv.org/abs/1809.02627)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/Unity-Technologies/ml-agents)
- **[IROS'13]** — *V-REP: A versatile and scalable robot simulation framework*
  [![Paper](https://img.shields.io/badge/Paper-IROS-4B5D67.svg)](https://doi.org/10.1109/IROS.2013.6696520)

#### Real-Scene Based Simulators
- **[arXiv'17]** — *AI2-THOR: An Interactive 3D Environment for Visual AI*
  [![arXiv](https://img.shields.io/badge/arXiv-1712.05474-b31b1b.svg)](https://arxiv.org/abs/1712.05474)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/allenai/ai2thor)
  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://ai2thor.allenai.org/)
- **[3DV'17]** — *Matterport3D: Learning from RGB-D Data in Indoor Environments*
  [![arXiv](https://img.shields.io/badge/arXiv-1709.06158-b31b1b.svg)](https://arxiv.org/abs/1709.06158)
  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://niessner.github.io/Matterport/)
- **[CVPR'18]** — *VirtualHome: Simulating Household Activities via Programs*
  [![arXiv](https://img.shields.io/badge/arXiv-1806.07011-b31b1b.svg)](https://arxiv.org/abs/1806.07011)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/xavierpuigf/virtualhome)
  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](http://virtual-home.org/)
- **[ICCV'19]** — *Habitat: A Platform for Embodied AI Research*
  [![arXiv](https://img.shields.io/badge/arXiv-1904.01201-b31b1b.svg)](https://arxiv.org/abs/1904.01201)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/facebookresearch/habitat-lab)
  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://aihabitat.org/)
- **[CVPR'20]** — *SAPIEN: A SimulAted Part-based Interactive ENvironment*
  [![arXiv](https://img.shields.io/badge/arXiv-2003.08515-b31b1b.svg)](https://arxiv.org/abs/2003.08515)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/haosulab/SAPIEN)
  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://sapien.ucsd.edu/)
- **[arXiv'20]** — *iGibson 1.0: a Simulation Environment for Interactive Tasks in Large Realistic Scenes*
  [![arXiv](https://img.shields.io/badge/arXiv-2012.02924-b31b1b.svg)](https://arxiv.org/abs/2012.02924)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/StanfordVL/iGibson)
- **[arXiv'21]** — *iGibson 2.0: Object-Centric Simulation for Robot Learning of Everyday Household Tasks*
  [![arXiv](https://img.shields.io/badge/arXiv-2108.03272-b31b1b.svg)](https://arxiv.org/abs/2108.03272)
- **[arXiv'20]** — *ThreeDWorld: A Platform for Interactive Multi-Modal Physical Simulation*
  [![arXiv](https://img.shields.io/badge/arXiv-2007.04954-b31b1b.svg)](https://arxiv.org/abs/2007.04954)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/threedworld-mit/tdw)
- **[NeurIPS'22]** — *ProcTHOR: Large-Scale Embodied AI Using Procedural Generation*
  [![arXiv](https://img.shields.io/badge/arXiv-2206.06994-b31b1b.svg)](https://arxiv.org/abs/2206.06994)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/allenai/procthor)
- **[arXiv'23]** — *RoboGen: Towards Unleashing Infinite Data for Automated Robot Learning via Generative Simulation*
  [![arXiv](https://img.shields.io/badge/arXiv-2311.01455-b31b1b.svg)](https://arxiv.org/abs/2311.01455)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/Genesis-Embodied-AI/RoboGen)
- **[arXiv'23]** — *Holodeck: Language Guided Generation of 3D Embodied AI Environments*
  [![arXiv](https://img.shields.io/badge/arXiv-2312.09067-b31b1b.svg)](https://arxiv.org/abs/2312.09067)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/allenai/Holodeck)
- **[arXiv'24]** — *PhyScene: Physically Interactable 3D Scene Synthesis for Embodied AI*
  [![arXiv](https://img.shields.io/badge/arXiv-2404.09465-b31b1b.svg)](https://arxiv.org/abs/2404.09465)

#### Domain-Specific Simulators
- **[CoRL'17]** — *CARLA: An Open Urban Driving Simulator*
  [![arXiv](https://img.shields.io/badge/arXiv-1711.03938-b31b1b.svg)](https://arxiv.org/abs/1711.03938)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/carla-simulator/carla)
  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://carla.org/)
- **[ITSC'18]** — *Microscopic Traffic Simulation using SUMO*
  [![Paper](https://img.shields.io/badge/Paper-ITSC-4B5D67.svg)](https://doi.org/10.1109/ITSC.2018.8569938)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/eclipse-sumo/sumo)
- **[CVPR'22]** — *NuPlan: A closed-loop ML-based planning benchmark for autonomous vehicles*
  [![arXiv](https://img.shields.io/badge/arXiv-2106.11810-b31b1b.svg)](https://arxiv.org/abs/2106.11810)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/motional/nuplan-devkit)
- **[arXiv'23]** — *Waymax: An Accelerated, Data-Driven Simulator for Large-Scale Autonomous Driving Research*
  [![arXiv](https://img.shields.io/badge/arXiv-2310.08710-b31b1b.svg)](https://arxiv.org/abs/2310.08710)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/waymo-research/waymax)
- **[LRA'22]** — *TACTO: A Fast, Flexible, and Open-Source Simulator for High-Resolution Vision-Based Tactile Sensors*
  [![arXiv](https://img.shields.io/badge/arXiv-2012.08456-b31b1b.svg)](https://arxiv.org/abs/2012.08456)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/facebookresearch/tacto)
- **[ECCV'20]** — *SoundSpaces: Audio-Visual Navigation in 3D Environments*
  [![arXiv](https://img.shields.io/badge/arXiv-1912.11474-b31b1b.svg)](https://arxiv.org/abs/1912.11474)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/facebookresearch/sound-spaces)
- **[Software'23]** — *Wireless InSite*
  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://www.remcom.com/wireless-insite-em-propagation-software)
- **[ICC'17]** — *A novel millimeter-wave channel simulator and applications for 5G wireless communications (NYUSIM)*
  [![Paper](https://img.shields.io/badge/Paper-ICC-4B5D67.svg)](https://doi.org/10.1109/ICC.2017.7996792)
  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://wireless.engineering.nyu.edu/nyusim/)
- **[ICISP'11]** — *IMUSim: A Simulation Environment for Inertial Sensing Algorithm Design and Evaluation*
  [![Paper](https://img.shields.io/badge/Paper-ICISP-4B5D67.svg)](https://ieeexplore.ieee.org/document/5779038)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/martinling/imusim)

<a id="data-collection"></a>

### Data Collection

#### Real-World Robot Data Acquisition
- **[arXiv'24]** — *Mobile ALOHA: Learning Bimanual Mobile Manipulation with Low-Cost Whole-Body Teleoperation*
  [![arXiv](https://img.shields.io/badge/arXiv-2401.02117-b31b1b.svg)](https://arxiv.org/abs/2401.02117)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/MarkFzp/mobile-aloha)
- **[arXiv'24]** — *Universal Manipulation Interface: In-the-Wild Robot Teaching without In-the-Wild Robots*
  [![arXiv](https://img.shields.io/badge/arXiv-2402.10329-b31b1b.svg)](https://arxiv.org/abs/2402.10329)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/real-stanford/universal_manipulation_interface)
- **[RSS'23]** — *AnyTeleop: A General Vision-Based Dexterous Robot Arm-Hand Teleoperation System*
  [![arXiv](https://img.shields.io/badge/arXiv-2307.04577-b31b1b.svg)](https://arxiv.org/abs/2307.04577)
- **[arXiv'24]** — *Human-Agent Joint Learning for Efficient Robot Manipulation Skill Acquisition*
  [![arXiv](https://img.shields.io/badge/arXiv-2407.00299-b31b1b.svg)](https://arxiv.org/abs/2407.00299)
- **[arXiv'24]** — *DROID: A Large-Scale In-The-Wild Robot Manipulation Dataset*
  [![arXiv](https://img.shields.io/badge/arXiv-2403.12945-b31b1b.svg)](https://arxiv.org/abs/2403.12945)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/droid-dataset/droid)
- **[arXiv'24]** — *Open X-Embodiment: Robotic Learning Datasets and RT-X Models*
  [![arXiv](https://img.shields.io/badge/arXiv-2310.08864-b31b1b.svg)](https://arxiv.org/abs/2310.08864)
- **[arXiv'25]** — *AgiBot World Colosseo: A Large-scale Manipulation Platform for Scalable and Intelligent Embodied Systems*
  [![arXiv](https://img.shields.io/badge/arXiv-2503.06669-b31b1b.svg)](https://arxiv.org/abs/2503.06669)
- **[arXiv'24]** — *All Robots in One: A New Standard and Unified Dataset for Versatile, General-Purpose Embodied Agents*
  [![arXiv](https://img.shields.io/badge/arXiv-2408.10899-b31b1b.svg)](https://arxiv.org/abs/2408.10899)
- **[CVPR'20]** — *GraspNet-1Billion: A Large-Scale Benchmark for General Object Grasping*
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)](https://openaccess.thecvf.com/content_CVPR_2020/html/Fang_GraspNet-1Billion_A_Large-Scale_Benchmark_for_General_Object_Grasping_CVPR_2020_paper.html)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/graspnet/graspnet-baseline)
- **[arXiv'25]** — *M³A Policy: Mutable Material Manipulation Augmentation Policy through Photometric Re-rendering*
  [![arXiv](https://img.shields.io/badge/arXiv-2512.01446-b31b1b.svg)](https://arxiv.org/abs/2512.01446)

#### Simulation-Based Data Generation
- **[CoRL'21]** — *CLIPort: What and Where Pathways for Robotic Manipulation*
  [![arXiv](https://img.shields.io/badge/arXiv-2109.12098-b31b1b.svg)](https://arxiv.org/abs/2109.12098)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/cliport/cliport)
- **[CoRL'20]** — *Transporter Networks: Rearranging the Visual World for Robotic Manipulation*
  [![arXiv](https://img.shields.io/badge/arXiv-2010.14406-b31b1b.svg)](https://arxiv.org/abs/2010.14406)
- **[arXiv'22]** — *GAPartNet: Cross-Category Domain-Generalizable Object Perception and Manipulation via Generalizable and Actionable Parts*
  [![arXiv](https://img.shields.io/badge/arXiv-2211.05272-b31b1b.svg)](https://arxiv.org/abs/2211.05272)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/PKU-EPIC/GAPartNet)
- **[arXiv'24]** — *SemGrasp: Semantic Grasp Generation via Language Aligned Discretization*
  [![arXiv](https://img.shields.io/badge/arXiv-2404.03590-b31b1b.svg)](https://arxiv.org/abs/2404.03590)
- **[CVPR'18]** — *Vision-and-Language Navigation: Interpreting Visually-Grounded Navigation Instructions in Real Environments*
  [![arXiv](https://img.shields.io/badge/arXiv-1711.07280-b31b1b.svg)](https://arxiv.org/abs/1711.07280)
- **[CVPR'20]** — *REVERIE: Remote Embodied Visual Referring Expression in Real Indoor Environments*
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)](https://openaccess.thecvf.com/content_CVPR_2020/html/Qi_REVERIE_Remote_Embodied_Visual_Referring_Expression_in_Real_Indoor_Environments_CVPR_2020_paper.html)
- **[EMNLP'20]** — *Room-Across-Room: Multilingual Vision-and-Language Navigation with Dense Spatiotemporal Grounding*
  [![arXiv](https://img.shields.io/badge/arXiv-2004.02709-b31b1b.svg)](https://arxiv.org/abs/2004.02709)
- **[arXiv'24]** — *NaVILA: Legged Robot Vision-Language-Action Model for Navigation*
  [![arXiv](https://img.shields.io/badge/arXiv-2412.04453-b31b1b.svg)](https://arxiv.org/abs/2412.04453)
- **[arXiv'25]** — *StreamVLN: Streaming Vision-and-Language Navigation via SlowFast Context Modeling*
  [![arXiv](https://img.shields.io/badge/arXiv-2507.05240-b31b1b.svg)](https://arxiv.org/abs/2507.05240)
- **[CoRL'23]** — *MimicGen: A Data Generation System for Scalable Robot Learning using Human Demonstrations*
  [![arXiv](https://img.shields.io/badge/arXiv-2310.17596-b31b1b.svg)](https://arxiv.org/abs/2310.17596)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/NVlabs/mimicgen_environments)
- **[ICRA'25]** — *DexMimicGen: Automated Data Generation for Bimanual Dexterous Manipulation via Imitation Learning*
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)](https://doi.org/10.1109/ICRA55743.2025.11127809)
- **[arXiv'23]** — *RoboGen: Towards Unleashing Infinite Data for Automated Robot Learning via Generative Simulation*
  [![arXiv](https://img.shields.io/badge/arXiv-2311.01455-b31b1b.svg)](https://arxiv.org/abs/2311.01455)
- **[ICLR'23]** — *GenSim: Generating Robotic Simulation Tasks via Large Language Models*
  [![arXiv](https://img.shields.io/badge/arXiv-2310.01361-b31b1b.svg)](https://arxiv.org/abs/2310.01361)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/liruiw/GenSim)
- **[arXiv'24]** — *RoboCasa: Large-Scale Simulation of Everyday Tasks for Generalist Robots*
  [![arXiv](https://img.shields.io/badge/arXiv-2406.02523-b31b1b.svg)](https://arxiv.org/abs/2406.02523)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/robocasa/robocasa)
- **[arXiv'24]** — *BEHAVIOR-1K: A Human-Centered, Embodied AI Benchmark with 1,000 Everyday Activities and Realistic Simulation*
  [![arXiv](https://img.shields.io/badge/arXiv-2403.09227-b31b1b.svg)](https://arxiv.org/abs/2403.09227)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/StanfordVL/BEHAVIOR-1K)

#### Human Video and Web-Scale Data
- **[CVPR'22]** — *Ego4D: Around the World in 3,000 Hours of Egocentric Video*
  [![arXiv](https://img.shields.io/badge/arXiv-2110.07058-b31b1b.svg)](https://arxiv.org/abs/2110.07058)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/facebookresearch/Ego4d)
- **[arXiv'23]** — *Ego-Exo4D: Understanding Skilled Human Activity from First- and Third-Person Perspectives*
  [![arXiv](https://img.shields.io/badge/arXiv-2311.18259-b31b1b.svg)](https://arxiv.org/abs/2311.18259)
- **[IJCV'22]** — *Rescaling Egocentric Vision: Collection, Pipeline and Challenges for EPIC-KITCHENS-100*
  [![arXiv](https://img.shields.io/badge/arXiv-2006.13256-b31b1b.svg)](https://arxiv.org/abs/2006.13256)
- **[arXiv'23]** — *HoloAssist: An Egocentric Human Interaction Dataset for Interactive AI Assistants in the Real World*
  [![arXiv](https://img.shields.io/badge/arXiv-2309.17024-b31b1b.svg)](https://arxiv.org/abs/2309.17024)
- **[ICCV'17]** — *The "something something" video database for learning and evaluating visual common sense*
  [![arXiv](https://img.shields.io/badge/arXiv-1706.04261-b31b1b.svg)](https://arxiv.org/abs/1706.04261)
- **[ICCV'19]** — *HowTo100M: Learning a Text-Video Embedding by Watching Hundred Million Narrated Video Clips*
  [![arXiv](https://img.shields.io/badge/arXiv-1906.03327-b31b1b.svg)](https://arxiv.org/abs/1906.03327)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/antoine77340/howto100m)
- **[CoRL'23]** — *RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control*
  [![arXiv](https://img.shields.io/badge/arXiv-2307.15818-b31b1b.svg)](https://arxiv.org/abs/2307.15818)
- **[arXiv'24]** — *GR-2: A Generative Video-Language-Action Model with Web-Scale Knowledge for Robot Manipulation*
  [![arXiv](https://img.shields.io/badge/arXiv-2410.06158-b31b1b.svg)](https://arxiv.org/abs/2410.06158)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/THU-VCLab/GR-2)
- **[arXiv'26]** — *Fast SAM 3D Body: Accelerating SAM 3D Body for Real-Time Full-Body Human Mesh Recovery*
  [![arXiv](https://img.shields.io/badge/arXiv-2603.15603-b31b1b.svg)](https://arxiv.org/abs/2603.15603)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/yangtiming/Fast-SAM-3D-Body)

<a id="simulation-benchmarks"></a>

### Simulation Benchmarks

- **[arXiv'19]** — *RLBench: The Robot Learning Benchmark & Learning Environment*
  [![arXiv](https://img.shields.io/badge/arXiv-1909.12271-b31b1b.svg)](https://arxiv.org/abs/1909.12271)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/stepjam/RLBench)
- **[CoRL'20]** — *Meta-World: A Benchmark and Evaluation for Multi-Task and Meta Reinforcement Learning*
  [![arXiv](https://img.shields.io/badge/arXiv-1910.10897-b31b1b.svg)](https://arxiv.org/abs/1910.10897)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/Farama-Foundation/Metaworld)
- **[LRA'22]** — *CALVIN: A Benchmark for Language-Conditioned Policy Learning for Long-Horizon Robot Manipulation Tasks*
  [![arXiv](https://img.shields.io/badge/arXiv-2112.03227-b31b1b.svg)](https://arxiv.org/abs/2112.03227)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/mees/calvin)
- **[arXiv'21]** — *ManiSkill: Generalizable Manipulation Skill Benchmark with Large-Scale Demonstrations*
  [![arXiv](https://img.shields.io/badge/arXiv-2107.14483-b31b1b.svg)](https://arxiv.org/abs/2107.14483)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/haosulab/ManiSkill)
- **[ICCV'19]** — *Habitat: A Platform for Embodied AI Research*
  [![arXiv](https://img.shields.io/badge/arXiv-1904.01201-b31b1b.svg)](https://arxiv.org/abs/1904.01201)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/facebookresearch/habitat-lab)
- **[CVPR'20]** — *ALFRED: A Benchmark for Interpreting Grounded Instructions for Everyday Tasks*
  [![arXiv](https://img.shields.io/badge/arXiv-1912.01734-b31b1b.svg)](https://arxiv.org/abs/1912.01734)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/askforalfred/alfred)
- **[CVPR'18]** — *Embodied Question Answering*
  [![arXiv](https://img.shields.io/badge/arXiv-1711.11543-b31b1b.svg)](https://arxiv.org/abs/1711.11543)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/facebookresearch/EmbodiedQA)
- **[CVPR'20]** — *nuScenes: A Multimodal Dataset for Autonomous Driving*
  [![arXiv](https://img.shields.io/badge/arXiv-1903.11027-b31b1b.svg)](https://arxiv.org/abs/1903.11027)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/nutonomy/nuscenes-devkit)
- **[CVPR'20]** — *Scalability in Perception for Autonomous Driving: Waymo Open Dataset*
  [![arXiv](https://img.shields.io/badge/arXiv-1912.04838-b31b1b.svg)](https://arxiv.org/abs/1912.04838)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/waymo-research/waymo-open-dataset)
- **[CoRL'17]** — *CARLA: An Open Urban Driving Simulator*
  [![arXiv](https://img.shields.io/badge/arXiv-1711.03938-b31b1b.svg)](https://arxiv.org/abs/1711.03938)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/carla-simulator/carla)

<a id="real-world-validation-protocols"></a>

### Real-World Validation Protocols

- **[arXiv'24]** — *ALOHA 2: An Enhanced Low-Cost Hardware for Bimanual Teleoperation*
  [![arXiv](https://img.shields.io/badge/arXiv-2405.02292-b31b1b.svg)](https://arxiv.org/abs/2405.02292)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/tonyzhaozh/aloha)
- **[arXiv'24]** — *Mobile ALOHA: Learning Bimanual Mobile Manipulation with Low-Cost Whole-Body Teleoperation*
  [![arXiv](https://img.shields.io/badge/arXiv-2401.02117-b31b1b.svg)](https://arxiv.org/abs/2401.02117)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/MarkFzp/mobile-aloha)

<a id="digital-twin"></a>

### Digital Twin

#### Concept and Architecture
- **[Book'17]** — *Digital Twin: Mitigating Unpredictable, Undesirable Emergent Behavior in Complex Systems*
  [![Paper](https://img.shields.io/badge/Paper-Link-4B5D67.svg)](https://doi.org/10.1007/978-3-319-38756-7_4)
- **[IEEE Access'17]** — *Digital Twin Shop-Floor: A New Shop-Floor Paradigm Towards Smart Manufacturing*
  [![Paper](https://img.shields.io/badge/Paper-Link-4B5D67.svg)](https://doi.org/10.1109/access.2017.2756069)

#### Role in PAI Development
- **[JMSY'21]** — *Review of Digital Twin About Concepts, Technologies, and Industrial Applications*
  [![Paper](https://img.shields.io/badge/Paper-JMSY-4B5D67.svg)](https://doi.org/10.1016/j.jmsy.2020.06.017)
- **[IEEE Access'20]** — *Digital Twin: Values, Challenges and Enablers From a Modeling Perspective*
  [![Paper](https://img.shields.io/badge/Paper-IEEE%20Access-4B5D67.svg)](https://doi.org/10.1109/ACCESS.2020.2970143)
- **[Software'23]** — *NVIDIA Omniverse Platform*
  [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://www.nvidia.com/en-us/omniverse/)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/NVIDIA-Omniverse)

#### From Offline Simulation to Online Synchronization
- **[Nat. Comput. Sci.'21]** — *A probabilistic graphical model foundation for enabling predictive digital twins at scale*
  [![Paper](https://img.shields.io/badge/Paper-Link-4B5D67.svg)](https://doi.org/10.1038/s43588-021-00069-0)

---

## Citation

If you find this repository useful for your research, please consider citing our survey:

```bibtex
@article{liu2026physicalai,
  title   = {Physical AI: A Comprehensive Survey of Enabling Technologies From
A Systems Perspective},
  author  = {Liu, Shengding and Zhang, Zhanwei and Li, Zhiying and Lin, Yudi and Lin, Ruxin and Liu, Xiaoqun and Nguyen, Khang and Gao, Ziran and Liao, Guopeng and Mo, Jingxiang and Jiang, Linshan and Yang, Jianfei and Azulay, Osher and Yu, Stella X. and Yu, Philip S. and Yan, Qiben},
  year    = {2026},
}
```

## Contributing

Contributions are very welcome! Please:

- Open an issue to suggest new papers, fix metadata, or report broken links.
- Submit a pull request that follows the existing entry format:
  ```
  - **[Venue/Year]** *Paper Title*
    [![Paper](...)] [![arXiv](...)] [![GitHub](...)] [![Website](...)]
  ```
- Group your additions under the most appropriate section. If a new subsection is warranted, mention it in your PR description.

## Acknowledgements

This list builds on community efforts in Embodied AI, Mobile and Wireless Sensing, AIoT, Cyber-Physical Systems, and Robot Learning. We thank all authors of the papers cited here for their contributions to the field.
