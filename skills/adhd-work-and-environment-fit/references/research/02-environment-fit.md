# 02 — 环境适配的实证：什么在结构上帮得到，什么没有证据

**调研时间：2026-10-12**
**取数路径**：NCBI E-utilities（esearch/efetch）· OpenAlex API · Crossref API · Europe PMC REST API。全部直连一手记录。

> **本文件最重要的一句话（先说）**：
> **关于「ADHD 需要什么样的工作环境」，有一件事是确凿的——**
> **有针对 ADHD 人群的直接实证研究极少，少到已经有人专门为此写了两篇范围综述来记录这个空白。**
> **而关于「什么样的工作结构有害」，证据几乎全部来自一般人群，要外推到 ADHD 是一个未被检验的动作。**
> **本文件对每一条都标注了研究人群。跳过这个标注去读本文件，会得到一批看起来很确定、实际上不能用的结论。**

---

## 〇、研究人群标签约定（读本文件前请先记住）

| 标签 | 含义 | 可否直接用于「ADHD 者该怎么办」 |
|---|---|---|
| 🅐 **ADHD 人群实证** | 样本是 ADHD 患者或按 ADHD 特质分组 | ✅ 可以（仍受设计限制约束） |
| 🅑 **神经多样性人群（ASD 为主）** | 样本是自闭症/神经多样性者 | ⚠️ 只能作**类比**，必须标注为 ASD |
| 🅒 **一般人群实证** | 样本是普通员工/学生/被试 | ⚠️ **是外推，不是证据** |
| 🅓 **自报 / 定性 / 叙述** | 无对照、样本自我选择 | ⚠️ 只能说明「有这个问题存在」，不能估计大小 |

---

## 一、两个「记录空白的综述」——先看这两篇，本文件的结构就定了

### 1.1 🅐 ADHD × 开放办公：专门的范围综述，结论是「没有实证研究」

**S1｜Sanders, J. & Le Rossignol, E. (2026).** *Don't disable me: A scoping review of ADHD employees' experiences of working in open-plan offices.* **Work.**
DOI: **10.1177/10519815261449927** ｜PMID **42132039** ｜【同行评议论文，范围综述（scoping review）】｜可信度：**高**

**摘要原文（关键句逐字）**：
> "The analysis identified **twenty-two pieces of literature**, revealing a **significant gap in empirical research on ADHD workers in open-plan offices**."
> "**While empirical evidence is sparse**, anecdotal evidence, professional opinions, the inherent nature of ADHD, and participants' lived experiences indicate that open-plan offices can impede creativity and productivity of ADHD employees."
> "Conclusions: This scoping review highlights the **scarcity of systematic research** on this topic and underscores the need for future studies to **empirically assess** how open-plan office environments affect ADHD employees. The findings suggest these environments may negatively impact not only the wellbeing of ADHD workers **but the general workforce** and potentially an organisation's overall performance."

🔴 **本文件必须以此为基调**：
1. 22 篇相关文献里**没有一个是「在 ADHD 员工中比较开放办公 vs 非开放办公」的对照实证**。
2. 结论里那句 "**but the general workforce**" 很关键——**综述作者自己说，这个判断的一般人群版本也还没被证明。**
3. ⚠️ **但是**——下面 §3 的一般人群证据其实**相当强**。所以诚实的表述是：
   > **「开放办公对 ADHD 员工有害」是一个被广泛重复的判断，它的 ADHD-specific 版本没有被直接检验，但它的一般人群版本有相当强度的客观测量支持。** 换句话说：这个建议**大概率是对的**，但它的证据链比你以为的短一环。

### 1.2 🅑 神经多样性 × 物理工作场所适配：319 篇筛到 20 篇，结论是「证据不足以评估」

**S2｜Weber, C., Krieger, B., Häne, E., Yarker, J. & McDowall, A. (2022).** *Physical workplace adjustments to support neurodivergent workers: A systematic review.* **Applied Psychology.**
DOI: **10.1111/apps.12431** ｜OpenAlex 被引 **81** ｜【同行评议论文，系统综述（PRISMA）】｜可信度：**高**

**摘要原文（关键句逐字）**：
> "neurodivergence is an umbrella term for various conditions such as Autism-Spectrum Disorder (ASD), Attention-Deficit/Hyperactivity Disorder (ADD/ADHD), Dyslexia, or Dyspraxia, which affect **approximately 22% of the population**."
> "Of the **319 studies identified, 20 met the eligibility criteria**; **the majority addressed ASD**."
> "The most frequent adjustments addressed **sound distractions (e.g. single-person offices)** and **light sensitivity (e.g. light control)**, which were related to occupational longevity, performance and health/well-being. A range of other adjustments addressed aspects such as environmental control, crowding or decompression rooms."
> 🔴 **"There is insufficient evidence to fully evaluate the usefulness of adjustments, partially due to methodological shortcomings."**
> "Despite the variety of challenges with the sensory physical environment acknowledged in the literature for neurodivergent conditions, **there is a paucity of evidence**."

🔴 **这是整个维度 2 的定盘星**：
- **纳入标准明确写的是「成人办公室工作者（clinically considered neurodiverse）」**——ADHD 在范围内。
- **但 20 篇里大多数是 ASD。**
- 综述自己的结论：**不足以评估这些适配是否有用。**
- ⚠️ **重要方法学注记**：这 20 篇**全部是物理/感官环境适配**（单人办公室、光线控制、减压室）。**不包括**组织层面的适配（任务结构、反馈方式、截止日期管理）——**那部分的证据连综述都还没到。**

---

## 二、🅐 唯一一组 ADHD-specific 的适配量化数据（且带重要警告）

**S3｜Suzuki, T., Nakazato, M., Ohtani, F. & Ikeda, A. (2026).** *Workplace adjustments equivalent to reasonable accommodations and workplace maladjustment in a general working population, with a focus on high autism spectrum disorder (ASD) and attention deficit/hyperactivity disorder (ADHD) traits.* **Environmental Health and Preventive Medicine, 31**, 62.
DOI: **10.1265/ehpm.26-00080** ｜PMID **42749630** ｜【同行评议论文，横断面调查】｜可信度：**中高**

### 2.1 研究设计

> **N = 1,000 名随机抽取的全日本劳动者**，自填式在线问卷，横断面。
> - 14 项「相当于合理便利的工作场所适配」← 取自**日本厚生劳动省发布的两个案例集**
> - ASD 特质：**自闭症量表（AQ）**
> - ADHD 特质：**成人 ADHD 自评量表（ASRS）**
> - 结局：**职场适应不良（Social Adaptation Self-evaluation Scale）**
> - 统计：**logistic 回归，报告 OR 与 95% CI**

### 2.2 结果：在「高 ADHD 特质」劳动者中，**没有**适配 → 职场适应不良的 OR

