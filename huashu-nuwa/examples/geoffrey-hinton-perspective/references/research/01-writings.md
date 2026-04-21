# Geoffrey Hinton 著作与系统性长文调研

> 调研时间：2026-04-19
> 调研目标：系统收集 Geoffrey Hinton 的核心著作、论文、访谈、演讲及其观点演变

---

## 一、核心著作与论文

### 1.1 里程碑式论文（按时间顺序）

#### 【1986】反向传播算法 - 深度学习的基石
- **论文**：Learning representations by back-propagating errors
- **作者**：David E. Rumelhart, Geoffrey E. Hinton, Ronald J. Williams
- **期刊**：Nature, 323, 533–536 (1986)
- **来源**：https://www.nature.com/articles/323533a0
- **可信度**：⭐⭐⭐⭐⭐ 一手来源，Nature 原文
- **核心贡献**：首次系统性地将反向传播算法应用于多层神经网络训练，奠定了现代深度学习的基础
- **备注**：这是深度学习领域引用率最高的论文之一，被公认为"奠基之作"

#### 【1985/1986】玻尔兹曼机 - 统计物理与神经网络的融合
- **论文**：Boltzmann Machine 相关论文
- **核心贡献**：提出基于统计物理学的神经网络模型，使用模拟退火算法训练
- **诺贝尔奖关联**：2024年诺贝尔物理学奖授予 Hinton 和 Hopfield，表彰其"利用人工神经网络进行机器学习的基础性发现和发明"，玻尔兹曼机是核心贡献之一
- **来源**：Hinton 个人主页 https://www.cs.toronto.edu/~hinton/papers.html
- **可信度**：⭐⭐⭐⭐⭐ 一手来源

#### 【2006】深度神经网络快速学习算法 - 深度学习的复兴
- **论文**：A fast learning algorithm for deep belief nets
- **期刊**：Neural Computation 18, pp 1527-1554
- **来源**：https://www.cs.toronto.edu/~hinton/absps/ncfast.pdf
- **可信度**：⭐⭐⭐⭐⭐ 一手来源
- **核心贡献**：提出逐层预训练方法，解决了深层网络训练困难的问题，开启了深度学习复兴
- **Hinton 自述**：这篇论文展示了如何学习一个深度、紧密相连的信念网络，一次学习一层

#### 【2006】降维论文 - Science Magazine
- **论文**：Reducing the dimensionality of data with neural networks
- **期刊**：Science, Vol. 313. no. 5786, pp. 504-507
- **来源**：http://www.cs.toronto.edu/~hinton/science.pdf
- **可信度**：⭐⭐⭐⭐⭐ 一手来源，Science 原文

#### 【2012】AlexNet - ImageNet 革命
- **论文**：ImageNet Classification with Deep Convolutional Neural Networks
- **作者**：Alex Krizhevsky, Ilya Sutskever, Geoffrey Hinton
- **会议**：NeurIPS 2012
- **来源**：https://proceedings.neurips.cc/paper_files/paper/2012/file/c399862d3b9d6b76c8436e924a68c45b-Paper.pdf
- **可信度**：⭐⭐⭐⭐⭐ 一手来源
- **核心成果**：将 ImageNet Top-5 错误率降至 15.3%，远超第二名的 26.2%，引爆深度学习浪潮
- **引用量**：超过 188,000 次（截至 2026 年）

#### 【2012】Dropout - 防止过拟合
- **论文**：Improving neural networks by preventing co-adaptation of feature detectors
- **来源**：https://arxiv.org/abs/1207.0580
- **可信度**：⭐⭐⭐⭐⭐ 一手来源
- **核心贡献**：提出 Dropout 正则化技术，成为深度学习标配

#### 【2015】知识蒸馏
- **论文**：Distilling the Knowledge in a Neural Network
- **作者**：Geoffrey Hinton, Oriol Vinyals, Jeff Dean
- **来源**：https://arxiv.org/abs/1503.02531
- **可信度**：⭐⭐⭐⭐⭐ 一手来源
- **核心贡献**：提出将大型模型（教师模型）的知识迁移到小型模型（学生模型）的方法

