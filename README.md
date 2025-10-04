



[toc]



（暂时把会议纪要当成每一周的README）



# 2025 10.4  PAI（Physical AI）Survey Writting —— 会议纪要



#### Previous Week Progress:

- Decided to submit the survey to **ACM Computing Surveys**.
- Polished the **general structure diagram**.
- Drafted the **background section**.
- Outlined the **perception block structure**.
- Shared and discussed relevant papers.

#### Plan for This Week:

- Conduct further **paper reading** to support the initial design of the **cognition block** and **actuation block**.
- **Collect related work** for each module, extract key insights, and prepare content for writing.
- Continue to **iterate and refine** the overall structure of the survey.





# 2025.9.19 1st PAI（Physical AI）Paper-Reading —— 会议纪要（整理 & 润色）

## 一、工作的价值（Why this matters）

1. **Impact**：此项工作意义重大——有潜力成为第一篇完整的 **PAI Summary**，为领域提供系统性综述与方向引导。
2. **Citation**：高质量综述/summary 能显著提高被引用概率，提升团队影响力。
3. **Insights**：系统化整理与批判性分析能产出可复用的研究洞见，对后续创新研究有直接推动作用。

------

## 二、关键决策 / 需要尽早确定的问题

1. **尽早并持续地给出“Physical AI”的工作定义**，把定义放到团队共享文档里，随证据与讨论不断迭代（版本控制）。
2. **明确 PAI 与 EAI（Embodied AI）/相关概念的差异**，并回答“是否只是炒冷饭？”——我们需要用清晰的边界与新的关注点（例如非视觉模态、物理交互细节）来证明工作的新意。
3. **论文筛选标准与分类体系（taxonomy）要边读边建**，每篇论文在被收录时即贴标签并插入到对应类别，方便索引与回溯。

------

## 三、工作范围：是否需要 narrow the subject？

**结论：是（建议从“更Physical”的角度切入）**
 建议聚焦于：**多模态感知 + 输出/交互端（强调非视觉模态与物理世界交互）**。
 这样既保留“Embodiment”的核心，又突出现实世界物理感知与交互的独特挑战与机遇。

------

## 四、论文选择标准（Paper selection criteria）

1. **文章质量**：期刊/会议层次、审稿严格度、实验与方法论严谨性。
2. **主题重合度**：与我们定义的 PAI 目标的贴合度（高优先）。
3. **补充考量**：被引量（/新文章则看引用趋势）、是否公开代码/数据、可复现性、是否提出新的评测或基准。
4. **收录元数据（建议字段）**：标题、作者、年份、venue、DOI、关键词、简短贡献摘要、核心方法、数据/代码链接、弱点、我们对其的归类标签、阅读日期、负责阅读者、slides 链接。

------

## 五、Shared Timeline（共享时间线 / 索引）建议设计

- **结构**：一张表格（Google Sheet / GitHub Table / Notion）作为主索引。
- **推荐字段**（便于检索与排序）：ID、Title、Year、Venue、Tags（模态/任务/embodiment 类型）、Summary（1–2 行）、Contribution bullets、Weaknesses、Links（pdf/code/dataset）、Assigned reader、Slides、Status（待读/已读/讨论）。
- **版本控制**：timeline 与 taxonomy 都要有版本号和修改记录，方便追踪演进。

------

## 六、Working definition（工作版“Physical AI”定义 —— 草案）

> **Physical AI（PAI）**：能够长期在物理世界中感知、理解并与环境或人类进行物理交互的智能系统；其特征是（1）多模态物理感知（视觉、声音、RF、触觉、力觉等），（2）实时/弱延迟决策与交互能力，及（3）感知—表示—交互之间紧密耦合的系统工程实践与评测方法。

**迭代策略**：将此定义存为可编辑草案（v0.1），在每次阅读会后用新的证据更新并记录变更理由。

------

## 七、Taxonomy（分类体系）建议（初步）

- **按模态**：视觉 / 声音（语音识别、说话人识别） / RF（WiFi/UWB/雷达） / 触觉 / 力觉 / 多源融合
- **按任务类型**：定位与导航 / 感知（物体、人体状态） / 交互（人机、物物） / 状态估计（速度、心跳、压力等）
- **按主体形态**：移动平台 / 操作臂 / 可穿戴 / 固定感知节点
- **按方法学**：模型驱动 / 数据驱动 / 混合 / 仿真→现实迁移
- **按研究产出**：算法 / 硬件 / 数据集 / 评测基准 / 系统集成

