# 4. Physical Perception in PAI


### Table of Contents

- [Perception Modalities](#perception-modalities)
- [Physics-Informed Perception](#physics-informed-perception)
  - [Signal Propagation Modeling](#signal-propagation-modeling)
  - [Phase and Frequency Dynamics Modeling](#phase-and-frequency-dynamics-modeling)
  - [Physical Interaction and Transduction Modeling](#physical-interaction-and-transduction-modeling)
- [Data-Driven Perception](#data-driven-perception)
  - [Task-Specific Discriminative Perception](#task-specific-discriminative-perception)
  - [Data-Efficient Perception](#data-efficient-perception)
- [Generative Perception](#generative-perception)
  - [Semantic World Understanding](#semantic-world-understanding)
  - [Sensor-grounded Reasoning](#sensor-grounded-reasoning)
  - [Sensor Data Synthesis](#sensor-data-synthesis)
- [Sensor Fusion and Multimodal Perception](#sensor-fusion-and-multimodal-perception)
  - [Architectural Fusion Strategies](#architectural-fusion-strategies)
  - [Cross-Modal Association and Robustness](#cross-modal-association-and-robustness)
  - [Spatiotemporal, Collaborative, and Foundation-Model Fusion](#spatiotemporal-collaborative-and-foundation-model-fusion)
- [Perception Tasks](#perception-tasks)
  - [Object Perception](#object-perception)
  - [Scene Perception](#scene-perception)
  - [Human Perception](#human-perception)

---

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

- **[Paper'23]** *SparseIMU: Computational Design of Sparse IMU Layouts for Sensing Fine-grained Finger Microgestures*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1145/3569894)  
- **[UIST'23]** *SmartPoser: Arm Pose Estimation with a Smartphone and Smartwatch Using UWB and IMU Data*  
  [![Paper](https://img.shields.io/badge/Paper-UIST-4B5D67.svg)](https://doi.org/10.1145/3586183.3606821)  
- **[IMWUT'23]** *Optimization-Free Test-Time Adaptation for Cross-Person Activity Recognition*  
  [![Paper](https://img.shields.io/badge/Paper-IMWUT-4B5D67.svg)](https://doi.org/10.1145/3631450)  
- **[IMWUT'24]** *Sf-adapter: Computational-efficient source-free domain adaptation for human activity recognition*  
  [![Paper](https://img.shields.io/badge/Paper-IMWUT-4B5D67.svg)]()  



<a id="physics-informed-perception"></a>

### Physics-Informed Perception




<a id="signal-propagation-modeling"></a>

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

<a id="phase-and-frequency-dynamics-modeling"></a>

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



<a id="physical-interaction-and-transduction-modeling"></a>

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

<a id="task-specific-discriminative-perception"></a>

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


<a id="data-efficient-perception"></a>

#### Data-Efficient Perception

- **[SenSys'20]** *RF-net: A unified meta-learning framework for RF-enabled one-shot human activity recognition*  
  [![Paper](https://img.shields.io/badge/Paper-SenSys-4B5D67.svg)]()  
- **[SenSys'21]** *Onefi: One-shot recognition for unseen gesture via cots wifi*  
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

<a id="semantic-world-understanding"></a>

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
- **[ECCV'24]** *Diffusion model is a good pose estimator from 3d rf-vision*  
  [![Paper](https://img.shields.io/badge/Paper-ECCV-4B5D67.svg)]()  

<a id="sensor-grounded-reasoning"></a>

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

<a id="sensor-data-synthesis"></a>

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

<a id="architectural-fusion-strategies"></a>

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
- **[IROS'19]** *Frustum convnet: Sliding frustums to aggregate local point-wise features for amodal 3d object detection*  
  [![Paper](https://img.shields.io/badge/Paper-IROS-4B5D67.svg)]()  

<a id="cross-modal-association-and-robustness"></a>

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

<a id="spatiotemporal-collaborative-and-foundation-model-fusion"></a>

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
- **[ECCV'22.03]** *BEVFormer: Learning Bird's-Eye-View Representation from Multi-Camera Images via Spatiotemporal Transformers*  
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

<a id="object-perception"></a>

#### Object Perception

- **[arXiv'25.10]** *Towards 3D Objectness Learning in an Open World*  
  [![arXiv](https://img.shields.io/badge/arXiv-2510.17686-b31b1b.svg)](https://arxiv.org/abs/2510.17686)  
- **[CVPR'22]** *Multimodal Material Segmentation*  
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)](https://doi.org/10.1109/cvpr52688.2022.01918)  
- **[MobiCom'21]** *RFID and camera fusion for recognition of human-object interactions*  
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)](https://doi.org/10.1145/3447993.3483244)  
- **[MobiCom'23]** *MobiSpectral: Hyperspectral Imaging on Mobile Devices*  
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)](https://doi.org/10.1145/3570361.3613296)  
- **[ICML'21]** *Learning Transferable Visual Models From Natural Language Supervision*  
  [![Paper](https://img.shields.io/badge/Paper-ICML-4B5D67.svg)](https://proceedings.mlr.press/v139/radford21a.html)  
- **[MobiSys'23]** *Contactless Material Identification with Millimeter Wave Vibrometry*  
  [![Paper](https://img.shields.io/badge/Paper-MobiSys-4B5D67.svg)](https://doi.org/10.1145/3581791.3596850)  
- **[ICLR'26]** *RF-MatID: Dataset and Benchmark for Radio Frequency Material Identification*  
  [![Paper](https://img.shields.io/badge/Paper-ICLR-4B5D67.svg)]()  
- **[Paper'21]** *milliEye: A Lightweight mmWave Radar and Camera Fusion System for Robust Object Detection*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)]()  
- **[SenSys'21]** *RFusion: Robotic Grasping via RF-Visual Sensing and Learning*  
  [![Paper](https://img.shields.io/badge/Paper-SenSys-4B5D67.svg)]()  

<a id="scene-perception"></a>

#### Scene Perception

- **[Paper'23]** *A Survey on Deep Learning Based Segmentation, Detection and Classification for 3D Point Clouds*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.3390/e25040635)  
- **[CACM'22]** *NeRF: Representing Scenes as Neural Radiance Fields for View Synthesis*  
  [![Paper](https://img.shields.io/badge/Paper-CACM-4B5D67.svg)]()  
- **[Paper'23]** *3D Gaussian Splatting for Real-Time Radiance Field Rendering*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1145/3592433)  
- **[arXiv'24.04]** *PhyScene: Physically Interactable 3D Scene Synthesis for Embodied AI*  
  [![arXiv](https://img.shields.io/badge/arXiv-2404.09465-b31b1b.svg)](https://arxiv.org/abs/2404.09465)  
- **[ECCV'23.11]** *OccWorld: Learning a 3D Occupancy World Model for Autonomous Driving*  
  [![arXiv](https://img.shields.io/badge/arXiv-2311.16038-b31b1b.svg)](https://arxiv.org/abs/2311.16038)  
- **[CVPR'20]** *REVERIE: Remote Embodied Visual Referring Expression in Real Indoor Environments*  
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)](https://doi.org/10.1109/cvpr42600.2020.01000)  
- **[MobiCom'24]** *Enabling Visual Recognition at Radio Frequency*  
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)](https://doi.org/10.1145/3636534.3649369)  
- **[MobiCom'22]** *VIPS: Real-Time Perception Fusion for Infrastructure-Assisted Autonomous Driving*  
  [![Paper](https://img.shields.io/badge/Paper-MobiCom-4B5D67.svg)]()  
- **[SenSys'24]** *Boosting Collaborative Vehicular Perception on the Edge with Vehicle-to-Vehicle Communication*  
  [![Paper](https://img.shields.io/badge/Paper-SenSys-4B5D67.svg)](https://doi.org/10.1145/3666025.3699328)  
- **[arXiv'24.09]** *Generative AI-Enhanced Multi-Modal Semantic Communication in Internet of Vehicles: System Design and Methodologies*  
  [![arXiv](https://img.shields.io/badge/arXiv-2409.15642-b31b1b.svg)](https://arxiv.org/abs/2409.15642)  

<a id="human-perception"></a>

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
- **[Paper'24]** *HARGPT: Are LLMs Zero-Shot Human Activity Recognizers?*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1109/fmsys62467.2024.00011)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/aiot-lab/HARGPT)  
- **[Paper'25]** *ContextLLM: Meaningful Context Reasoning from Multi-Sensor and Multi-Device Data Using LLMs*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1145/3708468.3711892)  
- **[arXiv'24.06]** *LLaSA: A Sensor-Aware LLM for Natural Language Reasoning of Human Activity from IMU Data*  
  [![arXiv](https://img.shields.io/badge/arXiv-2406.14498-b31b1b.svg)](https://arxiv.org/abs/2406.14498)  
- **[ACL'25]** *ProMind-LLM: Proactive Mental Health Care via Causal Reasoning with Sensor Data*  
  [![Paper](https://img.shields.io/badge/Paper-ACL-4B5D67.svg)](https://doi.org/10.18653/v1/2025.findings-acl.1033)  
- **[ACL'25]** *MEIT: Multimodal Electrocardiogram Instruction Tuning on Large Language Models for Report Generation*  
  [![Paper](https://img.shields.io/badge/Paper-ACL-4B5D67.svg)](https://doi.org/10.18653/v1/2025.findings-acl.749)
  [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/AIoT-MLSys-Lab/MEIT)  