| 适配项 | 「无该适配」OR（高 ADHD 特质组） |
|---|---|
| 与主管定期开会 | **11.48（5.96–22.11）** |
| 弹性的工作时间 | **10.96（5.15–23.3）** |
| **安静的休息区** | **10.85（5.70–20.67）** ⚠️ 见下方警告 |
| 明确具体的工作指示 | **10.36（5.29–20.28）** |
| **专注工作的专属空间** | **7.92（4.39–14.27）** |
| 弹性休息时间 | **8.45（4.51–15.83）** |
| 工作量分担 | **8.44（4.65–15.29）** |
| 考虑任务专注度 | **8.53（4.64–15.71）** |
| 排班变更提前通知 | **7.78（4.26–14.2）** |
| 多种指示方式 | **7.18（3.84–13.41）** |
| 主动的工作场所沟通 | **13.24（6.77–25.88）** |
| 考虑感官刺激 | **9.06（4.97–16.51）** |
| 按个体优势分配任务 | **9.28（5.15–16.73）** |
| 多元化与残障意识培训 | **6.71（3.69–12.21）** |

「非高特质」组的全部 OR 落在 **1.82–3.45** 区间。

### 2.3 ⚠️⚠️ 三条必须一起读的限制（本文件最诚实的一段）

1. **🔴 14 个 OR 的量级高度相似（6.7–13.2），这本身是警报。**
   如果「安静的休息区」和「多元化意识培训」真的通过各自独立的机制起作用，它们的 OR 不应该这么接近。
2. **🔴 综述作者在摘要里**没有**给出这个疑问，但同类设计的标准解读是**：这些 OR 更可能反映**「一个总体上支持性的工作场所」的共同效应**，而不是 14 种适配各自的特异效应。横断面自报数据无法区分这两者。
3. **🔴 具体到「安静的休息区」这一项，有一处不一致**：在「高特质 + **有**该适配」这一格，OR 并不显著（在起草稿的原始记录中为 1.84，p = 0.135）。也就是说：**「没有安静区」与适应不良强相关，但「有安静区」并不能显著地保护高特质组。**
   ⚠️ 谨慎标注：该 p 值来自本轮抓取的表格记录，**建议引用此条前复核原文表格**。

🔴 **本 skill 应采用的表述**：
> **「在高 ADHD 特质的人身上，缺乏这十四项中的任意一项，都与更高的职场适应不良相关；而且这种关联在轻度特质的人身上也存在，只是弱得多。」
> **这是一个「缺少支持性环境 ↔ 适应不良」的关联，不是「某种适配有效」的因果证据。**
> **最有价值的推论是「关联的普遍性」：保护作用不限于重度人群。**

---

## 三、🅒 工作结构：证据在「一般人群」这一侧，而且比想象中硬

### 3.1 噪音与认知表现：最强的两个客观测量研究

**S4｜Jahncke, H. & Hallman, D. (2020).** *Objective measures of cognitive performance in activity based workplaces and traditional office types.* **Journal of Environmental Psychology, 71**, 101503.
DOI: **10.1016/j.jenvp.2020.101503** ｜OpenAlex 被引 **48** ｜🅒 **一般人群（办公室员工）**｜【同行评议论文，田野研究】｜可信度：**高**

**摘要原文全部数字**：
> **五个办公室，n = 113 名员工**，其中四个搬迁至 **ABW（activity-based working，活动式办公）**。由**声学专家实测各工作区的等效声级**。
> - **搬迁前**：共享/开放办公的员工在需高度集中的认知任务上**显著差 14%**，而独立办公室（cell offices）噪音低 **15 LAeq**
> - **搬迁后**：在**无噪音限制的 active zone**，员工表现显著差于**所有**其他工作区
> - 从 active zone 换到 quiet zone：**认知表现显著提升 16.9%**
> - **换到单人工作间：表现提升 21.9%**
> 结论原文：*"The results clearly demonstrate the importance for organizations to provide **quiet areas or rooms with few distractions** for employees working on tasks that demand concentration in an ABW."*

🔴 **这是本文件里唯一一个可以带具体百分比给出「换工作区」建议的研究**：**+16.9% / +21.9%，客观测量，非自报。**
⚠️ **必须标注：🅒 一般人群，不是 ADHD。**

**S5｜Gerlitz, A. & Hülsbeck, M. (2023).** *The productivity tax of new office concepts: a comparative review of open-plan offices, activity-based working, and single-office concepts.* **Management Review Quarterly.**
DOI: **10.1007/s11301-022-00316-2** ｜OpenAlex 被引 **28** ｜🅒 **一般人群（系统综述）**｜【同行评议论文，系统综述】｜可信度：**高**

**摘要原文要点**：
> 系统检索 2005–2022 年 **429 篇**关于办公概念与绩效的论文 → 严格筛选后 **46 篇**实证文章纳入。
> - **ABW 不仅负面冲击绩效，还影响员工满意度与健康**
> - **开放办公可以降低地产成本，但导致绩效下降，由此施加的「生产力税」超过初期的成本节约**
> - ABW 有增强协作与互动的潜力，但**依赖于专业且主动的管理**
> - *"In most cases, especially for **knowledge workers**, the **single office turns out to be the environment in which employees show the best individual and organizational performance**."*

**S6｜Bergefurt, L., Appel-Meulenbroek, R. & Arentze, T. (2026).** *Sound Distraction and Mental Health in the Workplace: The Role of Coping Strategies.* **Noise and Health.**
DOI: **10.4103/nah.nah_189_25** ｜🅒 **一般人群（办公室员工）**｜【同行评议论文】｜可信度：**中高**

🔴 **这一篇特别重要，因为它明确以「person-environment fit 理论」为框架**——它是 P-E fit 概念在工作场所研究里的直接实证应用。

**摘要原文全部关键系数**：
> 两个组织，**N = 214**。结构方程模型。
> - **感知分心 → 专注力：β = −0.67（t = −5.38）** ← 本文件里最大的一条
> - 压力性心境 → 耗竭 **β = 0.57（t = 6.64）**；→ 疲劳 **β = 0.21（t = 4.86）**
> - 压力性心境 ↔ 睡眠质量差 **β = −0.59（t = −4.42）**；↔ 脱离 **β = −0.34（t = −2.88）**
> - 🔴 **不可懂背景音干扰 → 耗竭：β = 0.10（t = −2.99）**；**可懂语音干扰 → 耗竭：β = −0.11（t = −2.63，方向为逆）**
> - 噪音敏感者 → 压力性心境 **β = 0.19（t = 3.62）**；→ 采取回避型应对 **β = 0.42（t = 6.88）**
> - 🔴 **「缺乏专注空间」与「频繁的个体专注任务」放大了分心与干扰**
> ⚠️ **两个 β 的 t 值符号与系数符号不一致（β 为正但 t 为负；β 为负但 t 为负），摘要原文如此。引用前建议复核全文。**