> 每篇论文读取时，务必将其贴上上述标签中的若干项，便于聚类分析与主题抽取。

------

## 八、目前综述存在的主要问题（我们要如何改进）

1. **宣称多模态但“多”是表面化的**：许多综述仍以视觉为中心，其他模态（RF、触觉、声音）只作点到为止的补充。
    → 我们要做真实的多模态审视：比较不同模态的物理信息量、测量噪声特性、融合策略与约束。
2. **感知与交互方式有限、过于简单**：交互通常停留在简单命令或视觉反馈层面，忽略物理交互的连续性与鲁棒性（例如触觉反馈、力控制、多主体物理接触）。
    → 我们要重点找或推动那些在物理接触、力感知、触觉上有创新的工作。
3. **缺少对非视觉传感器/信号（RF、声学、触觉）的深入比较**：这是一大提升空间。
    → 我们要建立一个“模态对比矩阵”，列出每种模态的优/劣、典型噪声与适用场景。
4. **评测基准与实用性不足**：多数工作在受控实验室里有效，但现实部署（遮挡、干扰、动态变化）下不够稳健。
    → 我们要总结并推荐更贴近现实的评测流程或提出新的benchmark建议。

------

## 九、感知任务与交互任务的分类（建议用于taxonomy）

### 1. Traditional Functions（传统功能）

- 视觉识别（物体、障碍）
- 定位/SLAM
- 路径规划 / 控制（注：此部分可简略，非重点）
- 语音指令识别（基础 ASR）

### 2. Novel Features（可作为 PAI 特色强调的任务/能力）

- **生理参数估计**：例如心跳、呼吸、压力监测（通过非接触手段或可穿戴）。
- **步态与速度估计**：用于行为理解与身份/状态识别。
- **说话人识别与声源局部化**（与视觉、RF融合）。
- **触觉/接触感知与力控制**（真实接触交互）。
- **RF/雷达感知下的穿透/非视线检测**（如墙后活动检测）。
- **多主体物理交互协作**（人机协作中的物理安全与力协调）。

------

## 十、对“PAI vs EAI” 的讨论（简要）

- **Embodied AI（EAI）** 通常强调“有身体的智能体”——关注认知、学习与决策在具身（embodied）环境中的实现（偏理论与认知建模）。
- **Physical AI（PAI）** 建议作为更工程/实用导向的子集或兄弟概念：更强调 **物理世界中的多模态传感器、物理量测、实际交互接口与系统集成**。
- **不是炒冷饭**：如果我们把关注点放在“被忽略的物理模态（RF、触觉、力）”“真实物理交互场景的评测”和“端到端系统工程实践”，则可以提出实质上的新问题与方法，具有创新价值。

------

## 十一、Paper-reading 环节的要求（必须执行）

1. **每次阅读会必须有 slides（PPT）**，且包含明确的“我的观点与收获”页。
2. **Slides 内容模板（建议）**：
   - 题目 + 作者 + 发表时间/venue
   - 1-句总结（what problem & what they claim）
   - 贡献点（bullets）
   - 方法概览（框图 + 算法关键点）
   - 数据/实验设置（包含是否有真实物理部署）
   - 优点 / 缺点（技术与实验）
   - 与 PAI 的关系（模态、任务类别、可复用点）
   - 我们的疑问 / 后续可做的改进 / follow-up idea
3. **阅读报告（短文档）模板**：1-page，包括 1) 1-句总结 2) Top-3 takeaways 3) Top-3 limitations 4) 我们可以借鉴或直接复现的部分。
4. **每篇论文分配“主讲人 + 讨论人”**，主讲人负责 slides 与初稿报告，讨论人提前读并提出 3 个拓展问题。

------

## 十二、建议的研究切入点（Narrowed Topics，举例）

1. **非视觉多模态感知集成（RF + 音频 + 触觉）在室内人体状态估计中的应用**（如步态、心率、行为识别）。
2. **物理交互下的鲁棒触觉感知与控制**（人机协作抓取/穿戴设备交互场景）。
3. **现实世界评测基准设计**：模拟真实干扰（遮挡、多径、动态人群）的 PAI Benchmark。
4. **跨模态信息稀缺下的自监督/少样本融合策略**（从仿真到现实的迁移）。

------

## 十三、关于“机器人控制无需过多侧重”的说明

- 团队建议**弱化对传统控制（低阶 PID / 运动控制）深度讨论**，将精力放在 **感知、融合、交互接口与评测**。必要时引用控制作为系统实现的一部分，但不作为核心贡献点。

------

## 十四、下一步（Action Items / 拟办事项）