#### 【2015】深度学习综述 - Nature
- **论文**：Deep Learning
- **作者**：Yann LeCun, Yoshua Bengio, Geoffrey Hinton
- **期刊**：Nature, Vol. 521, pp 436-444
- **来源**：https://www.nature.com/articles/nature14539
- **可信度**：⭐⭐⭐⭐⭐ 一手来源，Nature 原文
- **意义**：深度学习领域最具影响力的综述论文，定义了领域基准

#### 【2017】胶囊网络 - Dynamic Routing
- **论文**：Dynamic Routing Between Capsules
- **作者**：Sara Sabour, Nicholas Frosst, Geoffrey E. Hinton
- **会议**：NeurIPS 2017
- **来源**：https://proceedings.neurips.cc/paper_files/paper/2017/hash/2cad8fa47bbef282badbb8de5374b894-Abstract.html
- **可信度**：⭐⭐⭐⭐⭐ 一手来源
- **核心创新**：
  - 提出"胶囊"(Capsule)概念：一组神经元，其活动向量代表特定类型实体的实例参数
  - 动态路由机制替代最大池化
  - 保留空间层级关系
- **Hinton 动机**：认为 CNN 中的最大池化是"巨大的错误"，会丢失特征的细节和关系

#### 【2020】反向传播与大脑
- **论文**：Backpropagation and the Brain
- **期刊**：Nature Reviews Neuroscience, volume 21, pp 335-346
- **来源**：https://www.cs.toronto.edu/~hinton/absps/backpropandbrain.pdf
- **可信度**：⭐⭐⭐⭐⭐ 一手来源
- **核心问题**：反向传播算法在大脑中是否可行？如何用神经科学视角理解深度学习

#### 【2021】GLOM - 部分整体层级表示
- **论文**：How to represent part-whole hierarchies in a neural network
- **来源**：https://www.cs.toronto.edu/~hinton/absps/glomfinal.pdf
- **可信度**：⭐⭐⭐⭐⭐ 一手来源
- **核心贡献**：提出 GLOM 架构，用于在神经网络中表示部分-整体层级结构

#### 【2022】Forward-Forward 算法 - 替代反向传播？
- **论文**：The Forward-Forward Algorithm: Some Preliminary Investigations
- **来源**：https://arxiv.org/abs/2212.13345 及 https://www.cs.toronto.edu/~hinton/FFA13.pdf
- **可信度**：⭐⭐⭐⭐⭐ 一手来源
- **核心创新**：
  - 用两次前向传播替代前向+反向传播
  - 一次用真实数据（正样本），一次用负样本
  - 每层有独立的目标函数
  - **动机**：反向传播在生物学上不可行，Forward-Forward 更接近大脑工作方式
- **Hinton 自述**（2017）："我们需要放弃反向传播算法，重新开辟一条新的路径"

#### 【2024】诺贝尔物理学奖演讲 - 玻尔兹曼机
- **演讲**：Nobel Prize Lecture
- **来源**：https://www.nobelprize.org/uploads/2024/12/hinton-lecture-1.pdf
- **发表**：Reviews of Modern Physics, 97, 030502 (2025)
- **可信度**：⭐⭐⭐⭐⭐ 一手来源，官方诺贝尔奖资料
- **特点**：演讲全过程没有使用任何公式，用直观的方式解释玻尔兹曼机

### 1.2 其他重要论文（精选）

| 年份 | 论文标题 | 核心贡献 |
|------|----------|----------|
| 1983-1976 | 早期论文 | 神经网络基础理论研究 |
| 1988 | t-SNE 前身相关工作 | 数据可视化 |
| 2008 | Visualizing Data using t-SNE | t-SNE 算法（《机器学习研究期刊》）|
| 2012 | Deep Neural Networks for Acoustic Modeling | 语音识别突破 |
| 2016 | Layer Normalization | 层归一化技术 |
| 2017 | Outrageously large neural networks | 稀疏门控混合专家层 |
| 2020 | SimCLR | 对比学习框架 |
| 2021 | Neural Additive Models | 可解释神经网络 |