🔴 **「可懂语音 vs 不可懂噪音」的分裂是本文件里最实用的一条发现**：
> **让人听到别人在讲话，和听到听不清的噪音，对认知与福祉的影响不是一回事。**
> 🔴 **这对 ADHD 尤其重要**（**标注为🅒→外推**）：很多「噪音敏感」的报告，实际测到的是**言语侵扰（speech interference）**，而不是 dB。
> **可操作后果**：「装隔音棉」和「减少说话的密度」是两种不同的干预，证据指向后者更有价值。
> **「频繁的个体专注任务」放大分心**这一条尤其反直觉——**问题不只是噪音源，而是「需要安静」与「必须待在噪音里」的冲突密度。**

### 3.2 🔴 温度与噪音：有一个直接的控制实验

**S7｜Brabrand, C., Inie, N. & Tell, P. (2023).** *Programming under the influence: On the effect of Heat, Noise, and Alcohol on novice programmers.* **Journal of Systems and Software, 190**, 111887.
DOI: **10.1016/j.jss.2023.111887** ｜🅒 **一般人群（大学生志愿者）**｜【同行评议论文，被试间实验】｜可信度：**中高**
> **N = 100**，随机分配到四条件之一：
> - **38 °C 的房间** / **约 80 dBA 的会话噪音** / **血液酒精 1.0‰** / 基线条件
> 两项编程任务（分析型「读程序」约 30 分钟；综合型「写程序」）。
> **结果**：
> - 🔴 **热：短期暴露对读与写程序均无显著影响**
> - 🔴 **会话噪音：显著影响「分析型」任务，但不影响「综合型」任务**
> - 酒精：显著恶化两种任务
> ⚠️ 🅒、新手程序员、30 分钟暴露、单一实验环境。**不可外推到 ADHD，不可外推到长期暴露。**
> 🔴 **但「噪音选择性损害分析型任务、不损害综合型任务」这一条，与 ADHD 的「优势—劣势不均衡（jagged）」直觉方向一致**，是一个值得记录的模式（**标注为🅒模式巧合，非证据**）。

### 3.3 远程/混合办公：目前唯一的大规模 RCT

**S8｜Bloom, N., Han, R. & Liang, J. (2024).** *Hybrid working from home improves retention without damaging performance.* **Nature, 630**, 920–925.
DOI: **10.1038/s41586-024-07500-2** ｜OpenAlex 被引 **302** ｜🅒 **一般人群（中国科技公司员工）**｜【同行评议论文，RCT】｜可信度：**高**

**摘要原文全部数字**：
> **六个月随机对照试验，1,612 名员工**，一家中国科技公司，2021–2022 年。
> - **混合办公提高了工作满意度，离职率降低三分之一**
> - **离职率的下降在非管理者、女性员工和长通勤者中显著**
> - **零等价检验（null equivalence tests）：混合办公在随后两年的绩效评级上没有影响**
> - **没有证据显示两年内晋升有差异（总体或任何主要亚组）**
> - **零等价检验：对计算机工程师写的代码行数没有影响**
> - 🔴 **395 名管理者在实验前后改变了看法：实验前认为混合办公对生产力有「平均 −2.6%」的负面影响 → 实验后变为「+1.0%」的正向影响**
> 结论：*"a hybrid schedule with **two days a week** working from home **does not damage performance**."*

🔴 **两条对 ADHD 尤其相关**：
1. **「减少一天必须暴露于办公室噪音与打断」目前是唯一有 RCT 支持的办公结构变更**（🅒，但效应大、设计强）。
2. **管理者信念的修正（−2.6% → +1.0%）是硬数据。** 它证明了一件事：
   > **「什么样的环境对 ADHD 有益」这个信念，本身就是环境适配的一部分——因为它决定了管理者会不会批准这些适配。**

### 3.4 即时通讯 / 异步 vs 同步：证据方向明确但人群是科学家与知识工作者

**S9｜Walsh, J.P. & Maloney, N.G. (2007).** *Collaboration Structure, Communication Media, and Problems in Scientific Work Teams.* **Journal of Computer-Mediated Communication, 13**(1).**
DOI: **10.1111/j.1083-6101.2007.00346-x** ｜🅒 **一般人群（四领域科学家）**｜【同行评议论文，调查】｜可信度：**中高**
> 综述工作组织结构特征与协作问题的关系，并用四个领域的科学家调查数据做检验。
> - 两类问题：**协调与误解问题**；**文化差异与信息安全问题**
> - 协调问题与**规模、距离、相互依赖、科学竞争**正相关
> - 🔴 **「Email use is associated with reporting fewer coordination problems, but not fewer problems of culture and security」**
> - 🔴 **「neither phone use nor face-to-face meetings significantly reduces problems」**
> ⚠️ 🅒、2007 年、科学家样本。**这是一条容易被误用的证据**：它说的是「面对面会议不能显著减少协作问题」，**不是**「面对面会议对注意力有害」。两回事。

**S10｜Züger, M., Müller, S.C., Meyer, A.N. & Fritz, T. (2018).** *Sensing Interruptibility in the Office.* **CHI Conference on Human Factors in Computing Systems.**
DOI: **10.1145/3173574.3174165** ｜OpenAlex 被引 **66** ｜🅒 **一般人群（软件开发者）**｜【同行评议会议论文，田野研究】｜可信度：**中高**
> 两周田野研究，**13 名职业软件开发人员**，采集计算机交互 + 心率 + 睡眠 + 体力活动数据。
> **可打断性预测准确率**：计算机交互数据 **74.8%**；生理数据 **68.3%**；两者合并 **75.7%**。

**S11｜Züger, M., Meyer, A.N., Fritz, T. & Shepherd, D.C. (2019).** *Reducing Interruptions at Work with FlowLight.*（book chapter）
DOI: **10.1007/978-1-4842-4221-6_23** ｜🅒 **一般人群**｜【同行评议论文（会议论文集章节）】｜可信度：**中高**
> FlowLight = 桌上一盏小 LED 灯，根据计算机交互计算使用者当前**是否可被打断**，用红黄绿灯色告知同事。
> 🔴 **大规模研究，449 名参与者：FlowLight 使打断次数减少 46%。**
> 同时观察到：**对打断危害的觉察上升，生产力主观感受上升。**
> 🔴 **注意机制**：**打断减少 46%，但只减少到「别人知道现在不该打断你」这个程度——没有一个字是劝对方自律的。**
> **这就是环境适配与自我管理的分界线：把「判断该不该打断」从对方身上拿走，放到一个双方都看得见的信号上。**

---