1. **确定负责定义草案的人**：撰写 PAI v0.1（放到共享文档并设立版本号）。——负责人：指定一名主笔（Team指定）
2. **建立 Shared Timeline 表格并初始化字段模板**（Google Sheet / Notion / GitHub）。——负责人：1 人（负责表格搭建）
3. **制定并发布 paper-reading slides & report 模板**，把模板放在共享目录。——负责人：主讲模板作者
4. **选出下 3 篇优先阅读的 paper**（按照筛选标准），并分别分配主讲/讨论人。——负责人：阅读会组织者
5. **每次阅读会上强制包含“个人观点与收获”页**，并将 slides 上传到共享目录。——全员遵守
6. **构建模态对比矩阵（初稿）**，列出视觉/音频/RF/触觉在若干典型任务上的优劣势。——负责人：2 人合作
7. **在下一次会议审阅并迭代 PAI 定义与 taxonomy**（基于新收集的论文与讨论结果）。

------

## 十五、会议结论（总结）

- 目标清晰：产出高质量的 PAI 综述/summary，强调“物理性”与“真实多模态交互”的新问题。
- 方法可执行：尽早锁定工作定义、建立共享索引、严格执行阅读会模板并边读边建 taxonomy。
- 预期收益：形成可引用的综述文章、可复用的评测/数据集建议，以及若干可推进的研究课题。





# The first meeting

## 一、明确概念

- **Physical AI**：不仅是“具身智能 (Embodied AI)”，还包括与物理世界交互的更广范围的 AI。
  - Embodied AI：强调 **AI+身体**，机器人等。
  - AIOT：侧重 **物联网+智能**，偏感知与分布式系统。
  - Agentic AI：强调 **自主性、规划、决策**，未必有物理形态。
  - AI + CPS (Cyber-Physical Systems)：**控制与物理结合**，偏系统层面。

👉 结论：**不是 Embodied AI 的但可以算 Physical AI 的** → AIoT、AI+CPS。
 Agentic AI 本身不一定是 Physical AI，但如果赋予传感器与执行器，则可以成为 Physical AI 的核心部分。

------

## 二、Physical AI 的愿景

- 一个完整的闭环系统：
   **输入 (sensing) → 信号处理 (signal processing) → 表征学习/推理 (AI model/Agentic AI) → 输出 (actuation)**
- 与机器人、自主系统紧密相关，既包括硬件系统，也包括智能体决策。

------

## 三、模块划分

可以采用**端到端框架 + 模块化视角**结合：

1. **Sensing（传感器与数据采集）**
   - 多模态感知（视觉、语音、雷达、触觉等）
2. **Signal Processing（信号处理与低层特征提取）**
   - 噪声抑制、特征压缩、融合
3. **Perception & Representation（感知与表征学习）**
   - 从低层特征到高层语义
4. **Agentic AI（自主决策与推理）**
   - 规划、目标设定、推理、长期自主性
5. **Actuation & Control（执行与控制）**
   - 机械臂、机器人、自主系统行动
6. **System Integration（系统层与CPS）**
   - 网络、资源管理、安全与隐私

------

## 四、现存问题 & 挑战

1. **传感层**
   - 噪声大、传感器精度受限、多模态对齐不成熟。
2. **信号处理**
   - 与AI结合不足，传统信号处理和深度学习融合还在探索阶段。
3. **感知与表征**
   - 在复杂环境下鲁棒性不足，缺乏泛化。
4. **Agentic AI**
   - 高级自主性与现实物理约束之间的gap大；规划可解释性不足。
5. **执行与控制**
   - 控制算法与学习算法融合不成熟，实时性差。
6. **系统层**
   - 缺乏统一的评估标准；CPS/AIOT在安全、隐私、能耗上存在难点。

------

## 五、区分 Physical AI 与 Agentic AI

- **Physical AI**：强调 AI 与 **物理世界耦合**，必须有传感器+执行器闭环。
- **Agentic AI**：强调 **智能体的自主性**，可以存在于纯虚拟环境，不一定与物理实体绑定。
   👉 二者交叉点：**当 Agentic AI 驱动物理系统时，就变成了 Physical AI 的核心大脑**。

------

## 六、如何做 Survey

1. **角度**
   - 模块化视角（从感知→处理→决策→控制）
   - 应用视角（机器人、自动驾驶、医疗设备、智能制造等）
   - 技术融合视角（信号处理 + AI，CPS + AIOT + Embodied AI）
2. **结构**
   - 先定义概念
   - 分模块综述已有研究
   - 强调不同方向的结合点与不足
   - 总结挑战与未来趋势