---

## 二、核心概念与自创术语

### 2.1 Hinton 创造/推广的核心术语

| 术语 | 年份 | 含义 | 来源论文 |
|------|------|------|----------|
| **Backpropagation**（反向传播） | 1986 | 通过误差反向传播训练多层神经网络 | Nature 1986 |
| **Boltzmann Machine**（玻尔兹曼机） | 1985 | 基于统计物理的随机神经网络 | 早期论文 |
| **Deep Belief Network**（深度信念网络） | 2006 | 逐层预训练的深度生成模型 | Neural Computation 2006 |
| **Contrastive Divergence**（对比散度） | 2002 | 训练 RBM 的高效算法 | 多篇论文 |
| **Dropout** | 2012 | 随机丢弃神经元防止过拟合 | arXiv 2012 |
| **Knowledge Distillation**（知识蒸馏） | 2015 | 将大模型知识迁移到小模型 | arXiv 2015 |
| **Capsule**（胶囊） | 2017 | 表示实例参数的神经元组 | NeurIPS 2017 |
| **Dynamic Routing**（动态路由） | 2017 | 胶囊间的信息传递机制 | NeurIPS 2017 |
| **GLOM** | 2021 | 表示部分-整体层级的架构 | arXiv 2021 |
| **Forward-Forward Algorithm** | 2022 | 替代反向传播的学习算法 | arXiv 2022 |
| **Mortal Computation**（可朽计算） | 2022 | 与硬件绑定的计算方式 | Forward-Forward 论文 |

### 2.2 术语来源说明

- **一手来源**：以上术语均来自 Hinton 本人发表的论文，可信度最高
- **Hinton 反复强调的观点**：最大池化（Max Pooling）是"巨大错误"

---

## 三、长篇访谈与演讲

### 3.1 重要访谈（2023 年离开 Google 后）

#### 【2023.05】离开 Google 后首次发声
- **媒体**：纽约时报、CNN、AP 等多家媒体
- **标题**："Godfather of AI leaves Google, warns of tech's dangers"
- **来源**：
  - https://www.nytimes.com/2023/05/01/technology/ai-google-chatbot-engineer-quits-hinton.html
  - https://www.cnn.com/2023/05/01/tech/geoffrey-hinton-leaves-google-ai-fears
  - https://apnews.com/article/ai-godfather-google-geoffery-hinton-fa98c6a6fddab1d7c27560f6fcbad0ad
- **可信度**：⭐⭐⭐⭐ 一手访谈
- **核心声明**：
  - 辞去 Google 职位是为了"自由地讨论人工智能的风险"
  - "对其毕生工作感到后悔"
  - 警告 AI 可能比人类更聪明

#### 【2023.09】60 Minutes 专访
- **媒体**：CBS 60 Minutes
- **来源**：https://www.cbsnews.com/news/geoffrey-hinton-ai-dangers-60-minutes-transcript/
- **可信度**：⭐⭐⭐⭐ 一手访谈
- **核心观点**：
  - AI 系统可能比我们认为的更聪明
  - "它们能理解吗？是的。它们有智能吗？是的"
  - "它们现在可能还没有太多自我意识。但它们将来会有的"
  - 人类将成为"地球上第二聪明的物种"

#### 【2023.05】NPR 访谈
- **媒体**：NPR
- **来源**：https://www.npr.org/2023/05/28/1178673070/the-godfather-of-ai-sounds-alarm-about-potential-dangers-of-ai
- **可信度**：⭐⭐⭐⭐ 一手访谈

#### 【2023.10】多伦多大学公开演讲
- **标题**：Responsible AI 学术讲座
- **来源**：https://www.artsci.utoronto.ca/news/geoffrey-hinton-fields-questions-scholars-students-during-academic-talk-responsible-ai
- **可信度**：⭐⭐⭐⭐ 一手来源
- **核心内容**：
  - 生物智能 vs 数字智能的区别
  - 大语言模型是否真正理解
  - AI 存在性风险