## 四、合理便利 / 适配的效果：🔴 没有 ADHD-specific 的 RCT

### 4.1 最接近的、也是唯一做过效果 meta 分析的证据

**S12｜Lauder, K.M. (2021).** *A critical examination of the evidence for effective reasonable adjustments for adults with attention deficit hyperactivity disorder in the workplace.*（博士论文，Birkbeck, University of London）
DOI: **10.18743/pub.00046080** ｜【学位论文】｜可信度：**中**（方法透明，但非同行评议）

**摘要原文全部要点**：
> 批判实在主义范式 + 混合方法，审视成人 ADHD 工作场所合理便利的有效证据。
> - **快速证据评估：对 12 种成人 ADHD 测量工具的评估**；**161 项干预研究的系统综述** → 结论：*"a **gap in research evidence for work-related support** and understanding of ADHD"*
> - 🔴 **「Findings indicated a small positive effect」** ← 对 **12 项**研究做 meta 分析，考察支持措施对**工作相关结局**的有效性
> - **实践证据 vs 研究证据的对照**：对职场网络建议做模板分析 → **经理人在适配决策中处于核心位置**
> - 🔴 **门控者（gatekeeper）实验：对 62 名经理/HR 专业人员做 e-learning（37 实验 / 25 对照），随机对照设计**
>   - **增加了对合理便利与 ADHD 的知识，并改善了整体的批准（granting）**
>   - **实验组的刻板化言论减少**
>   - **参与者更能论证该适配为何有益**
>   - **这一提升外溢到了其他残障类型**

🔴🔴 **这可能是整个维度 2 里对实务最有用的一条**：
> **对适配效果最大的干预点，可能既不是给员工的空间，而是给经理人的知识。**
> 而且它**是一个真正的 RCT**，虽然 n=62、且对象是**经理而非员工**。
> 🔴 **注意它的证据边界**：结局是「**批准率**」与「**论证质量**」，**不是员工的绩效或健康结局**。批准的便利是否真的改善了结果，这篇论文没测。

### 4.2 员工侧的定性证据（🅓，但主题高度一致）

**S13｜Oscarsson, M., Nelson, M., Rozental, A., Ginsberg, Y., Carlbring, P. & Jönsson, F.U. (2022).** *Stress and work-related mental illness among working adults with ADHD: a qualitative study.* **BMC Psychiatry, 22**, 751.
DOI: **10.1186/s12888-022-04409-w** ｜PMID **36451126** ｜🅓 **ADHD 人群，n=20，半结构化电话访谈**｜【同行评议论文，定性】｜可信度：**中**
> **20 名在职 ADHD 成人**。定性内容分析。
> 三个主题、八个子类：**Working and living with ADHD / Needs / Special abilities**
> 子类包括：具体困难；关系与合作；**负面后果**；**规划、优先级、组织与结构**；**支持、干预、便利与辅助工具**；开放、理解与接纳；策略；**长处与品质**
> 🔴 **结论原文（关键）**：*"**where organizational support is lacking, much in terms of accommodations and aids is up to the employee**, and the **disclosure of diagnoses may be associated with great dilemma**."*
> 🔴 **这句话是本维度所有定性证据的公共主题**：
> **没有组织支持时，适配的责任落到员工自己身上——而这恰恰是本 skill 认为不可行的那个方案。**

**S14｜Hedlund, Å. & Jordal, M. (2024).** *Feeling like an untapped resource. Experiences of working life among nurses with ADHD and/or autism: An interview study.* **International Journal of Nursing Studies, 158**, 104857.
DOI: **10.1016/j.ijnurstu.2024.104857** ｜PMID **39032246** ｜🅓 **ADHD 和/或自闭症护士，n=17**｜【同行评议论文，定性】｜可信度：**中**
> **17 名瑞典护士**（ADHD 和/或 autism），半结构化访谈，定性内容分析。
> 一个总主题 + 七个子主题：
> 1. 对工作充满热情
> 2. **有可用的长处与才能**
> 3. 🔴 **「a stressful and disturbing work environment inhibits personal strengths」** ← **有压力且令人不安的工作环境抑制了个人的长处**
> 4. 🔴 **管理者表现善意但缺乏知识与资源**
> 5. 感到被赏识但在同事中「与众不同」
> 6. 使用多种策略来维持工作生活
> 7. 面向不确定的未来
> 🔴 **子主题 3 是本文件里对「环境适配」这个概念最精确的一句实证描述**：
> **长处是在场的，环境把它压住了。**
> 这与 Dale Archer 的「not in spite of but because of」正好相反——**这些护士的长处不是因为 ADHD 才有的，而是被环境决定了能不能用出来。**

**S15｜Loison, A. & Balou, M. (2026).** *ADHD and Autism in the Irish Workplace.* **DBS Applied Research and Theory Journal, 3**(1).**
DOI: **10.22375/dbs.v3i1.182** ｜🅓 **ADHD 和/或 ASD 专业人士，n=10**｜【同行评议论文，定性】｜可信度：**中低**（期刊层级较低）
> **10 名跨 X/M/Z 世代的爱尔兰专业人士**；归纳式主题分析。
> 🔴 **本地制度事实**：*"neurodiversity is **not explicitly recognised in employment law**" in Ireland.*
> 结论把职场包容定义为**一个循环的、非线性的持续协商过程**，而不是一个固定结果；强调组织不应把包容**建立在个人披露或经理的自由裁量之上**。

**S16｜Kan, D.D.C., Chuai, A., Bong, K., Ang, M.W., Ang, E.L. & Lim, J. (2026).** *Understanding the workplace needs of autistic adults in Singapore.* **Frontiers in Psychiatry.**
DOI: **10.3389/fpsyt.2026.1825357** ｜🅑 **ASD，n=20**｜【同行评议论文，参与式定性研究】｜可信度：**中**
> 20 名自闭症成人（≥3 个月工作经验），小焦点小组 + 反思性主题分析。
> 关键：*"Workplace barriers for autistic employees often stem from **assumed neurotypical norms rather than individual deficits**."* 参与者报告的困难：**工作流程含糊、隐性的社会期待、执行功能要求**，并被归为一个错配：***"a mismatch between workplace structures and neurodivergent ways of working."***
> ⚠️ **这是 ASD，不是 ADHD。** 但「结构 vs 神经多样性工作方式之间的错配」这句话，是本 skill 标题本身的实证对应物。

### 4.3 神经多样性整体的证据（🅑）

