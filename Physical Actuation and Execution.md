<a id="3-physical-actuation-and-execution"></a>

# 3. Physical Actuation and Execution

The physical actuation layer translates cognitive intent into forces, motions, and interactions in the real world. This page curates papers organized along three themes: **Actuators and End-Effectors** (the physical hardware substrate); **Physical Control** (mapping trajectories to stable real-time motor commands); and **Closed-Loop Execution and Interaction** (closed-loop behaviors in the real world).


<a id="table-of-contents"></a>

## Table of Contents

- [Actuators and End-Effectors](#actuators-and-end-effectors)
  - [Foundations and Taxonomy](#foundations-and-taxonomy)
  - [Representative Actuator Families](#representative-actuator-families)
  - [End-Effectors and Grippers](#end-effectors-and-grippers)
- [Physical Control](#physical-control)
  - [Classical and Optimization-Based Control](#classical-and-optimization-based-control)
  - [Learning-Based Control for Physical Embodiments](#learning-based-control-for-physical-embodiments)
  - [Foundation-Model-Based Action Generation](#foundation-model-based-action-generation)
- [Closed-Loop Execution and Interaction](#closed-loop-execution-and-interaction)
  - [Locomotion and Navigation](#locomotion-and-navigation)
  - [Manipulation and Grasping](#manipulation-and-grasping)
  - [Physical Human–Robot Interaction and Collaboration](#physical-humanrobot-interaction-and-collaboration)
  - [Active Perception and Environment Exploration](#active-perception-and-environment-exploration)
  - [Language-Conditioned and Human-in-the-Loop Execution](#language-conditioned-and-human-in-the-loop-execution)

---

<a id="actuators-and-end-effectors"></a>

### Actuators and End-Effectors

<a id="foundations-and-taxonomy"></a>

#### Foundations and Taxonomy

- **[Proc. R. Soc. A'97]** *The selection of mechanical actuators based on performance indices*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1098/rspa.1997.0117)

- **[Nature'15]** *Design, fabrication and control of soft robots*  
  [![Paper](https://img.shields.io/badge/Paper-Nature-4B5D67.svg)](https://doi.org/10.1038/nature14543)

- **[IEEE RAM'25]** *A Survey on Soft Robot Adaptability: Implementations, Applications, and Prospects*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1109/mra.2025.3584346) [![arXiv](https://img.shields.io/badge/arXiv-2506.19397-b31b1b.svg)](https://arxiv.org/abs/2506.19397)

- **[ACM CSUR'24]** *A Survey on Robotic Prosthetics: Neuroprosthetics, Soft Actuators, and Control Strategies*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1145/3648355)

- **[Nature Medicine'24]** *Continuous neural control of a bionic limb restores biomimetic gait after amputation*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1038/s41591-024-02994-9)

- **[Nat. Biomed. Eng.'23]** *Opportunities and challenges in the development of exoskeletons for locomotor assistance*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1038/s41551-022-00984-1)

- **[Nat. Rev. Bioeng.'25]** *Soft robotics for personalized and sustainable wearables*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1038/s44222-025-00359-6)

- **[Curr. Robot. Rep.'23]** *Bioinspired Soft Robotics: State of the Art, Challenges, and Future Directions*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1007/s43154-023-00102-2)

<a id="representative-actuator-families"></a>

#### Representative Actuator Families

##### Electrical / Electromagnetic Actuation

- **[ICRA'19]** *Quasi-Direct Drive for Low-Cost Compliant Robotic Manipulation*  
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)](https://doi.org/10.1109/icra.2019.8794236) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://berkeleyopenarms.github.io/)

- **[ICRA'19]** *Mini Cheetah: A Platform for Pushing the Limits of Dynamic Quadruped Control*  
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)](https://doi.org/10.1109/ICRA.2019.8793865) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/mit-biomimetics/Cheetah-Software)

- **[IEEE RA-L'20]** *An Open Torque-Controlled Modular Robot Architecture for Legged Locomotion Research*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1109/lra.2020.2976639) [![arXiv](https://img.shields.io/badge/arXiv-1910.00093-b31b1b.svg)](https://arxiv.org/abs/1910.00093) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/open-dynamic-robot-initiative/solo) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://open-dynamic-robot-initiative.github.io/)

- **[arXiv'24.05]** *Development of a Novel Impedance-Controlled Quasi-Direct-Drive Robotic Hand*  
  [![arXiv](https://img.shields.io/badge/arXiv-2405.18730-b31b1b.svg)](https://arxiv.org/abs/2405.18730)

- **[IEEE T-IE'22]** *Performance-Driven Cascade Controller Tuning With Bayesian Optimization*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1109/tie.2021.3050356) [![arXiv](https://img.shields.io/badge/arXiv-2007.12536-b31b1b.svg)](https://arxiv.org/abs/2007.12536)

##### Hydraulic Actuation

- **[Springer'19]** *The PETMAN and Atlas Robots at Boston Dynamics*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1007/978-94-007-6046-2_15) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://bostondynamics.com/atlas/)

- **[MED'20]** *Hybrid Position/Force Control for Hydraulic Actuators*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1109/MED48518.2020.9183305)

##### Pneumatic and Tendon-Driven Actuation

- **[JIMSS'12]** *Modelling of the McKibben artificial muscle: A review*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1177/1045389x11435435)

- **[Soft Robotics'24]** *A Comparison of Pneumatic Actuators for Soft Growing Vine Robots*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1089/soro.2023.0169)

- **[Annu. Rev. Control'19]** *A Century of Robotic Hands*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1146/annurev-control-060117-105003)

##### Compliant and Variable Stiffness / Impedance Actuation

- **[IROS'95]** *Series elastic actuators*  
  [![Paper](https://img.shields.io/badge/Paper-IROS-4B5D67.svg)](https://doi.org/10.1109/iros.1995.525827)

- **[arXiv'09.12]** *Modeling and Application of Series Elastic Actuators for Force Control Multi Legged Robots*  
  [![arXiv](https://img.shields.io/badge/arXiv-0912.3956-b31b1b.svg)](https://arxiv.org/abs/0912.3956)

- **[IEEE/ASME TMECH'26]** *Design and Control of a Compact Series Elastic Actuator Module for Robots in MRI Scanners*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1109/TMECH.2026.3658501) [![arXiv](https://img.shields.io/badge/arXiv-2406.07670-b31b1b.svg)](https://arxiv.org/abs/2406.07670)

- **[Robot. Auton. Syst.'13]** *Variable impedance actuators: A review*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1016/j.robot.2013.06.009)

- **[IEEE/ASME TMECH'23]** *Design and Control of a Novel Variable Stiffness Series Elastic Actuator*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1109/TMECH.2022.3232471)

- **[arXiv'19.06]** *A Dynamic Robotic Actuator with Variable Physical Stiffness and Damping*  
  [![arXiv](https://img.shields.io/badge/arXiv-1906.07669-b31b1b.svg)](https://arxiv.org/abs/1906.07669)

- **[arXiv'25.11]** *Safe and Optimal Variable Impedance Control via Certified Reinforcement Learning*  
  [![arXiv](https://img.shields.io/badge/arXiv-2511.16330-b31b1b.svg)](https://arxiv.org/abs/2511.16330)

##### Soft and Emerging Actuation

- **[arXiv'21.02]** *Hydraulically Amplified Self-Healing ELectrostatic (HASEL) Inspired Actuators*  
  [![arXiv](https://img.shields.io/badge/arXiv-2102.13039-b31b1b.svg)](https://arxiv.org/abs/2102.13039)

- **[Biomimetics'25]** *Review of Electrohydraulic Actuators Inspired by the HASEL Actuator*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.3390/biomimetics10030152)

- **[Mater. Des.'14]** *A review of shape memory alloy research, applications and opportunities*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1016/j.matdes.2013.11.084)

- **[npj Robotics'26]** *Advancing soft robotics: recent progress in dielectric elastomer and fluid actuators*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1038/s44182-026-00074-3)

- **[Soft Robotics'26]** *A Stiffness-Tunable Soft Actuator with Adjustable Jamming for Dexterous Manipulation*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1177/21695172251405996)

- **[arXiv'25.04]** *Unified Manipulability and Compliance Analysis of Modular Soft-Rigid Hybrid Fingers*  
  [![arXiv](https://img.shields.io/badge/arXiv-2504.13800-b31b1b.svg)](https://arxiv.org/abs/2504.13800)

<a id="end-effectors-and-grippers"></a>

#### End-Effectors and Grippers

- **[IJRR'10]** *The Highly Adaptive SDM Hand: Design and Performance Evaluation*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1177/0278364909360852)

- **[RSS'23]** *LEAP Hand: Low-Cost, Efficient, and Anthropomorphic Hand for Robot Learning*  
  [![Paper](https://img.shields.io/badge/Paper-RSS-4B5D67.svg)](https://doi.org/10.15607/RSS.2023.XIX.089) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/leap-hand/LEAP_Hand_API) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://leaphand.com/)

- **[Sci. Adv.'25]** *Biomimetic rigid-soft finger design for highly dexterous and adaptive robotic hands*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1126/sciadv.adu2018)

- **[Adv. Mater.'18]** *Soft Robotic Grippers*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1002/adma.201707035)

- **[Soft Robotics'26]** *Everything-Grasping Gripper: A Universal Gripper with Synergistic Suction–Grasping Capabilities for Cross-Scale and Cross-State Manipulation*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1177/21695172251400144)

- **[npj Robotics'26]** *Tactile-reactive gripper with an active palm for dexterous manipulation*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1038/s44182-026-00079-y) [![Demo](https://img.shields.io/badge/Demo-YouTube-FF0000.svg)](https://www.youtube.com/watch?v=C6EQ-J-9wrs)

- **[ICRA'25]** *PolyTouch: A Robust Multi-Modal Tactile Sensor for Contact-Rich Manipulation Using Tactile-Diffusion Policies*  
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)](https://doi.org/10.1109/icra55743.2025.11128816) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://polytouch.alanz.info/)

- **[arXiv'25.07]** *DexWrist: A Robotic Wrist for Constrained and Dynamic Manipulation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2507.01008-b31b1b.svg)](https://arxiv.org/abs/2507.01008) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://dexwrist.csail.mit.edu/)

- **[ICRA'25]** *D(R,O) Grasp: A Unified Representation of Robot and Object Interaction for Cross-Embodiment Dexterous Grasping*  
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)](https://doi.org/10.1109/icra55743.2025.11127754) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/zhenyuwei2003/DRO-Grasp) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://nus-lins-lab.github.io/drograspweb/)

- **[CVPR'25]** *DexGrasp Anything: Towards Universal Robotic Dexterous Grasping with Physics Awareness*  
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)](https://doi.org/10.1109/cvpr52734.2025.02103) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/4DVLab/DexGrasp-Anything) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://dexgraspanything.github.io/)

- **[CoRL'25]** *Robust Dexterous Grasping of General Objects*  
  [![Paper](https://img.shields.io/badge/Paper-CoRL-4B5D67.svg)](https://proceedings.mlr.press/v305/zhang25h.html) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/zdchan/robust_dexgrasp) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://zdchan.github.io/Robust_DexGrasp/)

- **[Nat. Commun.'26]** *Hand-like autonomous flying robot for airborne grasping and interaction*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1038/s41467-026-68967-3)

---

<a id="physical-control"></a>

### Physical Control

<a id="classical-and-optimization-based-control"></a>

#### Classical and Optimization-Based Control

- **[IEEE J. Robot. Autom.'87]** *A unified approach for motion and force control of robot manipulators: The operational space formulation*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1109/jra.1987.1087068)

- **[ASME JDSMC'85]** *Impedance Control: An Approach to Manipulation (Parts I–III)*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)]()

- **[IJRR'07]** *A Unified Passivity-based Control Framework for Position, Torque and Impedance Control of Flexible Joint Robots*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1177/0278364907073776)

- **[Springer LNCIS'09]** *Efficient Numerical Methods for Nonlinear MPC and Moving Horizon Estimation*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1007/978-3-642-01094-1_32)

- **[IEEE TAC'17]** *Control Barrier Function Based Quadratic Programs for Safety Critical Systems*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1109/tac.2016.2638961)

- **[arXiv'26.04]** *A Control Barrier Function-Constrained Model Predictive Control Framework for Safe Reinforcement Learning*  
  [![arXiv](https://img.shields.io/badge/arXiv-2604.06463-b31b1b.svg)](https://arxiv.org/abs/2604.06463)

<a id="learning-based-control-for-physical-embodiments"></a>

#### Learning-Based Control for Physical Embodiments

##### Reinforcement Learning for Feedback Control

- **[RSS'21]** *RMA: Rapid Motor Adaptation for Legged Robots*  
  [![Paper](https://img.shields.io/badge/Paper-RSS-4B5D67.svg)](https://www.roboticsproceedings.org/rss17/p011.html) [![arXiv](https://img.shields.io/badge/arXiv-2107.04034-b31b1b.svg)](https://arxiv.org/abs/2107.04034) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://ashish-kmr.github.io/rma-legged-robots/)

- **[ICRA'25]** *HOVER: Versatile Neural Whole-Body Controller for Humanoid Robots*  
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)](https://doi.org/10.1109/icra55743.2025.11128549) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/NVlabs/HOVER) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://hover-versatile-humanoid.github.io/)

- **[arXiv'18.08]** *Learning Dexterous In-Hand Manipulation*  
  [![arXiv](https://img.shields.io/badge/arXiv-1808.00177-b31b1b.svg)](https://arxiv.org/abs/1808.00177) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://openai.com/research/learning-dexterity/)

##### Imitation Learning and Behavior Cloning

- **[arXiv'24.05]** *Tilde: Teleoperation for Dexterous In-Hand Manipulation Learning with a DeltaHand*  
  [![arXiv](https://img.shields.io/badge/arXiv-2405.18804-b31b1b.svg)](https://arxiv.org/abs/2405.18804) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/iamlab-cmu/DeltaHands)

- **[ICRA'25]** *DexMimicGen: Automated Data Generation for Bimanual Dexterous Manipulation via Imitation Learning*  
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)](https://doi.org/10.1109/icra55743.2025.11127809) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/NVlabs/dexmimicgen) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://dexmimicgen.github.io/)

- **[Sci. Robot.'25]** *Precise and dexterous robotic manipulation via human-in-the-loop reinforcement learning*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1126/scirobotics.ads5033) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/rail-berkeley/hil-serl) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://hil-serl.github.io/)

##### Residual and Hybrid Learning

- **[ICRA'19]** *Residual Reinforcement Learning for Robot Control*  
  [![arXiv](https://img.shields.io/badge/arXiv-1812.03201-b31b1b.svg)](https://arxiv.org/abs/1812.03201)

- **[IROS'23]** *Real-Time Model-Free Deep Reinforcement Learning for Force Control of a Series Elastic Actuator*  
  [![Paper](https://img.shields.io/badge/Paper-IROS-4B5D67.svg)](https://doi.org/10.1109/IROS55552.2023.10341751) [![arXiv](https://img.shields.io/badge/arXiv-2304.04911-b31b1b.svg)](https://arxiv.org/abs/2304.04911)

##### Diffusion, Flow, and Action-Chunking Models

- **[NeurIPS'20]** *Denoising Diffusion Probabilistic Models*  
  [![Paper](https://img.shields.io/badge/Paper-NeurIPS-4B5D67.svg)](https://arxiv.org/abs/2006.11239) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/hojonathanho/diffusion) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://hojonathanho.github.io/diffusion/)

- **[ICLR'21]** *Denoising Diffusion Implicit Models*  
  [![Paper](https://img.shields.io/badge/Paper-ICLR-4B5D67.svg)](https://arxiv.org/abs/2010.02502) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/ermongroup/ddim)

- **[RSS'23]** *Diffusion Policy: Visuomotor Policy Learning via Action Diffusion*  
  [![Paper](https://img.shields.io/badge/Paper-RSS-4B5D67.svg)](https://doi.org/10.15607/rss.2023.xix.026) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/real-stanford/diffusion_policy) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://diffusion-policy.cs.columbia.edu/)

- **[RSS'23]** *Learning Fine-Grained Bimanual Manipulation with Low-Cost Hardware (ACT)*  
  [![Paper](https://img.shields.io/badge/Paper-RSS-4B5D67.svg)](https://doi.org/10.15607/RSS.2023.XIX.016) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/tonyzhaozh/act) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://tonyzhaozh.github.io/aloha/)

- **[ICLR'23]** *Flow Matching for Generative Modeling*  
  [![Paper](https://img.shields.io/badge/Paper-ICLR-4B5D67.svg)](https://arxiv.org/abs/2210.02747) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/atong01/conditional-flow-matching)

- **[arXiv'26.02]** *Action-to-Action Flow Matching*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.07322-b31b1b.svg)](https://arxiv.org/abs/2602.07322) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://lorenzo-0-0.github.io/A2A_Flow_Matching)

<a id="foundation-model-based-action-generation"></a>

#### Foundation-Model-Based Action Generation

- **[ICML'23]** *PaLM-E: An Embodied Multimodal Language Model*  
  [![Paper](https://img.shields.io/badge/Paper-ICML-4B5D67.svg)](https://proceedings.mlr.press/v202/driess23a.html) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://palm-e.github.io/)

- **[CoRL'23]** *RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control*  
  [![Paper](https://img.shields.io/badge/Paper-CoRL-4B5D67.svg)](https://proceedings.mlr.press/v229/brohan23a.html) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://robotics-transformer2.github.io/) [![Blog](https://img.shields.io/badge/Blog-DeepMind-0A66C2.svg)](https://deepmind.google/blog/rt-2-new-model-translates-vision-and-language-into-action/)

- **[arXiv'24.06]** *OpenVLA: An Open-Source Vision-Language-Action Model*  
  [![arXiv](https://img.shields.io/badge/arXiv-2406.09246-b31b1b.svg)](https://arxiv.org/abs/2406.09246) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/openvla/openvla) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://openvla.github.io/)

- **[arXiv'25.03]** *GR00T N1: An Open Foundation Model for Generalist Humanoid Robots*  
  [![arXiv](https://img.shields.io/badge/arXiv-2503.14734-b31b1b.svg)](https://arxiv.org/abs/2503.14734) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/NVIDIA/Isaac-GR00T)

- **[arXiv'25.11]** *π<sub>0.6</sub>: a VLA That Learns From Experience*  
  [![arXiv](https://img.shields.io/badge/arXiv-2511.14759-b31b1b.svg)](https://arxiv.org/abs/2511.14759) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/Physical-Intelligence/openpi) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://www.physicalintelligence.company/blog/pi06)

- **[arXiv'25.06]** *VLA-OS: Structuring and Dissecting Planning Representations and Paradigms in Vision-Language-Action Models*  
  [![arXiv](https://img.shields.io/badge/arXiv-2506.17561-b31b1b.svg)](https://arxiv.org/abs/2506.17561) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/HeegerGao/VLA-OS) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://nus-lins-lab.github.io/vlaos/)

- **[arXiv'26.02]** *Green-VLA: Staged Vision-Language-Action Model for Generalist Robots*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.00919-b31b1b.svg)](https://arxiv.org/abs/2602.00919) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/greenvla/GreenVLA) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://greenvla.github.io/)

- **[arXiv'26.03]** *RoboForge: Physically Optimized Text-guided Whole-Body Locomotion for Humanoids*  
  [![arXiv](https://img.shields.io/badge/arXiv-2603.17927-b31b1b.svg)](https://arxiv.org/abs/2603.17927) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://theroboforge.github.io/)

---

<a id="closed-loop-execution-and-interaction"></a>

### Closed-Loop Execution and Interaction

<a id="locomotion-and-navigation"></a>

#### Locomotion and Navigation

##### Legged Locomotion

- **[Sci. Robot.'20]** *Learning quadrupedal locomotion over challenging terrain*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1126/scirobotics.abc5986) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/leggedrobotics/learning_quadrupedal_locomotion_over_challenging_terrain_supplementary)

- **[Sci. Robot.'22]** *Learning robust perceptive locomotion for quadrupedal robots in the wild*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1126/scirobotics.abk2822) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://leggedrobotics.github.io/rl-perceptiveloco/)

- **[RSS'25]** *ASAP: Aligning Simulation and Real-World Physics for Learning Agile Humanoid Whole-Body Skills*  
  [![Paper](https://img.shields.io/badge/Paper-RSS-4B5D67.svg)](https://roboticsconference.org/program/papers/66/) [![arXiv](https://img.shields.io/badge/arXiv-2502.01143-b31b1b.svg)](https://arxiv.org/abs/2502.01143) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/LeCAR-Lab/ASAP) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://agile.human2humanoid.com/)

- **[IROS'25]** *Humanoid Whole-Body Locomotion on Narrow Terrain via Dynamic Balance and Reinforcement Learning*  
  [![Paper](https://img.shields.io/badge/Paper-IROS-4B5D67.svg)]() [![arXiv](https://img.shields.io/badge/arXiv-2502.17219-b31b1b.svg)](https://arxiv.org/abs/2502.17219) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://whole-body-loco.github.io/)

##### Wheeled and Mobile Navigation

- **[IROS'20]** *The Marathon 2: A Navigation System*  
  [![Paper](https://img.shields.io/badge/Paper-IROS-4B5D67.svg)](https://doi.org/10.1109/IROS45743.2020.9341207) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/ros-navigation/navigation2)

- **[ICRA'21]** *RelMoGen: Leveraging Motion Generation in Reinforcement Learning for Mobile Manipulation*  
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)](https://doi.org/10.1109/ICRA48506.2021.9561315) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://svl.stanford.edu/projects/relmogen/)

<a id="manipulation-and-grasping"></a>

#### Manipulation and Grasping

##### Grasp Planning

- **[ICRA'00]** *Robotic Grasping and Contact: A Review*  
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)]()

- **[CVPR'20]** *GraspNet-1Billion: A Large-Scale Benchmark for General Object Grasping*  
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)](https://doi.org/10.1109/cvpr42600.2020.01146) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/graspnet/graspnet-baseline) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://graspnet.net/)

- **[ICRA'21]** *Contact-GraspNet: Efficient 6-DoF Grasp Generation in Cluttered Scenes*  
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)](https://doi.org/10.1109/icra48506.2021.9561877) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/NVlabs/contact_graspnet)

##### Dexterous and In-Hand Manipulation

- **[arXiv'19.10]** *Solving Rubik's Cube with a Robot Hand*  
  [![arXiv](https://img.shields.io/badge/arXiv-1910.07113-b31b1b.svg)](https://arxiv.org/abs/1910.07113) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://openai.com/research/solving-rubiks-cube)

- **[CoRL'25]** *Reasoning Grasping via Multimodal Large Language Model*  
  [![Paper](https://img.shields.io/badge/Paper-CoRL-4B5D67.svg)](https://proceedings.mlr.press/v270/jin25a.html) [![arXiv](https://img.shields.io/badge/arXiv-2402.06798-b31b1b.svg)](https://arxiv.org/abs/2402.06798)

##### Bimanual Manipulation

- **[CVPR'25]** *ManipTrans: Efficient Dexterous Bimanual Manipulation Transfer via Residual Learning*  
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)](https://doi.org/10.1109/cvpr52734.2025.00656) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/ManipTrans/ManipTrans) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://maniptrans.github.io/)

<a id="physical-humanrobot-interaction-and-collaboration"></a>

#### Physical Human–Robot Interaction and Collaboration

- **[IJIDeM'25]** *Safe physical human–robot interaction through variable impedance control based on ISO/TS 15066*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1007/s12008-024-02074-9)

- **[ICORR'23]** *Comparison of Admittance Control Dynamic Models for Transparent Free-Motion Human-Robot Interaction*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1109/icorr58425.2023.10304709)

- **[IEEE Access'25]** *A Cooperation Control Framework Based on Admittance Control and Time-Varying Passive Velocity Field Control for Human-Robot Co-Carrying Tasks*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)]()

- **[IEEE/ASME TMECH'25]** *Musculoskeletal Model-Based Adaptive Variable Impedance Control With Flexible Prescribed Performance for Rehabilitation Robots*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1109/tmech.2025.3562670)

- **[arXiv'26.01]** *Physical Human-Robot Interaction: A Critical Review of Safety Constraints*  
  [![arXiv](https://img.shields.io/badge/arXiv-2601.19462-b31b1b.svg)](https://arxiv.org/abs/2601.19462)

- **[ICLR'26]** *REI-Bench: Can Embodied Agents Understand Vague Human Instructions in Task Planning?*  
  [![Paper](https://img.shields.io/badge/Paper-ICLR-4B5D67.svg)](https://arxiv.org/abs/2505.10872) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://jcx0110.github.io/rei-bench-project)

- **[CVPR'26]** *When Robots Should Say "I Don't Know": Benchmarking Abstention in Embodied Question Answering*  
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)](https://arxiv.org/abs/2512.04597) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://abstaineqa.github.io/)

<a id="active-perception-and-environment-exploration"></a>

#### Active Perception and Environment Exploration

- **[IROS'23]** *Push to know! - Visuo-tactile based active object parameter inference with dual differentiable filtering*  
  [![Paper](https://img.shields.io/badge/Paper-IROS-4B5D67.svg)]()

- **[IEEE T-RO'25]** *Predictive visuo-tactile interactive perception framework for object properties inference*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)]()

- **[CoRL'23]** *Leveraging 3D Reconstruction for Mechanical Search on Cluttered Shelves*  
  [![Paper](https://img.shields.io/badge/Paper-CoRL-4B5D67.svg)](https://proceedings.mlr.press/v229/kim23a.html) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/seungyeon-k/Search-for-Grasp-public)

- **[CVPR'24]** *OpenEQA: Embodied Question Answering in the Era of Foundation Models*  
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)](https://doi.org/10.1109/cvpr52733.2024.01560) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/facebookresearch/open-eqa)

- **[arXiv'26.02]** *AnyTouch 2: General Optical Tactile Representation Learning For Dynamic Tactile Perception*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.09617-b31b1b.svg)](https://arxiv.org/abs/2602.09617) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/GeWu-Lab/AnyTouch2)

<a id="language-conditioned-and-human-in-the-loop-execution"></a>

#### Language-Conditioned and Human-in-the-Loop Execution

- **[RSS'24]** *Octo: An Open-Source Generalist Robot Policy*  
  [![Paper](https://img.shields.io/badge/Paper-RSS-4B5D67.svg)]() [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/octo-models/octo) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://octo-models.github.io/)

- **[IEEE/ASME TMECH'25]** *Aligning Cyber Space With Physical World: A Comprehensive Survey on Embodied AI*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1109/tmech.2025.3574943) [![arXiv](https://img.shields.io/badge/arXiv-2407.06886-b31b1b.svg)](https://arxiv.org/abs/2407.06886) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/HCPLab-SYSU/Embodied_AI_Paper_List)