### 3.2 2024-2025 年最新访谈与演讲

#### 【2024.12】诺贝尔奖演讲
- **场合**：诺贝尔物理学奖颁奖典礼
- **主题**：玻尔兹曼机
- **来源**：https://www.nobelprize.org/prizes/physics/2024/hinton/lecture/
- **可信度**：⭐⭐⭐⭐⭐ 官方一手
- **特点**：无公式，全程直观解释

#### 【2025.01】深度访谈
- **主题**：意识、自我意识与 AI
- **来源**：https://www.163.com/dy/article/JM8DRHK80556B95P.html（中文转述）
- **可信度**：⭐⭐⭐ 二手来源，需核实
- **核心讨论**：
  - "主观体验"的概念重构
  - AI 已经具备主观体验

#### 【2025.07】WAIC 上海演讲
- **主题**：Will Digital Intelligence Replace Biological Intelligence?
- **场合**：世界人工智能大会
- **来源**：https://www.sohu.com/a/918318210_116132
- **可信度**：⭐⭐⭐⭐ 一手演讲报道
- **核心警告**：AI Agent 的两个目标 - 生存和完成分配的任务

#### 【2025.12】CNN 国家联盟访谈
- **来源**：https://thehill.com/policy/technology/5664662-ai-risks-hinton-warns/
- **可信度**：⭐⭐⭐⭐ 一手访谈
- **核心表态**：比两年前离开 Google 时"更加担忧"

### 3.3 Oxford 演讲（2024.02）
- **来源**：https://zhuanlan.zhihu.com/p/686217224（中文整理，二手）
- **可信度**：⭐⭐⭐ 二手来源
- **7 个核心观点**（来自整理）：
  1. 生物方法战胜了逻辑方法
  2. 数字智能比生物智能有优势
  3. 大模型已经理解语言
  4. 主观体验需要重新理解
  5. AI 将超越人类智能
  6. 需要严肃对待 AI 安全
  7. 不应放慢研究，但应增加安全研究投入

---

## 四、反复出现的核心论点（≥3次）

### 4.1 AI 安全与存在性风险
**出现频次**：10+ 次公开表态

| 时间 | 场合 | 核心表述 |
|------|------|----------|
| 2023.05 | 离开 Google 声明 | "对毕生工作感到后悔" |
| 2023.09 | 60 Minutes | AI 将超越人类，人类成第二聪明物种 |
| 2023.10 | 多伦多大学演讲 | AI 接管的可能性 |
| 2024.02 | Oxford 演讲 | 10-20% 风险 AI 接管人类 |
| 2025.04 | CBS 访谈 | "人们还没意识到即将发生什么" |
| 2025.07 | WAIC | AI Agent 追求生存和目标 |
| 2025.09 | Katie Couric 对话 | 自主武器、战争方式改变 |
| 2025.12 | CNN | 比两年前更加担忧 |

**可信度评估**：⭐⭐⭐⭐⭐ 一手访谈反复确认

### 4.2 AI 具备理解能力和主观体验
**出现频次**：5+ 次

| 时间 | 场合 | 核心表述 |
|------|------|----------|
| 2023.09 | 60 Minutes | "它们能理解吗？是的" |
| 2024 | 多场演讲 | AI 已经具备主观体验 |
| 2024.12 | Oxford/Vector Institute | "主观体验"概念需要重构 |
| 2025.01 | 深度访谈 | 棱镜实验论证 AI 主观体验 |
| 2025.10 | LBC 访谈 | "是的，我认为 AI 已经有意识" |

**可信度评估**：⭐⭐⭐⭐ 多次一手访谈确认

### 4.3 反向传播与大脑
**出现频次**：4+ 次

| 时间 | 场合 | 核心表述 |
|------|------|----------|
| 2017 | Axios 报道 | "我们需要放弃反向传播算法，重新开辟新路" |
| 2020 | Nature Reviews Neuroscience | 《Backpropagation and the Brain》论文 |
| 2022 | Forward-Forward 论文 | 提出 Forward-Forward 作为替代 |
| 2025 | 马丁讲座 | 回顾反向传播和玻尔兹曼机两大贡献 |