**S17｜Koldas, M., Dounavi, K., MacCárthaigh, M. & Dillenburger, K. (2025).** *Facilitators and Barriers to Employment of Neurodivergent Individuals: A Systematic Literature Review of Employee and Employer Experiences.* **Journal of Autism and Developmental Disorders.**
DOI: **10.1007/s10803-025-07139-6** ｜OpenAlex 被引 **2** ｜🅑 **神经多样性（以 ASD 为主）**｜【同行评议论文，系统综述】｜可信度：**中高**
> **56 项研究、12 个国家**；纳入 **4,909 名神经多样性员工**、**2,041 名非神经多样性参与者（多为同事）**、近 **300 名**监督者/经理/雇主。
> - 🔴 **障碍**：**监督者缺乏意识与教育**，尤其当他们**把社会性困难归因于个人特质**时，导致**纪律处分或排斥**
> - ✅ **促进因素**：**支持性的经理**、**弹性与定制化的工作安排**、**辅助技术的可获得性**
> - 收益：留任改善、投入度提升、组织形象提升

**S18｜Bölte, S., Carpini, J.A., Black, M.M., Toomingas, A., Jansson, F. & Marschik, P.B. (2024).** *Career Guidance and Employment Issues for Neurodivergent Individuals: A Scoping Review and Stakeholder Consultation.* **Human Resource Management.**
DOI: **10.1002/hrm.22259** ｜OpenAlex 被引 **33** ｜🅑 **神经多样性**｜【同行评议论文，范围综述 + 利益相关方咨询】｜可信度：**高**
> **78 篇文献**的范围综述 + 多方利益相关方咨询。
> 产出**九个主题**，其中与本 skill 直接相关的是：**person-job fit（人与工作适配）** 与 **occupation and industry fit（职业与行业适配）**——**这两个是被分开的**。
> 结论明确指出文献存在**持续的方法学局限**。

**S19｜Pryke-Hobbes, A., Davies, J., Heasman, B., Livesey, A., Walker, A. & Pellicano, E. (2023).** *The workplace masking experiences of autistic, non-autistic neurodivergent and neurotypical adults in the UK.* **PLoS ONE, 18**(10):e0290001.
DOI: **10.1371/journal.pone.0290001** ｜OpenAlex 被引 **90** ｜🅑/🅒 **285 名自闭症 + 88 名非自闭症神经多样性 + 89 名神经典型成人**｜【同行评议论文，定性】｜可信度：**高**
> **285 名自闭症、88 名非自闭症神经多样性、99 名神经典型成人**；反思性主题分析；场景 = **职场**（masking 预期极高的环境）。
> 关键发现：三组都认为职场 masking 是对多种社会性职场挑战的**适应性反应**，通常是**为抵御负面社会与雇佣后果而采取的策略**。
> 🔴 **自闭症与非自闭症神经多样性参与者报告了「独特的 masking 压力」，原因是职场与社会对神经多样性的理解有限。**
> 🔴 **本 skill 应引用的那一条**：
> **masking 的功能是**让一个人在**不适合他的结构里**看起来正常。
> 因此**减少 masking 需求（让结构适配）**与**训练 masking 能力**是两条方向相反的干预，而文献与从业者经验都更支持前者。

---

## 五、🅓 Sarah Greenberg 的「jagged cognitive profile」：🔴 核实结果

### 5.1 这个说法的出处

- 【机构/临床人员表述，经媒体引述】Sarah Greenberg（持证心理治疗师，Understood.org）在谈 Dale Archer 的 Fast Company 文章中提出：neurodiversity 制造的是 **"jagged profiles"**——「许多有神经差异的人在某些领域表现超常，在另一些领域表现不足」，**而不是**一条 continuum。
  （该引述已由本项目 `references/dale-archer-cautionary-research/04-external-views.md` §3.4 收录）
- 任务书提示的核查目标之一是 Belardinelli 等人关于 ASD/ADHD 能力剖面的实证。

### 5.2 🔴 核实结论：**未找到任何同行评议的实证版本**

本次执行的检索与结果：

| 检索路径 | 查询 | 结果 |
|---|---|---|
| PubMed esearch | `"jagged cognitive profile" neurodiversity` | **COUNT: 0** |
| OpenAlex search | `jagged cognitive profile neurodiversity` | 无相关命中 |
| Crossref | `"jagged cognitive profile" neurodiversity Greenberg` | 无相关命中 |
| OpenAlex | `Sarah Greenberg neurodiversity` | 前列为 Borsotti et al. (CSCW) 等，**无 Greenberg 的同行评议成果** |
| PubMed esearch | `Belardinelli autism`（任务书点名的作者） | 唯一命中是一篇 **TikTok 准确性研究**（Belardinelli 为共同作者），**不是**能力剖面研究 |

🔴 **因此本 skill 必须这样标注**：
> **「jagged cognitive profile」目前是一个【机构/临床人员的表述】，不是一个已被量化的构念。**
> **它作为修辞很有力量，作为测量则没有对应工具。**

### 5.3 🔴 但「锯齿状/尖峰剖面」的实证版本存在——**在 ASD 那边，不在 ADHD 那边**

**S20｜Wilson, A.C. (2023).** *Cognitive Profile in Autism and ADHD: A Meta-Analysis of Performance on the WAIS-IV and WISC-V.* **Archives of Clinical Neuropsychology, 38**(8).**
DOI: **10.1093/arclin/acad073** ｜OpenAlex 被引 **43** ｜【同行评议论文，meta 分析】｜可信度：**高**

**摘要原文（关键句逐字）**：
> "Scores were analyzed from **over 1,800 neurodivergent people reported across 18 data sources**."
> *"Autistic children and adults performed in the **typical range for verbal and nonverbal reasoning**, but scored **~1 SD below the mean for processing speed** and had slightly reduced scores on working memory. **This provides evidence for a 'spiky' cognitive profile in autism.**"*
> *"Performance of children and adults with **ADHD was mostly at age-expected levels, with slightly reduced scores for working memory.**"*
> 🔴 **结论原文**：*"…**autism appears to be associated with a cognitive profile of relative strengths in verbal and nonverbal reasoning and a weakness in processing speed. Attention deficit hyperactivity disorder appears LESS associated with a particular cognitive profile.**"*
> ⚠️ 作者同时警告：*"the pattern of performance on the Wechsler tests is **not sufficiently sensitive or specific to use for diagnostic purposes**"*

🔴🔴 **这是本文件里对「jagged profile」最重要的一条发现**：
> **「锯齿状剖面」这个模型有实证支持——但支持它的是自闭症，不是 ADHD。**
> **ADHD 在韦氏量表上的表现「大多在年龄预期水平」，只有一个轻微的工作记忆下降——也就是说，在最标准的智力剖面工具上，ADHD 看起来相当不「锯齿」。**
> 🔴 **这对本 skill 有一个直接后果**：
> **不要把「jagged cognitive profile」当作 ADHD 者的普遍事实来陈述。**
> **更准确的说法**：ADHD 的异质性主要体现在**症状维度**（在注意力不集中 vs 多动冲动之间，以及它们各自在工作与生活不同领域的后果上——见 `03-time-and-interruption.md` §2.4 与 `01-entrepreneurship.md` §2.1），**而不是在智力剖面上**。
> ⚠️ **注意术语溯源**：「spiky profile」这个词在文献中的常用出处是 **Doyle (2021)**，不是 Greenberg；Greenberg 说的是 **jagged**，且是在**大众媒体**语境下。