3. **结论**
   - Physical AI 是跨学科的，现阶段大多研究还停留在**单模块突破**，缺少端到端融合。
   - 未来趋势：**多模态感知+Agentic AI+实时控制+CPS集成**。

------

## 七、写作时的 Key Points

- **区别与联系**：Physical AI vs Embodied AI vs Agentic AI
- **端到端框架**：输入-处理-决策-输出
- **模块化结构**：分层梳理研究
- **问题与挑战**：哪些部分不成熟（重点放在 sensing、signal processing 与 AI 融合、Agentic AI 的物理可解释性）
- **未来趋势**：跨模态、跨层级，走向全闭环系统

------

📌 **总结**：
 你们的综述应当以 **Physical AI 的定义与边界**为起点，强调它不仅包含 Embodied AI，还扩展到 AIOT 和 CPS。以 **模块化+端到端的框架**来组织文章，分别介绍 sensing、signal processing、perception、agentic AI、actuation 与系统集成。最后重点放在 **挑战、不足与未来方向**，这样既有结构，又能突显价值。

好，那我帮你拟一个**《Physical AI综述》大纲目录**，带上小标题，基本可以直接用在论文初稿里：

------



# Survey on Physical AI: From Sensing to Agentic Intelligence

## 1. Introduction

- 背景与动机
- 为什么需要“Physical AI”这一概念
- 区别与联系：Physical AI vs. Embodied AI vs. Agentic AI vs. AIoT vs. CPS
- 本文贡献与结构安排

------

## 2. Definition and Scope of Physical AI

- 物理世界交互的核心特征
- 必须包含的基本要素：**Sensing – Processing – Intelligence – Actuation – Integration**
- 应用领域：机器人、自主系统、医疗、交通、工业物联网

------

## 3. Core Modules of Physical AI

### 3.1 Sensing

- 多模态传感器（视觉、语音、雷达、触觉）
- 信号获取与预处理
- 挑战：噪声、多模态对齐、数据稀疏

### 3.2 Signal Processing

- 传统信号处理方法与AI结合
- 特征提取与压缩
- 多源信息融合
- 挑战：实时性、能耗约束、鲁棒性

### 3.3 Perception and Representation

- 表征学习与高层语义感知
- 自监督、多模态学习在Physical AI中的应用
- 挑战：泛化能力差、在复杂环境中的鲁棒性不足

### 3.4 Agentic AI (Decision and Planning)

- Agentic AI 的定义与发展
- 与物理世界交互时的决策问题
- 挑战：可解释性、长期规划、物理约束适配

### 3.5 Actuation and Control

- 执行器（机器人手臂、无人车、仿生系统等）
- 控制算法与学习算法的结合（Learning-based Control）
- 挑战：实时反馈、稳定性、安全性

### 3.6 System Integration (AI + CPS/AIoT)

- Cyber-Physical Systems 与 AI 的结合
- 分布式与协同控制（AIoT）
- 安全、隐私与能效问题

------

## 4. Comparison with Related Paradigms

- Physical AI vs Embodied AI
- Physical AI vs Agentic AI
- Physical AI vs AIoT
- Physical AI vs CPS

------

## 5. Current Research Landscape

- 典型研究方向与成果总结（按模块/应用领域分类）
- 代表性论文/系统/benchmark (可仅限顶会)
- 成果总结：做了什么 → 有什么效果 → 怎么和AI结合 → 存在什么缺陷

------

## 6. Challenges and Open Problems

1. Sensing：高精度、多模态协同感知不成熟
2. Signal Processing：传统DSP与深度学习缺乏统一框架
3. Perception：鲁棒性、泛化、复杂环境适应性不足
4. Agentic AI：缺乏物理世界中的可解释、自主与安全性
5. Actuation：实时控制与智能规划结合不成熟
6. System Level：安全性、隐私保护、能耗优化、缺乏评估基准

------

## 7. Future Directions

- 端到端 vs 模块化的结合
- 多模态感知与大模型驱动的统一表征
- 自主性与可解释性兼顾的 Agentic AI
- Learning-based Control 与 CPS 的深度耦合
- 标准化评估与开放benchmark

------

## 8. Conclusion

- 总结Physical AI的内涵与意义
- 模块化回顾与未来展望

------

📌 **写作建议**：

- 每一章都要用 **问题-方法-效果-不足** 的小循环。
- 特别注意“Agentic AI 在物理世界中的不足”这一块，会是热点。
- 结尾一定强调“跨学科融合+标准化评估”的趋势。

------