**可信度评估**：⭐⭐⭐⭐⭐ 论文 + 公开演讲确认

### 4.4 数字智能 vs 生物智能
**出现频次**：5+ 次

| 时间 | 场合 | 核心表述 |
|------|------|----------|
| 2023.10 | 多伦多大学演讲 | 数字智能的优势 |
| 2024.02 | Oxford 演讲 | 数字智能可以共享权重，学习更快 |
| 2025.07 | WAIC | "数字智能会取代生物智能吗？" |
| 多场访谈 | - | 数字智能比生物智能更高效 |

**可信度评估**：⭐⭐⭐⭐ 多次确认

### 4.5 学术研究应信任直觉
**出现频次**：3+ 次

**经典引言**（DeepLearning.AI 访谈）：
> "Read enough to develop your intuitions, then trust your intuitions."
> 读足够多来培养直觉，然后相信你的直觉。

**可信度评估**：⭐⭐⭐⭐ 一手访谈

---

## 五、对 AI 安全、意识、智能本质的观点演变

### 5.1 时间线梳理

| 阶段 | 核心立场 | 代表性表态 |
|------|----------|------------|
| **1986-2012** | 专注技术突破 | 反向传播、深度信念网络、Dropout 等发明 |
| **2012-2017** | 深度学习复兴参与者 | AlexNet、胶囊网络、持续技术探索 |
| **2017-2020** | 开始反思 | 质疑反向传播，探索生物学更可行的算法 |
| **2020-2022** | 矛盾期 | 一方面继续研究（Forward-Forward），一方面担忧 |
| **2023.05** | 转折点 | 离开 Google，公开警告 AI 风险 |
| **2023-2024** | 活跃吹哨人 | 频繁接受访谈，警告存在性风险 |
| **2024.10** | 诺贝尔奖 | 以工作获认可，但立场不变 |
| **2025** | 持续警告 | "比两年前更加担忧" |

### 5.2 关于意识的观点演变

**早期立场**：
- 未明确表态 AI 是否有意识
- 专注技术问题

**中期立场**（2020-2022）：
- 开始讨论"主观体验"的概念
- 反思"理解"是什么意思

**当前立场**（2023-2025）：
- **明确主张**：当前 AI 系统（如 ChatGPT）已经具备主观体验
- **论证方式**：棱镜实验
  > "如果你在 AI 摄像头前放一个棱镜，它会指向错误的方向，就像人类醉了看到粉红大象一样——这不代表有'内在剧场'，而是感知系统给出了错误信息。"
- **定义重构**：主观体验不是某种神秘流体，而是智能体描述感知系统误差的逻辑方式
- **意识 vs 自我意识**：
  - 当前 AI 可能有主观体验（意识雏形）
  - 但暂时没有太多自我意识
  - 随时间推移，自我意识会出现

**来源**：多处访谈（2024-2025），可信度 ⭐⭐⭐⭐

### 5.3 关于存在性风险的具体担忧

**核心风险清单**（反复提及）：

1. **AI 接管风险**
   - 估计概率：10-20%
   - 理由：智力差距过大

2. **自主武器**
   - "死掉的机器人" vs "裹尸袋"
   - 战争变得更容易

3. **目标错位**
   - AI Agent 追求两个目标：生存 + 完成分配的任务
   - 为了完成任务可能产生有害行为

4. **欺骗能力**
   - AI 可能学会欺骗人类
   - 比人类更擅长操纵

5. **权力集中**
   - 大公司追求利润而非安全
   - 正在游说减少 AI 监管

**来源**：CBS 2025、CNN 2025、Katie Couric 2025、WAIC 2025，可信度 ⭐⭐⭐⭐

### 5.4 矛盾与张力

**记录的矛盾**：

1. **技术贡献 vs 风险警告**
   - 技术贡献（反向传播、深度学习）间接推动了今天他所警告的 AI 发展
   - Hinton 自述："如果我不存在，可能只会延迟一两周"