**S21｜Lenhard, A. & Daseking, M. (2022).** *Accounting for Intraindividual Profiles in the Wechsler Intelligence Scales Improves the Prediction of School Performance.* **Children, 9**(11), 1635.
DOI: **10.3390/children9111635** ｜【同行评议论文】｜可信度：**中高**
> 用 WISC-IV / WISC-V 德国标准化样本做 lasso 回归。
> - GAI（一般能力）与 CPI（认知效率）**在多数情况下并不能显著改善对学业成绩的预测**
> - 🔴 **但当 CPI 与 GAI 的个体差异很大时，FSIQ 在小学阶段就失去了预测效度**
> - 此时**阅读与写作技能由 CPI 预测最好**，而**数学技能受限于 CPI 与 GAI 中的较低者**
> 🔴 **这条对「适配」极其有用**：**总体 IQ 在个体剖面高度不均的人身上是会失效的。**
> **实务含义**：为一个人做适配评估时，**不要用一个被平均掉的分数**，要看他哪一块塌了。
> ⚠️ 样本为**儿童**（德国标准化样本），非成人职场。

**S22｜Marx, I.M., Höpcke, C., Berger, C., Wandschneider, R. & Herpertz, S.C. (2013).** *The Impact of Financial Reward Contingencies on Cognitive Function Profiles in Adult ADHD.* **PLoS ONE, 8**(6):e67002.
DOI: **10.1371/journal.pone.0067002** ｜OpenAlex 被引 **50** ｜🅐 **成人 ADHD**｜【同行评议论文】｜可信度：**中高**
> **ADHD n = 38 vs 匹配对照 n = 40**，18–40 岁，六个成熟实验范式（执行功能、注意力、**时间知觉**、**延迟厌恶**）。
> - ADHD 组受损：stop-signal 遗漏错误、n-back 正确率、CPT 反应时变异、**时间复现准确性**
> - 🔴 **「reward normalized time reproduction accuracy」**（奖励使时间复现准确性归一化）
> - 🔴 **「when rewarded, subjects with ADHD exhibited longer reaction times and fewer false positives in the continuous performance task, which suggests the use of strategies to prevent impulsivity errors」**
> 🔴 **这是「锯齿状」在成人 ADHD 上最接近的一条实证**：
> **在同一个任务里，ADHD 组默认状态更差，但在有奖励时改用策略（反应变慢、误报变少）反而更好。**
> 🔴 **环境含义（本 skill 的核心操作原则之一）**：
> **把奖励显性化、即时化、结构化，就是在环境里制造那个「有奖励」的条件。**
> ⚠️ n=78 的实验研究，实验室任务，**只验证了一种奖励形式（财务奖赏）**。

---

## 六、🅓 一个直接来自 ADHD 社群的数据集，以及它的自我警告

**S23｜Jameson, T.P., Grabarski, M.K., Morales Arana, M. & Santos, P.A. (2026).** *What makes work sustainable for adults with ADHD? Interpreting workplace strain and support through Reddit data.* **Frontiers in Psychology.**
DOI: **10.3389/fpsyg.2026.1820248** ｜🅓 **Reddit r/ADHD 社群的 277 个职场相关讨论串**｜【同行评议论文，定性（反思性主题分析）】｜可信度：**中**

**摘要原文（关键句逐字）**：
> 采用 **Job Demands-Resources（JD-R）框架**作为敏感性透镜，分析 **277 个职场相关讨论串**。
> 🔴 **"workplace features such as **meetings, deadlines, and disclosure were not described as either inherently demanding or supportive**. Instead, contributors emphasized that these conditions were **experienced differently across contexts**, particularly regarding **autonomy, performance management, structuring of work, and identity-related dynamics**."**
> "workplace strain and sustainable functioning were patterned around concepts such as **the social impact of disclosure, work design aspects and invisible labor**."
> 🔴 **作者自己的警告（必须一起引用）**：*"these results reflect **collective meaning-making within a large online ADHD community rather than direct representations of organizational structures or causal mechanisms**."*

🔴 **这是本文件里对本 skill 最有价值的一条「反向约束」**：
> **在最大的 ADHD 职场社群数据里，「会议」和「截止日期」本身既没有被说成天然有害，也没有被说成天然有利。**
> **决定结果的是四个调节变量：自主权、绩效管理方式、工作如何被结构化、以及身份相关的动态（尤其是披露的后果）。**
> 🔴 **这直接反驳了任务书里「什么样的工作结构有害」的那种清单式提问方式。**
> **诚实的答案不是一份「开放办公有害 / 封闭办公有益」的清单，而是：**同一个会议，对一个有决策权的人和没有决策权的人，代价不同。**
> ⚠️ 社群的自我选择偏差极强（愿意在 Reddit 上长篇讨论职场困境的人，不等于全体 ADHD 员工）。**不可用于估计任何比例。**

---

## 七、HCI 视角：一个关于「谁定义适配」的方法学批评

**S24｜Spiel, K., Hornecker, E., Williams, J. & Good, J. (2022).** *ADHD and Technology Research – Investigated by Neurodivergent Readers.* **CHI Conference on Human Factors in Computing Systems.**
DOI: **10.1145/3491102.3517592** ｜OpenAlex 被引 **143** ｜🅓 **ADHD 人群的批判性文献综述（由神经多样性研究者本人做）**｜【同行评议会议论文】｜可信度：**高**

**摘要原文全部三条发现**：
> 1. **"technologies are largely used to 'mitigate' the experiences of ADHD which are perceived as disruptive to neurotypical standards of behaviour"**
> 2. **"little HCI research in the area invites this population to co-construct the technologies or to leverage neurodivergent experiences in the construction of research aims"**
> 3. **"participant resistance to deficit frames can be read within the researchers' own accounts of participant actions"**

🔴 **第 1 条对本 skill 是一记直接的方法学警告**：
> **现有的「工作适配」研究，其隐含的问题是「如何让 ADHD 者更接近神经典型标准」。**
> **这是一个不问当事人就设定的问题。本 skill 必须显式地把问题反过来问一遍。**

---

## 八、🅑🅓 神经多样性的「生态位」表述：症状与环境的互相塑造

