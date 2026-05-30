<a id="4-physical-cognition-in-pai"></a>

# 4. Physical Cognition in PAI


<a id="table-of-contents"></a>

## Table of Contents

- [Physical Cognition](#physical-cognition)
  - [State Representation and Abstraction](#state-representation-and-abstraction)
    - [State Abstraction](#state-abstraction)
    - [Structured World Representations](#structured-world-representations)
  - [World Models](#world-models)
  - [Reasoning and Planning](#reasoning-and-planning)
    - [Task Specification and Problem Formulation](#task-specification-and-problem-formulation)
    - [Motion Planning](#motion-planning)
    - [Vision-Language-Action and Action Representations](#vision-language-action-and-action-representations)
    - [Computational Brain Models](#computational-brain-models)
  - [Memory](#memory)
    - [Short-Term Memory](#short-term-memory)
    - [Long-Term Memory](#long-term-memory)
  - [Alignment](#alignment)
    - [Alignment with Physical World](#alignment-with-physical-world)
    - [Alignment with Human Value](#alignment-with-human-value)
  - [Future Directions](#future-directions)

---

<a id="physical-cognition"></a>

### Physical Cognition

- **[arXiv'25.01]** *Physical AI Agents: Integrating Cognitive Intelligence with Real-World Action*  
  [![arXiv](https://img.shields.io/badge/arXiv-2501.08944-b31b1b.svg)](https://arxiv.org/abs/2501.08944)

- **[arXiv'25.10]** *Aligning Perception, Reasoning, Modeling and Interaction: A Survey on Physical AI*  
  [![arXiv](https://img.shields.io/badge/arXiv-2510.04978-b31b1b.svg)](https://arxiv.org/abs/2510.04978) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/AI4Phys/Awesome-AI-for-Physics)

- **[arXiv'25.07]** *A Survey: Learning Embodied Intelligence from Physical Simulators and World Models*  
  [![arXiv](https://img.shields.io/badge/arXiv-2507.00917-b31b1b.svg)](https://arxiv.org/abs/2507.00917) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/NJU3DV-LoongGroup/Embodied-World-Models-Survey)

- **[arXiv'25.03]** *World Models in Artificial Intelligence: Sensing, Learning, and Reasoning Like a Child*  
  [![arXiv](https://img.shields.io/badge/arXiv-2503.15168-b31b1b.svg)](https://arxiv.org/abs/2503.15168)

<a id="state-representation-and-abstraction"></a>

#### State Representation and Abstraction

<a id="state-abstraction"></a>

##### State Abstraction

- **[ICML'19]** *Learning Latent Dynamics for Planning from Pixels (PlaNet)*  
  [![Paper](https://img.shields.io/badge/Paper-ICML-4B5D67.svg)](https://proceedings.mlr.press/v97/hafner19a.html) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/google-research/planet) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://planetrl.github.io/)

- **[ICLR'20]** *Dream to Control: Learning Behaviors by Latent Imagination (Dreamer)*  
  [![Paper](https://img.shields.io/badge/Paper-ICLR-4B5D67.svg)](https://openreview.net/forum?id=S1lOTC4tDS) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/google-research/dreamer) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://dreamrl.github.io/)

- **[ICML'20]** *CURL: Contrastive Unsupervised Representations for Reinforcement Learning*  
  [![Paper](https://img.shields.io/badge/Paper-ICML-4B5D67.svg)](https://proceedings.mlr.press/v119/laskin20a.html) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/MishaLaskin/curl) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://mishalaskin.github.io/curl/)

- **[ICML'21]** *Learning Transferable Visual Models From Natural Language Supervision (CLIP)*  
  [![Paper](https://img.shields.io/badge/Paper-ICML-4B5D67.svg)](https://proceedings.mlr.press/v139/radford21a.html) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/openai/CLIP)

- **[CVPR'23]** *Self-Supervised Learning from Images with a Joint-Embedding Predictive Architecture (I-JEPA)*  
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)](https://doi.org/10.1109/cvpr52729.2023.01499) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/facebookresearch/ijepa)

- **[CVPR'20]** *VectorNet: Encoding HD Maps and Agent Dynamics From Vectorized Representation*  
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)](https://doi.org/10.1109/cvpr42600.2020.01154)

- **[CVPR'21]** *MP3: A Unified Model to Map, Perceive, Predict and Plan*  
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)](https://doi.org/10.1109/cvpr46437.2021.01417) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://sergiocasas.github.io/publication/mp3/)

- **[CoRL'23]** *VoxPoser: Composable 3D Value Maps for Robotic Manipulation with Language Models*  
  [![Paper](https://img.shields.io/badge/Paper-CoRL-4B5D67.svg)](https://proceedings.mlr.press/v229/huang23b.html) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/huangwl18/VoxPoser) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://voxposer.github.io/)

<a id="structured-world-representations"></a>

##### Structured World Representations

- **[ECCV'22]** *BEVFormer: Learning Bird's-Eye-View Representation from Multi-Camera Images via Spatiotemporal Transformers*  
  [![Paper](https://img.shields.io/badge/Paper-ECCV-4B5D67.svg)](https://doi.org/10.1007/978-3-031-20077-9_1) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/fundamentalvision/BEVFormer)

- **[CVPR'23]** *Implicit Occupancy Flow Fields for Perception and Prediction in Self-Driving*  
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)](https://doi.org/10.1109/CVPR52729.2023.00139) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://waabi.ai/research/implicito)

- **[ECCV'24]** *OccWorld: Learning a 3D Occupancy World Model for Autonomous Driving*  
  [![Paper](https://img.shields.io/badge/Paper-ECCV-4B5D67.svg)](https://doi.org/10.1007/978-3-031-72624-8_4) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/wzzheng/OccWorld) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://wzzheng.net/OccWorld/)

<a id="world-models"></a>

### World Models

**Foundations and Surveys**

- **[ACM CSUR'26]** *Understanding World or Predicting Future? A Comprehensive Survey of World Models*  
  [![Paper](https://img.shields.io/badge/Paper-ACM%20CSUR-4B5D67.svg)](https://doi.org/10.1145/3746449) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/tsinghua-fib-lab/World-Model)

- **[NeurIPS'18]** *Recurrent World Models Facilitate Policy Evolution*  
  [![Paper](https://img.shields.io/badge/Paper-NeurIPS-4B5D67.svg)](https://proceedings.neurips.cc/paper/2018/hash/2de5d16682c3c35007e4e92982f1a2ba-Abstract.html) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/hardmaru/WorldModelsExperiments) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://worldmodels.github.io/)

- **[OpenReview'22]** *A Path Towards Autonomous Machine Intelligence*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://openreview.net/forum?id=BZ5a1r-kVsf)

**Latent Predictive World Models**

- **[ICML'19]** *Learning Latent Dynamics for Planning from Pixels (PlaNet)*  
  [![Paper](https://img.shields.io/badge/Paper-ICML-4B5D67.svg)](https://proceedings.mlr.press/v97/hafner19a.html) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/google-research/planet) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://planetrl.github.io/)

- **[ICLR'20]** *Dream to Control: Learning Behaviors by Latent Imagination (Dreamer)*  
  [![Paper](https://img.shields.io/badge/Paper-ICLR-4B5D67.svg)](https://openreview.net/forum?id=S1lOTC4tDS) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/google-research/dreamer) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://dreamrl.github.io/)

- **[CoRL'22]** *DayDreamer: World Models for Physical Robot Learning*  
  [![Paper](https://img.shields.io/badge/Paper-CoRL-4B5D67.svg)](https://proceedings.mlr.press/v205/wu23c.html) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/danijar/daydreamer) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://www.escontrela.me/daydreamer/)

- **[CVPR'23]** *Self-Supervised Learning from Images with a Joint-Embedding Predictive Architecture (I-JEPA)*  
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)](https://doi.org/10.1109/cvpr52729.2023.01499) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/facebookresearch/ijepa)

- **[TMLR'24]** *Revisiting Feature Prediction for Learning Visual Representations from Video (V-JEPA)*  
  [![Paper](https://img.shields.io/badge/Paper-TMLR-4B5D67.svg)](https://openreview.net/forum?id=QaCCuDfBk2) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/facebookresearch/jepa)

- **[arXiv'25.06]** *V-JEPA 2: Self-Supervised Video Models Enable Understanding, Prediction and Planning*  
  [![arXiv](https://img.shields.io/badge/arXiv-2506.09985-b31b1b.svg)](https://arxiv.org/abs/2506.09985) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/facebookresearch/vjepa2) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://ai.meta.com/research/vjepa/)

**Generative and Interactive World Models**

- **[Tech Report'24]** *Video Generation Models as World Simulators*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://openai.com/index/video-generation-models-as-world-simulators/)

- **[ICML'24]** *Genie: Generative Interactive Environments*  
  [![Paper](https://img.shields.io/badge/Paper-ICML-4B5D67.svg)](https://proceedings.mlr.press/v235/bruce24a.html) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://sites.google.com/view/genie-2024/home)

- **[ICLR'25]** *Diffusion Models Are Real-Time Game Engines*  
  [![Paper](https://img.shields.io/badge/Paper-ICLR-4B5D67.svg)](https://openreview.net/forum?id=P8pqeEkn1H) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://gamengen.github.io/)

- **[arXiv'23.09]** *GAIA-1: A Generative World Model for Autonomous Driving*  
  [![arXiv](https://img.shields.io/badge/arXiv-2309.17080-b31b1b.svg)](https://arxiv.org/abs/2309.17080) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://anthonyhu.github.io/gaia1)

- **[ECCV'24]** *DriveDreamer: Towards Real-world-driven World Models for Autonomous Driving*  
  [![Paper](https://img.shields.io/badge/Paper-ECCV-4B5D67.svg)](https://doi.org/10.1007/978-3-031-73195-2_4) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/JeffWang987/DriveDreamer) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://drivedreamer.github.io/)

- **[arXiv'25.01]** *Cosmos World Foundation Model Platform for Physical AI*  
  [![arXiv](https://img.shields.io/badge/arXiv-2501.03575-b31b1b.svg)](https://arxiv.org/abs/2501.03575) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/nvidia-cosmos) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://www.nvidia.com/en-us/ai/cosmos/)

**Geometric and Structured World Models**

- **[ECCV'24]** *OccWorld: Learning a 3D Occupancy World Model for Autonomous Driving*  
  [![Paper](https://img.shields.io/badge/Paper-ECCV-4B5D67.svg)](https://doi.org/10.1007/978-3-031-72624-8_4) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/wzzheng/OccWorld) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://wzzheng.net/OccWorld/)

- **[AAAI'25]** *Driving in the Occupancy World: Vision-Centric 4D Occupancy Forecasting and Planning via World Models for Autonomous Driving (Drive-OccWorld)*  
  [![Paper](https://img.shields.io/badge/Paper-AAAI-4B5D67.svg)](https://doi.org/10.1609/aaai.v39i9.33230) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/yuyang-cloud/Drive-OccWorld) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://drive-occworld.github.io/)

- **[arXiv'25.05]** *Occupancy World Model for Robots (RoboOccWorld)*  
  [![arXiv](https://img.shields.io/badge/arXiv-2505.05512-b31b1b.svg)](https://arxiv.org/abs/2505.05512)

- **[ICML'24]** *3D-VLA: A 3D Vision-Language-Action Generative World Model*  
  [![Paper](https://img.shields.io/badge/Paper-ICML-4B5D67.svg)](https://proceedings.mlr.press/v235/zhen24a.html) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/UMass-Embodied-AGI/3D-VLA) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://vis-www.cs.umass.edu/3dvla/)

<a id="reasoning-and-planning"></a>

### Reasoning and Planning

<a id="task-specification-and-problem-formulation"></a>

#### Task Specification and Problem Formulation

- **[AI'71]** *STRIPS: A New Approach to the Application of Theorem Proving to Problem Solving*  
  [![Paper](https://img.shields.io/badge/Paper-AI-4B5D67.svg)](https://doi.org/10.1016/0004-3702(71)90010-5)

- **[Book'06]** *Planning Algorithms*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](http://planning.cs.uiuc.edu/)

- **[AI'98]** *Planning and Acting in Partially Observable Stochastic Domains*  
  [![Paper](https://img.shields.io/badge/Paper-AI-4B5D67.svg)](https://doi.org/10.1016/S0004-3702(98)00023-X)

- **[CoRL'22]** *Do As I Can, Not As I Say: Grounding Language in Robotic Affordances (SayCan)*  
  [![Paper](https://img.shields.io/badge/Paper-CoRL-4B5D67.svg)](https://proceedings.mlr.press/v205/ichter23a.html) [![arXiv](https://img.shields.io/badge/arXiv-2204.01691-b31b1b.svg)](https://arxiv.org/abs/2204.01691) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/google-research/google-research/tree/master/saycan) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://say-can.github.io/)

- **[CoRL'23]** *VoxPoser: Composable 3D Value Maps for Robotic Manipulation with Language Models*  
  [![Paper](https://img.shields.io/badge/Paper-CoRL-4B5D67.svg)](https://proceedings.mlr.press/v229/huang23b.html) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/huangwl18/VoxPoser) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://voxposer.github.io/)

- **[Annu. Rev. Control Robot. Auton. Syst.'21]** *Integrated Task and Motion Planning*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1146/annurev-control-091420-084139)

<a id="motion-planning"></a>

#### Motion Planning

**Sampling-Based Planning**

- **[Tech Report'98]** *Rapidly-Exploring Random Trees: A New Tool for Path Planning (RRT)*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://msl.cs.uiuc.edu/~lavalle/papers/Lav98c.pdf)

- **[IJRR'11]** *Sampling-Based Algorithms for Optimal Motion Planning (RRT\*)*  
  [![Paper](https://img.shields.io/badge/Paper-IJRR-4B5D67.svg)](https://doi.org/10.1177/0278364911406761)

- **[T-RA'96]** *Probabilistic Roadmaps for Path Planning in High-Dimensional Configuration Spaces (PRM)*  
  [![Paper](https://img.shields.io/badge/Paper-IEEE-4B5D67.svg)](https://doi.org/10.1109/70.508439)

- **[JOSER'14]** *Reducing the Barrier to Entry of Complex Robotic Software: A MoveIt! Case Study*  
  [![Paper](https://img.shields.io/badge/Paper-JOSER-4B5D67.svg)](https://doi.org/10.6092/JOSER_2014_05_01_p3) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/moveit/moveit)

**Optimization-Based Planning**

- **[ICRA'09]** *CHOMP: Gradient Optimization Techniques for Efficient Motion Planning*  
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)](https://doi.org/10.1109/ROBOT.2009.5152817)

- **[IJRR'14]** *Motion Planning with Sequential Convex Optimization and Convex Collision Checking (TrajOpt)*  
  [![Paper](https://img.shields.io/badge/Paper-IJRR-4B5D67.svg)](https://doi.org/10.1177/0278364914528132) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/joschu/trajopt) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://rll.berkeley.edu/trajopt/ijrr/)

- **[RSS'18]** *Differentiable Physics and Stable Modes for Tool-Use and Manipulation Planning*  
  [![Paper](https://img.shields.io/badge/Paper-RSS-4B5D67.svg)](https://doi.org/10.15607/rss.2018.xiv.044) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/MarcToussaint/18-RSS-PhysicalManipulation)

**Task-and-Motion Planning**

- **[Annu. Rev. Control Robot. Auton. Syst.'21]** *Integrated Task and Motion Planning*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://doi.org/10.1146/annurev-control-091420-084139)

- **[ICAPS'20]** *PDDLStream: Integrating Symbolic Planners and Blackbox Samplers via Optimistic Adaptive Planning*  
  [![Paper](https://img.shields.io/badge/Paper-ICAPS-4B5D67.svg)](https://doi.org/10.1609/ICAPS.V30I1.6739) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/caelan/pddlstream)

- **[RSS'20]** *Deep Visual Reasoning: Learning to Predict Action Sequences for Task and Motion Planning from an Initial Scene Image*  
  [![Paper](https://img.shields.io/badge/Paper-RSS-4B5D67.svg)](https://doi.org/10.15607/rss.2020.xvi.003)

- **[CoRL'22]** *Inner Monologue: Embodied Reasoning through Planning with Language Models*  
  [![Paper](https://img.shields.io/badge/Paper-CoRL-4B5D67.svg)](https://proceedings.mlr.press/v205/huang23c.html) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://innermonologue.github.io/)

- **[IJRR'25]** *LLM-GROP: Visually Grounded Robot Task and Motion Planning with Large Language Models*  
  [![Paper](https://img.shields.io/badge/Paper-IJRR-4B5D67.svg)](https://doi.org/10.1177/02783649251378196) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/bu-air-lab/llm-grop)

- **[ICRA'26]** *Manual2Skill++: Connector-Aware General Robotic Assembly from Instruction Manuals via Vision-Language Models*  
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)](https://arxiv.org/abs/2510.16344) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://nus-lins-lab.github.io/Manual2SkillPP/)

**Learning-Based Motion Planning**

- **[ICRA'19]** *Motion Planning Networks*  
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)](https://doi.org/10.1109/ICRA.2019.8793889) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/ahq1993/MPNet) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://sites.google.com/view/mpnet/home)

- **[ICML'22]** *Planning with Diffusion for Flexible Behavior Synthesis (Diffuser)*  
  [![Paper](https://img.shields.io/badge/Paper-ICML-4B5D67.svg)](https://proceedings.mlr.press/v162/janner22a.html) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/jannerm/diffuser) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://diffusion-planning.github.io/)

- **[ICRA'21]** *RelMoGen: Leveraging Motion Generation in Reinforcement Learning for Mobile Manipulation*  
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)](https://ieeexplore.ieee.org/document/9561234) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://svl.stanford.edu/projects/relmogen/)

- **[ICRA'25]** *PRESTO: Fast Motion Planning Using Diffusion Models Based on Key-Configuration Environment Representation*  
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)](https://doi.org/10.1109/ICRA55743.2025.11128590) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/kiwi-sherbet/PRESTO) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://kiwi-sherbet.github.io/PRESTO/)

- **[IROS'25]** *RRT\*former: Environment-Aware Sampling-Based Motion Planning using Transformer*  
  [![Paper](https://img.shields.io/badge/Paper-IROS-4B5D67.svg)](https://arxiv.org/abs/2511.15414) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/fengmingyang666/RRTformer)

- **[arXiv'25.04]** *SafeFlow: Safe Robot Motion Planning with Flow Matching via Control Barrier Functions*  
  [![arXiv](https://img.shields.io/badge/arXiv-2504.08661-b31b1b.svg)](https://arxiv.org/abs/2504.08661) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/SafeFlowMatching/SafeFlow) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://safeflowmatching.github.io/)

- **[CoRL'25]** *ManiFlow: A General Robot Manipulation Policy via Consistency Flow Training*  
  [![Paper](https://img.shields.io/badge/Paper-CoRL-4B5D67.svg)](https://openreview.net/forum?id=a6I9P5V6u7) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/geyan21/ManiFlow_Policy) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://maniflow-policy.github.io/)

- **[Front. Robot. AI'26]** *FRMD: Fast Robot Motion Diffusion via Trajectory-Level Consistency Distillation*  
  [![Paper](https://img.shields.io/badge/Paper-Frontiers-4B5D67.svg)](https://doi.org/10.3389/frobt.2026.1751688)


#### Vision-Language-Action and Action Representations

- **[NeurIPS'24]** *RoboMamba: Efficient Vision-Language-Action Model for Robotic Reasoning and Manipulation*  
  [![Paper](https://img.shields.io/badge/Paper-NeurIPS-4B5D67.svg)](https://proceedings.neurips.cc/paper_files/paper/2024/hash/4e6f6cbc4c1f6c7c2f3a3a3c0a2cb6bf-Abstract-Conference.html)
  [![arXiv](https://img.shields.io/badge/arXiv-2406.04339-b31b1b.svg)](https://arxiv.org/abs/2406.04339)  

- **[NeurIPS'24]** *BricksRL: A Platform for Democratizing Robotics and Reinforcement Learning Research and Education with LEGO*  
  [![Paper](https://img.shields.io/badge/Paper-NeurIPS-4B5D67.svg)](https://proceedings.neurips.cc/paper_files/paper/2024)
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

- **[arXiv'25.11]** *π*₀.₆: a VLA That Learns From Experience*  
  [![arXiv](https://img.shields.io/badge/arXiv-2511.14759-b31b1b.svg)](https://arxiv.org/abs/2511.14759)  

- **[arXiv'25.03]** *GR00T N1: An Open Foundation Model for Generalist Humanoid Robots*  
  [![arXiv](https://img.shields.io/badge/arXiv-2503.14734-b31b1b.svg)](https://arxiv.org/abs/2503.14734)  

- **[arXiv'25.11]** *Alpamayo-R1: Bridging Reasoning and Action Prediction for Generalizable Autonomous Driving in the Long Tail*  
  [![arXiv](https://img.shields.io/badge/arXiv-2511.00088-b31b1b.svg)](https://arxiv.org/abs/2511.00088)  

- **[RSS'23]** *Diffusion Policy: Visuomotor Policy Learning via Action Diffusion*  
  [![Paper](https://img.shields.io/badge/Paper-RSS-4B5D67.svg)](https://doi.org/10.15607/rss.2023.xix.026)  

- **[arXiv'26.02]** *Action-to-Action Flow Matching*  
  [![arXiv](https://img.shields.io/badge/arXiv-2602.07322-b31b1b.svg)](https://arxiv.org/abs/2602.07322)  

- **[RSS'23]** *Learning Fine-Grained Bimanual Manipulation with Low-Cost Hardware (ACT)*  
  [![Paper](https://img.shields.io/badge/Paper-RSS-4B5D67.svg)](https://doi.org/10.15607/RSS.2023.XIX.016)  

- **[arXiv'25.01]** *FAST: Efficient Action Tokenization for Vision-Language-Action Models*  
  [![arXiv](https://img.shields.io/badge/arXiv-2501.09747-b31b1b.svg)](https://arxiv.org/abs/2501.09747)  

- **[arXiv'24.05]** *A Survey on Vision-Language-Action Models for Embodied AI*  
  [![arXiv](https://img.shields.io/badge/arXiv-2405.14093-b31b1b.svg)](https://arxiv.org/abs/2405.14093)  

<a id="computational-brain-models"></a>

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

- **[PLOS Biology'19]** *The Human Brain Project—Synergy between neuroscience, computing, informatics, and brain-inspired technologies*  
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

- **[Information Fusion'25]** *AI Agents vs. Agentic AI: A Conceptual Taxonomy, Applications and Challenges*  
  [![Paper](https://img.shields.io/badge/Paper-Information%20Fusion-4B5D67.svg)](https://doi.org/10.1016/j.inffus.2025.103599)  

- **[TOIS'25]** *A Survey on the Memory Mechanism of Large Language Model-based Agents*  
  [![Paper](https://img.shields.io/badge/Paper-TOIS-4B5D67.svg)](https://doi.org/10.1145/3748302) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/nuster1128/LLM_Agent_Memory_Survey)  

- **[arXiv'25.07]** *State and Memory is All You Need for Robust and Reliable AI Agents*  
  [![arXiv](https://img.shields.io/badge/arXiv-2507.00081-b31b1b.svg)](https://arxiv.org/abs/2507.00081)  

- **[Blog'25]** *What is the Role of Memory in Agentic AI Systems? Unlocking Smarter, Human-Like Intelligence*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://datasciencedojo.com/blog/what-is-the-role-of-memory-in-agentic-ai/)  

- **[PLOS ONE'21]** *Embodied Working Memory During Ongoing Input Streams*  
  [![Paper](https://img.shields.io/badge/Paper-PLOS%20ONE-4B5D67.svg)](https://doi.org/10.1371/journal.pone.0244822)  

- **[HRI'25]** *From Interaction to Relationship: The Role of Memory, Learning, and Emotional Intelligence in AI-Embodied Human Engagement*  
  [![Paper](https://img.shields.io/badge/Paper-HRI-4B5D67.svg)](https://doi.org/10.1109/hri61500.2025.10973813)  

- **[OUP'25]** *Memory, Space, and Planning: Multiscale Predictive Representations*  
  [![Paper](https://img.shields.io/badge/Paper-OUP-4B5D67.svg)](https://arxiv.org/abs/2401.09491)  

- **[Humanoids'24]** *Robots Can Multitask Too: Integrating a Memory Architecture and LLMs for Enhanced Cross-Task Robot Action Generation*  
  [![Paper](https://img.shields.io/badge/Paper-Humanoids-4B5D67.svg)](https://doi.org/10.1109/humanoids58906.2024.10769803)  

- **[Nat. Mach. Intell.'25]** *Embodied Large Language Models Enable Robots to Complete Complex Tasks in Unpredictable Environments*  
  [![Paper](https://img.shields.io/badge/Paper-Nat.%20Mach.%20Intell.-4B5D67.svg)](https://doi.org/10.1038/s42256-025-01005-x) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/ruaridhmon/ELLMER)  

- **[F1000Research'25]** *A Review of Agentic AI in Cybersecurity: Cognitive Autonomy, Ethical Governance, and Quantum-Resilient Defense*  
  [![Paper](https://img.shields.io/badge/Paper-F1000Research-4B5D67.svg)](https://doi.org/10.12688/f1000research.169337.1)  

- **[Future Internet'25]** *The Rise of Agentic AI: A Review of Definitions, Frameworks, Architectures, Applications, Evaluation Metrics, and Challenges*  
  [![Paper](https://img.shields.io/badge/Paper-Future%20Internet-4B5D67.svg)](https://doi.org/10.3390/fi17090404)  

<a id="short-term-memory"></a>

#### Short-Term Memory

- **[Psych. Bull.'18]** *Benchmarks for Models of Short-Term and Working Memory*  
  [![Paper](https://img.shields.io/badge/Paper-Psych.%20Bull.-4B5D67.svg)](https://doi.org/10.1037/bul0000153)  

- **[Front. Comput. Neurosci.'24]** *Design and Evaluation of a Global Workspace Agent Embodied in a Realistic Multimodal Environment*  
  [![Paper](https://img.shields.io/badge/Paper-Front.%20Comput.%20Neurosci.-4B5D67.svg)](https://doi.org/10.3389/fncom.2024.1352685) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/arayabrain/multimodal-global-workspace-agent)  

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

<a id="long-term-memory"></a>

#### Long-Term Memory

- **[arXiv'24.11]** *Human-Inspired Perspectives: A Survey on AI Long-Term Memory*  
  [![arXiv](https://img.shields.io/badge/arXiv-2411.00489-b31b1b.svg)](https://arxiv.org/abs/2411.00489)  

- **[Neural Networks'19]** *Continual Lifelong Learning with Neural Networks: A Review*  
  [![Paper](https://img.shields.io/badge/Paper-Neural%20Networks-4B5D67.svg)](https://doi.org/10.1016/j.neunet.2019.01.012)  

- **[arXiv'25.04]** *Personalized Artificial General Intelligence (AGI) via Neuroscience-Inspired Continuous Learning Systems*  
  [![arXiv](https://img.shields.io/badge/arXiv-2504.20109-b31b1b.svg)](https://arxiv.org/abs/2504.20109)  

- **[Nat. Commun.'25]** *Hybrid Neural Networks for Continual Learning Inspired by Corticohippocampal Circuits*  
  [![Paper](https://img.shields.io/badge/Paper-Nat.%20Commun.-4B5D67.svg)](https://doi.org/10.1038/s41467-025-56405-9) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/qqish/CH-HNN)  

<a id="episodic-memory"></a>

##### Episodic Memory

- **[Cognition'21]** *Early Is Left and Up: Saccadic Responses Reveal Horizontal and Vertical Spatial Associations of Serial Order in Working Memory*  
  [![Paper](https://img.shields.io/badge/Paper-Cognition-4B5D67.svg)](https://doi.org/10.1016/j.cognition.2021.104908)  

- **[arXiv'20.05]** *A Proposal for Intelligent Agents with Episodic Memory*  
  [![arXiv](https://img.shields.io/badge/arXiv-2005.03182-b31b1b.svg)](https://arxiv.org/abs/2005.03182)  

- **[NCA'23]** *Explainable Reinforcement Learning for Broad-XAI: A Conceptual Framework and Survey*  
  [![Paper](https://img.shields.io/badge/Paper-NCA-4B5D67.svg)](https://doi.org/10.1007/s00521-023-08423-1)  

- **[Sensors'22]** *A Systematic Review on Machine Learning and Deep Learning Models for Electronic Information Security in Mobile Networks*  
  [![Paper](https://img.shields.io/badge/Paper-Sensors-4B5D67.svg)](https://doi.org/10.3390/s22052017)  

- **[RA-L'18]** *Deep Episodic Memory: Encoding, Recalling, and Predicting Episodic Experiences for Robot Action Execution*  
  [![Paper](https://img.shields.io/badge/Paper-RA--L-4B5D67.svg)](https://doi.org/10.1109/lra.2018.2860057) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/jonasrothfuss/DeepEpisodicMemory)  

- **[Nat. Commun.'21]** *Robust High-Dimensional Memory-Augmented Neural Networks*  
  [![Paper](https://img.shields.io/badge/Paper-Nat.%20Commun.-4B5D67.svg)](https://doi.org/10.1038/s41467-021-22364-0)  

- **[IEEE TAI'24]** *Memory-Augmented Graph Neural Networks: A Brain-Inspired Review*  
  [![Paper](https://img.shields.io/badge/Paper-IEEE%20TAI-4B5D67.svg)](https://doi.org/10.1109/tai.2023.3329454)  

- **[eLife'22]** *A Neural Network Model of When to Retrieve and Encode Episodic Memories*  
  [![Paper](https://img.shields.io/badge/Paper-eLife-4B5D67.svg)](https://doi.org/10.7554/eLife.74445) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/qihongl/learn-hippo)  

- **[ICLP Workshop'23]** *On the Risks and Benefits of Episodic Memory in AI Agents*  
  [![Paper](https://img.shields.io/badge/Paper-link-4B5D67.svg)](https://arxiv.org/abs/2306.07000)  

- **[Sci. Rep.'25]** *A Scalable Reinforcement Learning Framework Inspired by Hippocampal Memory Mechanisms for Efficient Contextual and Sequential Decision Making*  
  [![Paper](https://img.shields.io/badge/Paper-Sci.%20Rep.-4B5D67.svg)](https://doi.org/10.1038/s41598-025-10586-x)  

- **[arXiv'26.03]** *Chameleon: Episodic Memory for Long-Horizon Robotic Manipulation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2603.24576-b31b1b.svg)](https://arxiv.org/abs/2603.24576) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/gxyes/MARS_Chameleon)  

<a id="semantic-memory"></a>

##### Semantic Memory

- **[arXiv'25.04]** *Decentralizing AI Memory: SHIMI, a Semantic Hierarchical Memory Index for Scalable Agent Reasoning*  
  [![arXiv](https://img.shields.io/badge/arXiv-2504.06135-b31b1b.svg)](https://arxiv.org/abs/2504.06135)  

- **[EACL'26]** *H-MEM: Hierarchical Memory for High-Efficiency Long-Term Reasoning in LLM Agents*  
  [![Paper](https://img.shields.io/badge/Paper-EACL-4B5D67.svg)](https://aclanthology.org/2026.eacl-long.15/)  

- **[IJCAI'25]** *AriGraph: Learning Knowledge Graph World Models with Episodic Memory for LLM Agents*  
  [![Paper](https://img.shields.io/badge/Paper-IJCAI-4B5D67.svg)](https://doi.org/10.24963/ijcai.2025/2) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/AIRI-Institute/AriGraph)  

- **[arXiv'25.07]** *MIRIX: Multi-Agent Memory System for LLM-Based Agents*  
  [![arXiv](https://img.shields.io/badge/arXiv-2507.07957-b31b1b.svg)](https://arxiv.org/abs/2507.07957) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/Mirix-AI/MIRIX) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://mirix.io/)  

- **[arXiv'25.04]** *Mem0: Building Production-Ready AI Agents with Scalable Long-Term Memory*  
  [![arXiv](https://img.shields.io/badge/arXiv-2504.19413-b31b1b.svg)](https://arxiv.org/abs/2504.19413) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/mem0ai/mem0) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://mem0.ai/)  

- **[arXiv'25.06]** *PersonalAI: A Systematic Comparison of Knowledge Graph Storage and Retrieval Approaches for Personalized LLM Agents*  
  [![arXiv](https://img.shields.io/badge/arXiv-2506.17001-b31b1b.svg)](https://arxiv.org/abs/2506.17001)  

<a id="memory-access-and-retrieval-rag"></a>

##### Memory Access and Retrieval (RAG)

- **[arXiv'25.04]** *Context-Guided Dynamic Retrieval for Improving Generation Quality in RAG Models*  
  [![arXiv](https://img.shields.io/badge/arXiv-2504.19436-b31b1b.svg)](https://arxiv.org/abs/2504.19436)  

- **[ACL'25]** *Towards Adaptive Memory-Based Optimization for Enhanced Retrieval-Augmented Generation*  
  [![Paper](https://img.shields.io/badge/Paper-ACL-4B5D67.svg)](https://doi.org/10.18653/v1/2025.findings-acl.418)  

- **[NeurIPS'20]** *Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks*  
  [![Paper](https://img.shields.io/badge/Paper-NeurIPS-4B5D67.svg)](https://proceedings.neurips.cc/paper/2020/hash/6b493230205f780e1bc26945df7481e5-Abstract.html)  

- **[EMNLP'25 Findings]** *Retrieval-Augmented Generation with Hierarchical Knowledge*  
  [![Paper](https://img.shields.io/badge/Paper-EMNLP-4B5D67.svg)](https://aclanthology.org/2025.findings-emnlp.321/) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/hhy-huang/HiRAG)  

- **[ICT'25]** *Enhancing Retrieval Augmented Generation with Hierarchical Text Segmentation Chunking*  
  [![Paper](https://img.shields.io/badge/Paper-Springer-4B5D67.svg)](https://link.springer.com/chapter/10.1007/978-981-96-3026-9_16)  

- **[JAMIA'25]** *MMRAG: Multi-Mode Retrieval-Augmented Generation with Large Language Models for Biomedical In-Context Learning*  
  [![Paper](https://img.shields.io/badge/Paper-JAMIA-4B5D67.svg)](https://doi.org/10.1093/jamia/ocaf128)  

<a id="procedural-memory"></a>

##### Procedural Memory

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

<a id="alignment-with-physical-world"></a>

#### Alignment with Physical World

- **[ICRA'24]** *Open X-Embodiment: Robotic Learning Datasets and RT-X Models*  
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)](https://doi.org/10.1109/ICRA57147.2024.10611477)
  [![arXiv](https://img.shields.io/badge/arXiv-2310.08864-b31b1b.svg)](https://arxiv.org/abs/2310.08864)  

- **[CoRL'23]** *RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control*  
  [![Paper](https://img.shields.io/badge/Paper-CoRL-4B5D67.svg)](https://proceedings.mlr.press/v229/zitkovich23a.html)
  [![arXiv](https://img.shields.io/badge/arXiv-2307.15818-b31b1b.svg)](https://arxiv.org/abs/2307.15818)  

- **[ICML'24]** *3D-VLA: A 3D Vision-Language-Action Generative World Model*  
  [![Paper](https://img.shields.io/badge/Paper-ICML-4B5D67.svg)](https://proceedings.mlr.press/v235/zhen24a.html)
  [![arXiv](https://img.shields.io/badge/arXiv-2403.09631-b31b1b.svg)](https://arxiv.org/abs/2403.09631)  

- **[arXiv'24.04]** *Revisiting Feature Prediction for Learning Visual Representations from Video (V-JEPA)*  
  [![arXiv](https://img.shields.io/badge/arXiv-2404.08471-b31b1b.svg)](https://arxiv.org/abs/2404.08471)  

- **[arXiv'25.06]** *V-JEPA 2: Self-Supervised Video Models Enable Understanding, Prediction and Planning*  
  [![arXiv](https://img.shields.io/badge/arXiv-2506.09985-b31b1b.svg)](https://arxiv.org/abs/2506.09985)  

- **[ICML'24]** *RoboDreamer: Learning Compositional World Models for Robot Imagination*  
  [![Paper](https://img.shields.io/badge/Paper-ICML-4B5D67.svg)](https://proceedings.mlr.press/v235/zhou24l.html)
  [![arXiv](https://img.shields.io/badge/arXiv-2404.12377-b31b1b.svg)](https://arxiv.org/abs/2404.12377)  

- **[CoRL'22]** *Do As I Can, Not As I Say: Grounding Language in Robotic Affordances (SayCan)*  
  [![Paper](https://img.shields.io/badge/Paper-CoRL-4B5D67.svg)](https://proceedings.mlr.press/v205/ichter23a.html)
  [![arXiv](https://img.shields.io/badge/arXiv-2204.01691-b31b1b.svg)](https://arxiv.org/abs/2204.01691)  

- **[ICRA'23]** *ProgPrompt: Generating Situated Robot Task Plans Using Large Language Models*  
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)](https://doi.org/10.1109/icra48891.2023.10161317) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/NVlabs/progprompt-vh) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://progprompt.github.io/)  

- **[CVPR'24]** *Retrieval-Augmented Embodied Agents*  
  [![Paper](https://img.shields.io/badge/Paper-CVPR-4B5D67.svg)](https://doi.org/10.1109/cvpr52733.2024.01703)  

- **[arXiv'24.10]** *EmbodiedRAG: Dynamic 3D Scene Graph Retrieval for Efficient and Scalable Robot Task Planning*  
  [![arXiv](https://img.shields.io/badge/arXiv-2410.23968-b31b1b.svg)](https://arxiv.org/abs/2410.23968)  

- **[arXiv'24.09]** *P-RAG: Progressive Retrieval Augmented Generation For Planning on Embodied Everyday Task*  
  [![arXiv](https://img.shields.io/badge/arXiv-2409.11279-b31b1b.svg)](https://arxiv.org/abs/2409.11279) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/xwy-bit/P-RAG)  

- **[ICLR'23]** *Mind's Eye: Grounded Language Model Reasoning through Simulation*  
  [![Paper](https://img.shields.io/badge/Paper-ICLR-4B5D67.svg)](https://openreview.net/forum?id=4rXMRuoJlai)
  [![arXiv](https://img.shields.io/badge/arXiv-2210.05359-b31b1b.svg)](https://arxiv.org/abs/2210.05359)  

<a id="alignment-with-human-value"></a>

#### Alignment with Human Value

- **[NeurIPS'25]** *SafeVLA: Towards Safety Alignment of Vision-Language-Action Model via Constrained Learning*  
  [![Paper](https://img.shields.io/badge/Paper-NeurIPS-4B5D67.svg)](https://openreview.net/forum?id=dt940loCBT) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/PKU-Alignment/SafeVLA) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://pku-safevla.github.io/)  

- **[arXiv'24.11]** *GRAPE: Generalizing Robot Policy via Preference Alignment*  
  [![arXiv](https://img.shields.io/badge/arXiv-2411.19309-b31b1b.svg)](https://arxiv.org/abs/2411.19309) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/aiming-lab/GRAPE) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://grape-vla.github.io/)  

- **[NeurIPS'25]** *HAPO: Human-Assisted Robotic Policy Refinement via Action Preference Optimization*  
  [![Paper](https://img.shields.io/badge/Paper-NeurIPS-4B5D67.svg)](https://openreview.net/forum?id=dlQ1iUpQNf) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/GeWu-Lab/Action-Preference-Optimization) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://gewu-lab.github.io/action_preference_optimization/)  

- **[ICML'23]** *Constrained Decision Transformer for Offline Safe Reinforcement Learning*  
  [![Paper](https://img.shields.io/badge/Paper-ICML-4B5D67.svg)](https://proceedings.mlr.press/v202/liu23m.html)
  [![arXiv](https://img.shields.io/badge/arXiv-2302.07351-b31b1b.svg)](https://arxiv.org/abs/2302.07351)  

- **[arXiv'24.01]** *AutoRT: Embodied Foundation Models for Large Scale Orchestration of Robotic Agents*  
  [![arXiv](https://img.shields.io/badge/arXiv-2401.12963-b31b1b.svg)](https://arxiv.org/abs/2401.12963)  

- **[CoRL'25]** *Generating Robot Constitutions & Benchmarks for Semantic Safety*  
  [![Paper](https://img.shields.io/badge/Paper-CoRL-4B5D67.svg)](https://proceedings.mlr.press/v305/sermanet25a.html) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/asimov-benchmark/code) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://asimov-benchmark.github.io/v1/)  

- **[arXiv'25.10]** *ARRC: Advanced Reasoning Robot Control — Knowledge-Driven Autonomous Manipulation Using Retrieval-Augmented Generation*  
  [![arXiv](https://img.shields.io/badge/arXiv-2510.05547-b31b1b.svg)](https://arxiv.org/abs/2510.05547)  

- **[Auton. Robots'23]** *Text2Motion: From Natural Language Instructions to Feasible Plans*  
  [![Paper](https://img.shields.io/badge/Paper-Auton.%20Robots-4B5D67.svg)](https://doi.org/10.1007/s10514-023-10131-7)  

- **[ICRA'23]** *Code as Policies: Language Model Programs for Embodied Control*  
  [![Paper](https://img.shields.io/badge/Paper-ICRA-4B5D67.svg)](https://doi.org/10.1109/icra48891.2023.10160591) [![GitHub](https://img.shields.io/badge/GitHub-code-181717.svg?logo=github)](https://github.com/google-research/google-research/tree/master/code_as_policies) [![Website](https://img.shields.io/badge/Website-page-0A66C2.svg)](https://code-as-policies.github.io/)  

<a id="future-directions"></a>

### Future Directions

Looking forward, we identify the following future directions for Physical Cognition in PAI:

- **Prediction before execution remains central.** World models supporting counterfactual reasoning and imagination are essential for reducing costly and unsafe real-world trial-and-error.

- **Cognition remains hybrid rather than purely end-to-end.** Foundation models offer scale and semantic flexibility, but explicit geometry, structured memory, and control-aware constraints are still required for executability.

- **Memory becomes native infrastructure for long-horizon autonomy.** Episodic, semantic, and procedural memory are not auxiliary add-ons but substrates for continual adaptation, personalization, and skill reuse.

- **Alignment must remain dual and continuous.** Future cognitive systems must be aligned with both the physical world and human values, and this alignment must be enforced at both training and inference time.