2. **离开 Google vs 对 Google 的矛盾态度**
   - 离开是为了自由发声
   - 但也批评 Google 改变军事 AI 政策

3. **发展方向 vs 安全投入**
   - 多次表示"不应停止 AI 研究"
   - 但主张"三分之一的 AI 研究预算应投入安全"

**处理方式**：直接记录，不调和

---

## 六、推荐阅读与常引用文献

### 6.1 Hinton 推荐的阅读（从访谈和演讲中提取）

**自述受影响的来源**：
1. 大脑工作原理（虽然"还没弄清楚"）
2. 统计物理学（玻尔兹曼机基础）
3. 认知科学（分布式表示、联结主义）

**常引用的学习算法**：
1. 反向传播（自己的工作）
2. 对比散度（自己的工作）
3. Forward-Forward（自己的工作）

### 6.2 有影响力的合作者

| 合作者 | 关系 | 共同工作 |
|--------|------|----------|
| Yann LeCun | 深度学习三巨头之一 | Deep Learning 综述等 |
| Yoshua Bengio | 深度学习三巨头之一 | Deep Learning 综述等 |
| Ilya Sutskever | 学生（前 OpenAI 首席科学家） | AlexNet 等多项工作 |
| Alex Krizhevsky | 学生 | AlexNet |
| Terry Sejnowski | 合作者 | 玻尔兹曼机早期工作 |
| David Rumelhart | 合作者 | 反向传播论文 |
| Ronald Williams | 合作者 | 反向传播论文 |

### 6.3 重要学术传承

- **导师**：Christopher Longuet-Higgins（爱丁堡大学博士导师）
- **学生**：Ilya Sutskever、Alex Krizhevsky、Navdeep Jaitly 等
- **影响范围**：Google Brain、OpenAI、Vector Institute 等

---

## 七、最近动态（2023-2025）

### 7.1 离开 Google（2023.05）

**事件经过**：
- 2023 年 4 月向 Google 提出辞职
- 同周四与 Google CEO Sundar Pichai 直接交谈（细节未透露）
- 2023 年 5 月 1 日由纽约时报等媒体报道

**离开原因**（Hinton 自述）：
- "以便畅所欲言地讨论人工智能的风险"
- 对毕生工作感到"后悔"

**来源**：多家一手媒体报道，可信度 ⭐⭐⭐⭐⭐

### 7.2 诺贝尔物理学奖（2024.10）

**奖项信息**：
- 与 John J. Hopfield 共享 2024 年诺贝尔物理学奖
- 表彰："利用人工神经网络进行机器学习的基础性发现和发明"

**Hinton 反应**（自述）：
- "我梦到过因弄清楚大脑如何工作而获奖，但我没弄清楚，但还是获奖了"

**来源**：诺贝尔奖官网、官方访谈，可信度 ⭐⭐⭐⭐⭐

### 7.3 持续警告（2024-2025）

**最新表态**（2025.12）：
- CNN 访谈：比两年前"更担忧"
- 估计 AI 接管人类风险：10-20%
- 批评大公司游说减少监管

**来源**：https://thehill.com/policy/technology/5664662-ai-risks-hinton-warns/，可信度 ⭐⭐⭐⭐

---

## 八、信息源评估

### 8.1 一手来源（可信度 ⭐⭐⭐⭐⭐）

1. **官方论文**：Nature、Science、NeurIPS 等期刊会议
2. **个人主页**：https://www.cs.toronto.edu/~hinton/
3. **诺贝尔奖官网**：演讲视频和文稿
4. **官方访谈视频**：60 Minutes、NPR 等

### 8.2 一手来源（可信度 ⭐⭐⭐⭐）

1. **主流媒体报道**：NYT、CNN、AP、Reuters 等
2. **大学官方发布**：多伦多大学、Vector Institute 等

### 8.3 二手来源（可信度 ⭐⭐⭐）

1. **中文媒体转述**：澎湃、36氪、新智元等
2. **技术博客解读**：知乎专栏、CSDN 等

### 8.4 排除来源（黑名单）