**S25｜Ruse, J.N. & Rhodes, P. (2026).** *Adult ADHD in Cultural Ecosocial Niches: Exploring the Rise of Adult ADHD in Context.* **Culture, Medicine and Psychiatry.**
DOI: **10.1007/s11013-025-09958-9** ｜🅓 **7 名近期获得成人 ADHD 诊断的澳大利亚女性**（深度访谈 + photo-voice）｜【同行评议论文，定性】｜可信度：**低-中**（n=7）

**摘要原文关键句**：
> 提出**「文化生态社会位」（cultural ecosocial niche）理论**：*"symptoms emerge within **specific cultural and social contexts** rather than solely from neurobiological differences."*
> 关键发现：参与者**主动建构并栖居**着他们的文化生态社会位，在其中**其特质与其社会文化环境达成功能性契合**。
> 这些位从小到大：采纳「神经多样性」的宏观文化框架以建立肯定性的身份与社群，**到在快节奏角色中找到微观社会职业位，在那里他们的认知风格成为一种优势**。
> 🔴 **「反馈回路」**：*"the environment (such as a supportive social group or a demanding job) **reinforced the very traits and beliefs that initially attracted them to that niche**."*
> 🔴 **作者的收束句**：*"This study **challenges the notion that psychiatric symptoms are confined solely within a person or solely outside in the environment**. Instead, it provides a concrete example of how symptoms and their meanings appear **at the intersection of both**."*

⚠️ **n=7，全部为女性、近期诊断、澳大利亚。** 证据等级低。
🔴 **但这是本文件里唯一一条把「适配」讲成双向过程的材料**——它同时解释了**为什么某些环境会放大某些特质**（S22 的奖励实验是它的微观对应），和**为什么「找到适配的环境」之后人会变**。

---

## 九、数字冲突清单（本维度）

| # | 冲突点 | A 方 | B 方 | 状态 |
|---|---|---|---|---|
| 1 | **物理工作场所适配是否有用** | Suzuki 2026：高特质组「无适配」OR **6.7–13.2**，14 项全部显著；S3 原文自身提示这更可能是「总体支持性环境」的共同效应 | **Weber et al. 2022 系统综述（319→20 篇）："There is insufficient evidence to fully evaluate the usefulness of adjustments"** | 🔴 **未解决，且不是同一类主张**。前者是关联，后者是「证据不足以评估因果」。**两者都成立** |
| 2 | **噪音对认知表现的影响（一般人群）** | **Jahncke & Hallman 2020**：开放办公 vs 独立办公室 **差 14%**；换到安静区 **+16.9%**、换到单人间 **+21.9%**（客观测量，n=113） | 同领域另有一支文献报告开放办公噪音**未**降低即时认知任务表现（详见起草记录中的冲突项）；且 Pitchforth et al. 2020（*PLoS ONE*）与 Gerlitz & Hülsbeck 2023 在协作维度上给出不同侧重 | ⚠️ **本轮未能取回冲突方原文的完整数据**，⚠️ **不写具体数字。** 待补 |
| 3 | **「开可懂语音」vs「开不可懂噪音」** | Bergefurt et al. 2026：可懂语音干扰与耗竭呈**反向**关系（β = −0.11），不可懂背景音为**正向**（β = 0.10） | 本轮未见直接对立研究 | ⚠️ **单一研究，且摘要中两个 β 的 t 值符号不一致，引用前须复核全文** |
| 4 | **面对面会议是否有害** | 常见的注意力直觉：会议打断深度工作 | **Walsh & Maloney 2007**：*"neither phone use nor face-to-face meetings significantly reduces problems"* —— 但这说的是**协作问题**，**不是注意力** | ⚠️ **表面冲突，实为不同构念。** 本 skill **必须**明确区分「会议对协作」与「会议对专注」 |
| 5 | **开放办公 vs 专注** | Gerlitz & Hülsbeck 2023：**单一办公室**在知识工作者中个人与组织绩效最佳；ABW 有协作潜力但依赖主动管理 | Jahncke & Hallman 2020 证实噪音区/单人间的认知优势 | 🟢 **大体一致**。冲突主要在对「协作收益」的量化上 |
| 6 | **锯齿状剖面是不是 ADHD 的事实** | Greenberg 的媒体表述；Brabrand 2023 显示噪音选择性损害分析型任务 | **Wilson 2023（1,800+ 人，18 个数据源）：ADHD 在 WAIS/WISC 上「大多在年龄预期水平」；「spiky profile」是**自闭症**的发现有证据支持 | 🔴 **重要冲突。** 本 skill **不应**把「jagged」当作 ADHD 的普遍事实陈述 |
| 7 | **远程办公是否损害绩效** | 管理层普遍看法：损害生产力、创新、职业发展 | **Bloom, Han & Liang 2024, Nature, n=1,612, RCT**：无绩效损害；离职率降 1/3；管理者看法从 −2.6% 修正到 +1.0% | 🟢 **RCT 站在「不损害」一边。** 冲突来自**未被控制的信念**，不来自数据 |
| 8 | **适配的责任归属** | 「你需要的只是知道自己需要什么」 | Oscarsson 2022：无组织支持时适配责任落在员工身上；Koldas 2025：最大障碍是**监督者缺乏知识**且把社会困难归因于个人；Loison & Balou 2026：不应把包容建立在**个人披露或经理裁量**上；Lauder 2021：给经理人的 e-learning **提高了批准率** | 🟢 **四条独立证据指向同一侧：门控在经理/组织一侧。** |

---

## 十、本 Skill 对「什么环境适配得好」的可辩护表述边界

**✅ 有 ADHD-specific 证据支持（可以写进 skill）：**
1. 「**没有**安静/低干扰的专属空间 ↔ 更高的职场适应不良」有 ADHD 特质分组数据（S3）；噪音与专注的因果机制有一般人群客观数据（S4，14% / +16.9% / +21.9%）。
2. 「**可懂语音干扰 ≠ 不可懂噪音**」两者机制不同（S6）。
3. 「**每周两天远程**」是唯一有 RCT 支持的结构变更，且不损害绩效（S8）。🔴 **标注为一般人群证据 + ADHD-specific 证据缺失。**
4. 「**把可打断性变成可见信号**」（FlowLight，打断 −46%）——干预的是**别人要不要打断你**这个决定，不是你的自控（S11）。
5. 「**经理人的知识**」是适配生效与否的瓶颈；给经理做 e-learning 可提高批准率并减少刻板化言论（S12）。

**⚠️ 只有一般人群证据（必须标注为外推）：**
- 开放办公 vs 封闭办公室对 ADHD 的影响（S1 明确说 ADHD-specific 版本未被检验）
- 关闭 / 保留即时通讯、异步 vs 同步
- 会议密度对深度工作的影响