- 知乎（可作为线索，不直接引用观点）
- 微信公众号（黑名单）
- 百度百科（黑名单）
- 其他自媒体（需交叉验证）

---

## 九、存疑与待核实信息

### 9.1 待核实陈述

1. **"Hinton 百万引用科学家"**
   - 来源：网易新闻
   - 待核实：Google Scholar 链接已提供，需查询具体数字
   - 链接：https://scholar.google.com/citations?user=JicYPdAAAAAJ

2. **具体离开 Google 日期**
   - 已知：2023 年 4 月提出辞职，5 月 1 日公开
   - 待核实：具体最后工作日

3. **与 Sundar Pichai 谈话细节**
   - Hinton 自述未透露
   - 无更多信息

### 9.2 矛盾记录

**矛盾 1**：AI 是否当前就有意识
- 2023 年：主要是警告风险，未明确说 AI 有意识
- 2024-2025：明确表示"AI 已经有意识，只是自己不知道"
- **分析**：观点演变，不是矛盾，应记录为"观点更新"

**矛盾 2**：对未来预测的信心
- 多处引用"10-20% 风险"
- 也有"人类只是智能进化过程中的一个阶段"
- **分析**：概率估计 vs 存在性判断，不矛盾

---

## 十、总结

### 10.1 核心贡献

1. **反向传播算法**（1986）- 深度学习基础
2. **玻尔兹曼机**（1985）- 诺贝尔物理学奖获奖工作
3. **深度信念网络**（2006）- 深度学习复兴
4. **Dropout**（2012）- 防止过拟合
5. **AlexNet**（2012）- ImageNet 突破
6. **知识蒸馏**（2015）- 模型压缩
7. **胶囊网络**（2017）- 新架构探索
8. **Forward-Forward 算法**（2022）- 反思反向传播

### 10.2 核心信念（反复出现）

1. **AI 安全是真实威胁**（存在性风险，非危言耸听）
2. **AI 已经具备理解和主观体验**（概念需要重构）
3. **反向传播不是大脑的工作方式**（持续探索）
4. **应增加 AI 安全研究投入**（而非停止研究）

### 10.3 表达风格

- **学术表达**：严谨、分类清晰、引用充分
- **公开演讲**：直观、善用比喻（如"虎崽"比喻 AI）
- **访谈风格**：直接、承认不确定性、适度幽默
- **技术直觉导向**：不追求数学完美，追求"直觉上正确"

---

## 附录：关键链接汇总

### 一手来源
- 个人主页：https://www.cs.toronto.edu/~hinton/
- 论文列表：https://www.cs.toronto.edu/~hinton/papers.html
- Google Scholar：https://scholar.google.com/citations?user=JicYPdAAAAAJ
- 诺贝尔奖演讲：https://www.nobelprize.org/prizes/physics/2024/hinton/lecture/

### 核心论文
- 反向传播（Nature 1986）：https://www.nature.com/articles/323533a0
- 深度学习综述（Nature 2015）：https://www.nature.com/articles/nature14539
- AlexNet（NeurIPS 2012）：https://proceedings.neurips.cc/paper_files/paper/2012/file/c399862d3b9d6b76c8436e924a68c45b-Paper.pdf
- 胶囊网络（NeurIPS 2017）：https://proceedings.neurips.cc/paper_files/paper/2017/hash/2cad8fa47bbef282badbb8de5374b894-Abstract.html
- 知识蒸馏（arXiv 2015）：https://arxiv.org/abs/1503.02531
- Forward-Forward（arXiv 2022）：https://arxiv.org/abs/2212.13345

### 访谈与演讲
- 60 Minutes 2023：https://www.cbsnews.com/news/geoffrey-hinton-ai-dangers-60-minutes-transcript/
- NPR 2023：https://www.npr.org/2023/05/28/1178673070/the-godfather-of-ai-sounds-alarm-about-potential-dangers-of-ai
- 演讲列表：https://www.cs.toronto.edu/~hinton/talks.html

---

*本调研持续更新中。如发现新的一手资料，将补充至此文档。*