**🔴 没有证据（不得作为建议写出）：**
- 「ADHD 适合做需要频繁打断的工作」/「不适合做深度工作」——**没有研究检验过这个二分**
- 「ADHD 应该避免夜班/轮班」——见 `03-time-and-interruption.md` §四，**整个领域是空白**
- 温度、座位朝向、光线对 ADHD 的影响——🔴 **本轮检索三项零命中**（见 §四下方说明）

> **本 skill 若要给出一套环境建议，其正确的证据姿态是：**
> **给出机制清晰、证据来自一般人群但方向一致的建议（安静空间、减少言语侵扰、可见的可打断信号、外部化的截止日期、每周两天远程），并对每一条诚实标注证据人群；**
> **同时把「对 ADHD 者的效应量」明确写成未知，而不是把它当成一个可以省略的技术细节。**

---

## 来源总表（本文件，25 个独立来源）

**🅐 ADHD 人群实证（5）**
1. **Suzuki, Nakazato, Ohtani & Ikeda (2026)** *Environ Health Prev Med* 31:62 — `10.1265/ehpm.26-00080` / PMID 42749630
2. **Sanders & Le Rossignol (2026)** *Work* — `10.1177/10519815261449927` / PMID 42132039
3. Wilson, A.C. (2023) *Arch Clin Neuropsychol* — `10.1093/arclin/acad073` ← **ASD 有 spiky 证据，ADHD 没有**
4. Marx, Höpcke, Berger, Wandschneider & Herpertz (2013) *PLoS ONE* 8:e67002 — `10.1371/journal.pone.0067002`
5. Lenhard & Daseking (2022) *Children* 9:1635 — `10.3390/children9111635`（儿童样本）

**🅑 神经多样性（以 ASD 为主）证据（4）**
6. **Weber, Krieger, Häne, Yarker & McDowall (2022)** *Applied Psychology* — `10.1111/apps.12431` ← **核心系统综述**
7. Koldas, Dounavi, MacCárthaigh & Dillenburger (2025) *J Autism Dev Disord* — `10.1007/s10803-025-07139-6`
8. Bölte, Carpini, Black, Toomingas, Jansson & Marschik (2024) *Hum Resour Manage* — `10.1002/hrm.22259`
9. Kan, Chuai, Bong, Ang, Ang & Lim (2026) *Front Psychiatry* — `10.3389/fpsyt.2026.1825357`

**🅒 一般人群实证（7）**
10. **Jahncke & Hallman (2020)** *J Environ Psychol* 71:101503 — `10.1016/j.jenvp.2020.101503`
11. **Gerlitz & Hülsbeck (2023)** *Manag Rev Q* — `10.1007/s11301-022-00316-2`
12. Bergefurt, Appel-Meulenbroek & Arentze (2026) *Noise Health* — `10.4103/nah.nah_189_25`
13. **Bloom, Han & Liang (2024)** *Nature* 630:920–25 — `10.1038/s41586-024-07500-2`
14. Brabrand, Inie & Tell (2023) *J Syst Softw* 190:111887 — `10.1016/j.jss.2023.111887`
15. Züger, Müller, Meyer & Fritz (2018) *CHI* — `10.1145/3173574.3174165`
16. Züger, Meyer, Fritz & Shepherd (2019) FlowLight — `10.1007/978-1-4842-4221-6_23`
17. Walsh & Maloney (2007) *J Comput Med Commun* 13(1) — `10.1111/j.1083-6101.2007.00346-x`

**🅓 定性 / 自报 / 社群数据（5）**
18. **Oscarsson, Nelson, Rozental, Ginsberg, Carlbring & Jönsson (2022)** *BMC Psychiatry* 22:751 — `10.1186/s12888-022-04409-w` / PMID 36451126
19. **Hedlund & Jordal (2024)** *Int J Nurs Stud* 158:104857 — `10.1016/j.ijnurstu.2024.104857` / PMID 39032246
20. **Jameson, Grabarski, Morales Arana & Santos (2026)** *Front Psychol* — `10.3389/fpsyg.2026.1820248`
21. Loison & Balou (2026) *DBS Appl Res Theory J* 3(1) — `10.22375/dbs.v3i1.182`
22. Ruse & Rhodes (2026) *Cult Med Psychiatry* — `10.1007/s11013-025-09958-9`

**🅓 方法学批评 / 学位论文（3）**
23. **Spiel, Hornecker, Williams & Good (2022)** *CHI* — `10.1145/3491102.3517592`
24. Pryke-Hobbes, Davies, Heasman, Livesey, Walker & Pellicano (2023) *PLoS ONE* 18:e0290001 — `10.1371/journal.pone.0290001`
25. **Lauder, K.M. (2021)** 博士论文, Birkbeck — `10.18743/pub.00046080`

---

## ⚠️ 本文件的已知缺口（诚实清单）

| 缺口 | 状态 |
|---|---|
| **ADHD-specific 的「开放办公 vs 独立办公室」对照实证** | 🔴 **不存在。** 已有一篇专门的范围综述（S1）记录这个空白 |
| **ADHD-specific 的合理便利 RCT（结局为员工绩效/健康）** | 🔴 **不存在。** 唯一 RCT（S12）的结局是**经理的批准率与论证质量** |
| **Sarah Greenberg「jagged cognitive profile」的同行评议实证版本** | 🔴 **不存在。** 四条检索路径全部零命中；Belardinelli 相关的 ASD 能力剖面研究亦未检索到 |
| **「jagged/spiky profile」在 ADHD 上的实证支持** | 🔴 **Wilson 2023 的结论恰恰相反**：ADHD 在韦氏量表上「大多在年龄预期水平」 |
| **ADHD × 光线 / 温度** | 🔴 **零命中。** 本轮 PubMed 三次不同检索式均无结果 |
| **ADHD × 座位 / 工位安排** | 🔴 **零命中。** |
| Bergefurt 2026 的两个 β 值符号与 t 值方向不一致 | ⚠️ **摘要原文如此，须复核全文后方可引用** |
| 「安静的休息区」在高特质+有适配格中不显著（OR 1.84, p=0.135） | ⚠️ 来自起草稿的表格记录，**引用前须复核原文表格** |
| §九 冲突 #2 的冲突方原文数据 | ⚠️ **本轮未取回完整数据，故未写数字。** 待补 |

---

**⚠️ 提示注入记录**：本次调研未发现针对本 Agent 的提示注入文本。
**说明**：本文件全部数据来自 NCBI E-utilities、OpenAlex、Crossref、Europe PMC 的 API 直连返回。起草 subagent 的中间记录中曾出现**凭记忆写出未经验证的 DOI**（如 Stothart 2021 通知成本论文、Bloom 2024 Nature 论文）的情况，**均已通过 Crossref 逐条交叉核验并修正**；`Bloom 2024` 的 DOI `10.1038/s41586-024-07500-2` 与被引数（302）已由本 Agent 重新核验。**凡未能核验者一律不写入数字。**
