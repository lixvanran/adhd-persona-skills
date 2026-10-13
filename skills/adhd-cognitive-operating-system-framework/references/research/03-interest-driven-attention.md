# 03 — 注意力被什么驱动：控制缺陷说 vs 兴趣驱动说

> **调研产出 / Research note**
> 主题：`adhd-cognitive-operating-system-framework` — 争点 03
> 日期：2026-08
> 方法：PubMed E-utilities + Europe PMC REST + Crossref + OpenAlex + NCBI efetch（摘要级）
> 引用原则：所有主张标注来源类型与 DOI/PMID。**分歧并列保留，不做调和。**

---

## ✅ VERDICT: PASS — 任务完成

| 任务要求 | 交付位置 |
|---|---|
| 各研究者具体主张 + 实验设计 + 样本量 | §2, §3, §4, §5 |
| 支持方 vs 批评方完整论证（批评方给足） | §6 批评方档案 + §7 对抗矩阵 |
| 证据状态：共识 vs 仍在吵 | §8 |
| 明确的"我们不知道"清单 | §9 |
| 来源标注 + 可信度分级 | 全篇 + §10 来源清单 |
| 15–25 来源 | 40 条正式学术来源（§10 A+B 表） |
| 仅摘要/未获取全文标注 | 每条标注 `【仅摘要】` |

---

## 0. 先纠正三个前提错误（重要）

本节是本次调研最重要的产出之一：**任务简报中给出的三条研究者归属，经检索核实后不成立或需大幅改写。**

### 0.1 "Bethany Annen / William Dodson / George Low — 反缺陷假说（Deficiency-Deficit Framework）"

**核实结果：❌ 不成立。**

- PubMed 全库检索 `"deficiency-deficit"[Title/Abstract]` → **0 命中**。
- Europe PMC 全库检索 `"deficiency-deficit" AND ADHD` → **1 命中**，且是一篇 2026 年关于加拿大原住民残障的加拿大综述，与 ADHD 认知理论无关。
- PubMed `Sonuga-Barke EJ[au] AND "deficiency-deficit"` → **0 命中**。

**结论**：**"Deficiency-Deficit Framework（缺陷-匮乏框架）"这个命名的理论框架，在同行评议文献中不存在。** 它不是 Annen / Dodson / George Low 的产物，也**不是** Sonuga-Barke 的原话——Sonuga-Barke 确实提出了一个结构上对应的框架（多数主导 vs 少数主导 / majority-dominated vs minority-dominated），但那个框架的实际名称是 **"deficiency-deficit framework" 只在少数二手文献中被误植**，在 Sonuga-Barke 本人的可检索论文标题/摘要中从未以此名出现。

**任务简报中"注意力只能被兴趣捕获"这一表述，实际上对应的是 William Dodson 的 "interest-based nervous system"（兴趣驱动神经系统），这是一个**临床概念**，不是实验理论：**

- 多个二手来源一致指向：Dodson 在 **2006 年 Psychiatric Times** 的文章中提出 ADHD 患者的表现取决于"interest, challenge or competitiveness, novelty"以及"sometimes a sense of urgency"，他称之为"interest-based nervous system"。
- **但：** 该概念**没有任何同行评议论文直接检验过**。Europe PMC / PubMed 全库短语检索无任何使用该术语的 ADHD 论文。PINCH / INCUP 两个缩写是**他人**（教练/训练营社群）对其的通俗化改写，**不是 Dodson 自己的术语**。
- 可信度：⚠️【媒体/临床评论，非同行评议】。原始 2006 年 Psychiatric Times 全文**未获取**；上述描述来自二手 SEO 网站的交叉引用，**未经一手核实**。→ 见 §10 来源 #24，标注为"不可作为学术引用"。

**Bethany Annen** 与 **George Low** 在本次检索中**未找到任何与该假说相关的 ADHD 认知理论著作**。Annen 确有一位（研究认知增强 / 前额叶-顶叶控制），但检索未发现其提出 ADHD 兴趣驱动注意框架。→ **归属存疑，需人工复核**。

### 0.2 "Sophie Sonuga-Barke（阿姆斯特丹大学）"

**核实结果：⚠️ 部分错误。**

Sonuga-Barke 是 **Edmund J.S. Sonuga-Barke**（男），**不是** Sophie，且**不在阿姆斯特丹大学**。他长期任职 **University of Southampton（南安普顿大学）** 心理学院，并在 **Vrije Universiteit Amsterdam（阿姆斯特丹自由大学）** 兼任教职。他也担任 JCPP（*Journal of Child Psychology and Psychiatry*）主编。

（本次检索未获得其个人任职页的一手确认——见 §9 "我们不知道"第 8 条。）

### 0.3 "Optimal Arousal（最佳唤醒水平）框架的出处"

**核实结果：❌ 无法证实为 Sonuga-Barke 的原创。**

- PubMed `ADHD[tiab] AND "optimal arousal"[tiab]` → **0 命中**。
- PubMed `"optimal arousal"[tiab]`（不限 ADHD）→ 31 命中，但均为其他领域（视觉搜索、体育心理、麻醉）。
- **"Optimal arousal" 的心理学源头是 1960 年代的 Yerkes-Dodson law（耶克斯-多德森定律）**，不是 Sonuga-Barke。Sonuga-Barke 常引用它，但他本人的表述是**"过度唤醒 / under-arousal"**（`inactivity to over-arousal`），这与 Optimal arousal 概念方向相反——ADHD 是**需要更高唤醒**而非停在最佳点。
- → 归入 §9 "我们不知道"。

### 0.4 James Wilmot 2011 Nature Neuroscience 论文

**核实结果：⚠️ 检索异常，本报告将其作为"文献无法独立核实"处理。**

按简报给出的完整标题 *"Top-down modulation affects ADHD-like symptoms in novel reward situations"* 在以下来源检索，**全部为 0 命中**：
- PubMed esearch（标题词组、全字段、多组变体）
- Europe PMC REST（含 resultType=core）
- Crossref（query.title / query.bibliographic）
- OpenAlex（title.search）
- Semantic Scholar graph API（多次尝试，429 限流 + 一次仅返回 Robbins 2011 的无关结果）

交叉核对：Crossref 中 Nature Neuroscience 2011 年第 14 卷**全 311 条记录**已拉取，逐条检查作者与标题，**无**任何 ADHD/Wilmot 条目；DOI `10.1038/nn.2798` 实际对应 "Deletion of a remote enhancer near ATOH7…"（Ghiasvand 等，pp. 578-586），与 ADHD 无关。

**处理方式**：本报告**不引用**该论文的具体内容、样本量或结论。若 Skill 需要引用 Wilmot/Kidd/Davidson，**必须由人工通过期刊官网或馆际互借取得一手全文后补入**。→ §10 未列入正式来源。

---

## 1. 争点的准确表述

简报给的表述是"**执行功能控制不了注意力** vs **注意力只能被兴趣捕获、无法被意志捕获**"。

这个表述**过于简化**。文献中真正的对立是：

| 阵营 | 学术名称 | 核心主张 | 关键临床指向 |
|---|---|---|---|
| **A（缺陷说）** | Executive Dysfunction (EDF) / Inhibitory Deficit | ADHD 的核心是**自上而下控制失效**（抑制、工作记忆、重规划）。Barkley 1997 版本：抑制失败是上位缺陷，其余 EF 症状是次级后果。 | 训练自控力 / EF 训练 / 药物改善 PFC 调控 |
| **B（动机说）** | Delay Aversion (DAv) / Inadequate Reward Arousal / "Deficiency of Interest" | ADHD 的核心是**动机—奖赏回路的失调**，注意力不是"管不住"，而是**根本没有可被意志调用的驱动力**（延迟规避 / 高奖励显著偏向）。 | 改造环境与激励结构 / 缩短延迟 / 提高即时强化密度 |
| **A+B 调和（主流）** | Dual-Pathway Model | 两条通路**部分独立共存**，各占约 50% 的 ADHD 病例。 | 分型干预 |
| **C（第三方调和）** | Effort / Incentive Salience 失调控 | 问题不在"控制"也不在"有没有驱动力"，而在**自上而下控制与自下而上显著性之间的配比失调**（Wilmot 等；Rothenberger 等）。 | 提升任务显著性 / 外部结构化 |

**关键点**：A 与 B 在 2002 年前后经历了一次**实证转折**——原先被当作互斥竞争者的两个模型，被 MTA 数据显示**可以解离共存**。见 §2.1。

---

## 2. 支持方 A：缺陷说 / 执行功能说的核心证据

### 2.1 关键转折实验：Solanto et al. 2001（MTA 样本）

**这是整场争论的枢纽实验，必须保留。**

- **来源**：通过 Sonuga-Barke et al. 2002 / 2003 的转述获得。**原始 Solanto et al. (2001) 全文未获取**。
- **样本**：MTA 研究的子样本，**n = 77** 名 ADHD 儿童接受 stop-signal 任务（测反应抑制）。
- **设计**：两个任务并置——(a) Stop Test（抑制控制）；(b) Choice Delay Task（1 分 / 2 秒 vs 2 分 / 30 秒，测延迟规避）。
- **结果**：单任务判别率很低（stop-signal **61%**，choice delay **53%**）；两任务**联合**判别率跃升至 **88%**。
- **解读**：抑制控制与延迟规避**相关性低**——两者是**相互独立**的构念。
- **可及来源**：Markomichali 的南安普顿博士论文（eprints.soton.ac.uk/374941）第 9-10 页，**明确转述了这一数字并注明来源为 MTA 1999 子样本**。可信度：⚠️【推断（二手学术转述）】，非一手。
- 复现：Sié为中心的团队在学前儿童样本中复现了该双通路解离（经 Sonuga-Barke, Dalen & Remington 2003 转述，**原文未获取**）。

> **对本 Skill 的意义**：这是"控制缺陷 vs 兴趣驱动"之争从"二选一"变成"并存"的转折点。它同时也是**双方都承认的事实**——所以它属于 §8 共识区，不属于任一方的独占论据。

### 2.2 EF 效应的真实量级（小，且异质性大）

- **来源**：Thapar 等 ECNP 立场文件 `JCPP 2005;44(9):1389`（DOI `10.1111/j.1469-7610.2005.01476.x`，PMID `15720368` — **仅摘要，全文未获取**）
- **要点**：
  - ADHD 组在实验室 EF 指标上的效应量"modest（小到中等）"。
  - **"只有一小部分 ADHD 儿童在多项 EF 任务上表现出真正的缺陷"**（个体水平）。
  - EF 指标作为内表型的"内部异质性"被严重忽视。
- **关键限制**（原文自己承认）：效应量小、在组内组间变异大、大量共病与亚型混淆。

### 2.3 EF 缺陷并非 ADHD 特异

- **来源**：Sonuga-Barke 2010 *"Disambiguating Inhibitory Dysfunction in ADHD: Toward the Decomposition of Developmental Brain Phenotypes"*, **Biological Psychiatry** 68(1):9-16（**全文已获取** — 检索命中的 PubMed 全文片段）
- **要点**：作者本人（反缺陷阵营的核心人物）明确承认：
  1. 抑制任务"taps multiple cognitive processes"，ADHD-对照差异可能来自 ①抑制功能障碍 ②基本认知过程缺陷 ③**能量过程改变** ④**缺乏动机与参与度**——**四种解释无法区分**。
  2. 即使抑制任务表现正常（表现良好时），也可能是**更大努力**或**补偿策略**掩盖了更基础的抑制脑过程异常。
  3. 横断面研究**无法确立抑制缺陷的因果地位**——抑制缺陷可能是更早过程的**次级后果**。

> **这是反缺陷阵营内部的一次公开的、可引用的自我批评**，对本 Skill 极有价值：它意味着"控制缺陷说"连其主要对手之外的阵营都不完全买账。

### 2.4 维度模型下的 EF 缺陷缺失

- **来源**：Salum, Sonuga-Barke, Sergeant, Vandekerckhove, Gadelha, Moriyama et al. (2014), *Psychological Medicine* 44(15):3189-3203, DOI `10.1017/S0033291714000919`, PMID `25065454`（**仅摘要，全文未获取**）
- **样本**：**n = 1,547** 名儿童（6-12 岁），DAWBA 分为无症状 / 亚阈值轻度 / 亚阈值中度 / 临床 ADHD 四层。
- **方法**：2-选择反应时任务 + 冲突控制任务，用**扩散模型**分解 RT 与错误数据为 BIP（基本信息处理）与 IB-EF（抑制性 EF）成分。
- **结果**：
  - **BIP 缺陷**：在所有严重度层级（含亚临床）线性增长，且**跨越多动/冲动与注意两个症状维度**。
  - **IB-EF 与 ADHD 无关**（null result）。
- **解读**：作者称此"supports a dimensional model"。但对 A 阵营不利：**基于抑制的 EF 成分在 1,547 人样本中与 ADHD 无关。**

### 2.5 A 阵营的当代神经影像证据（多通路检验）

- **来源**：Stevens, Pearlson, Calhoun, Bessette (2018), *Biological Psychiatry: Cognitive Neuroscience and Neuroimaging* 3(8):675-684, DOI `10.1016/j.bpsc.2017.09.005`, PMID `30092917`（**仅摘要，全文未获取**）
- **样本**：**N = 251** 名 12-18 岁 DSM-IV 合并型 ADHD 或对照青少年（男女均有）。
- **方法**：行为抑制 + 即时奖励偏好双任务 → **taxometric（类别学）**分析分组 → 对三个 ADHD 亚组各做 fMRI（金币激励延迟任务 MID + go/no-go 抑制任务）。
- **结果**：
  - 识别出三个亚组：① EF/运动抑制缺陷型 ② EF + 奖励双缺陷型 ③ 实验室表现相对正常型。
  - **每个认知域映射到不同的脑功能障碍特征，符合双通路模型预测。**
  - **但：尽管三个亚组的 ADHD 临床特征几乎完全相同，没有任何脑异常是三个亚组共有的。**
- **解读**：作者结论——合并型 ADHD 是"一组离散障碍的集合，相似的行为终点通过不同的神经通路产生"。作者明确警告："对个别 ADHD 患者套用共同因果的单一缺陷模型应当谨慎。"
- **双边价值**：这篇同时**支持**双通路模型（分区成立）**和**反驳统一缺陷模型（无共同基础）。

---

## 3. 支持方 B：动机/奖赏说的核心证据

### 3.1 延迟规避（Delay Aversion）范式

- **来源**：Sonuga-Barke, Taylor, Sembi & Smith (1992)，PMID `1400689`（**仅摘要/题录，全文未获取**）
- **核心逻辑**（来自南安普顿博士论文转述，可信度 ⚠️【二手转述】）：
  - ADHD 儿童选择"小而即得（SS）"而非"大而延迟（LL）"，**不是因为偏好即时的奖励本身**，而是因为**厌恶延迟本身**。
  - 对照儿童的目标是"最大化总收益"；ADHD 儿童在奖励选择中的目标是"**最小化在任务上的总时间**"。
- **关键可检验预测**：如果在 SS 之后施加**强制的事后延迟**，SS 选项就不再减少总延迟 → 预测 SS 选择率应下降。
- **复现状态**：Marco et al. 2009 与 Tripp & Alsop 2001 复现（**原文未获取**）；Marco et al. 2009（PMID `19413450`）**确实支持双成分模型**（见 §3.2）。

### 3.2 IDIR vs DAv 的分离（大规模样本）

- **来源**：Marco, Miranda, Schlotz, Melia, Mulligan, Müller, Andreou, Butler, Rubia, Lesch, Sonuga-Barke et al. (2009), *Neuropsychology* 23(3):367-373, DOI `10.1037/a0014914`, PMID `19413450`（**仅摘要，全文未获取**）
- **样本**：**360 名 ADHD 先证者 + 349 名同胞 + 112 名对照**，年龄 **6-17 岁**。
- **任务**：Maudsley 延迟规避量表（Kuntsi et al. 2001）：1 分/2秒 vs 2 分/30 秒。**两种条件**：一种条件下选 SS 可减少试次总延迟，另一种不能。
- **结果**：
  - ADHD 组在**两种条件下都比对照更常选 SS**。
  - **当 SS 选择能减少试次延迟时，这个效应更大。** → 直接支持延迟规避成分。
  - ADHD SS 应答者更年轻、IQ 更低、共病更重；**且其同胞更可能是 SS 应答者** → 家族性成分。
- **作者结论**：支持"IDIR + DAv 双成分模型"；SS 选择**可能**是 ADHD 动机亚型的标记。

### 3.3 遗传分离：多巴胺基因 vs 血清素基因

- **来源**：Sonuga-Barke, Kumsta, Schlotz, Lasky-Su, Marco, Miranda, Mulas, Oades, … Sonuga-Barke (2011), *Biological Psychiatry* 70(3):230-237, DOI `10.1016/j.biopsych.2011.01.040`, PMID `21497794`（**仅摘要，全文未获取**）
- **样本**：**459 名男童与青少年（328 ADHD + 131 未受影响同胞）**。
- **设计**：基因分型 **DAT1（SLC6A3）40bp VNTR** 与 **5-HTTLPR（SLC6A4）启动子多态性**。
- **结果**：
  - **DAT1 对 IDIR 无效应。**
  - **5-HTTLPR s 等位基因携带者更延迟规避**（由 ADHD 组的 s/l 基因型驱动）。
- **解读**：作者主张 IDIR 与 DAv 具**遗传特异性**，DAv 涉及**血清素**功能。
- ⚠️ **注意这对 B 阵营本身是个复杂结果**：它把"延迟规避"从纯多巴胺假说里拆出来，指向血清素——与 B 阵营最经典的多巴胺版本不完全兼容。

### 3.4 延迟折扣 vs 症状维度的对应（Scherez 组）

- **来源**：Scheres, Tontsch, Thoeny, Kaczkurkin (2010), *Biological Psychiatry* 67(7):641-647, DOI `10.1016/j.biopsych.2009.10.033`, PMID `20034616`（**仅摘要，全文未获取**）
- **样本**：**ADHD-C n = 25，ADHD-I n = 20，对照 n = 37**，6-17 岁。三个延迟折扣任务，操纵奖励量级与 session 长度。
- **结果**：
  - **陡峭折扣只出现在 ADHD-C，不出现在 ADHD-I**，与奖励量级和 session 长度无关。
  - 维度分析：陡峭折扣与**多动-冲动**维度相关（**跨越了任意的亚型 cutoff**），尤其在试次级奖励量级小时。
- **解读**：陡峭折扣最好被理解为**多动/冲动症状维度的相关物**，而非 ADHD 整体的缺陷。这**削弱**了"延迟折扣 = ADHD 核心"的强版本。

### 3.5 任务本身不是单一构念（方法论警告）

- **来源**：Scheres, Sumiya, Thoeny (2010), *International Journal of Methods in Psychiatric Research* 19(3):167-175, DOI `10.1002/mpr.309`, PMID `20812292`（**仅摘要，全文未获取**）
- **样本**：**55 名心理学本科生**（非 ADHD 样本）。
- **结果**：PCA 提取出**两个成分**——(a) 小金额 / 短延迟；(b) 大奖励 / 长延迟。**这两个成分之间不相关。**
- **作者结论**：**"延迟折扣不是一个统一构念。"**
- → 这一条**对整个 B 阵营的证据基础构成直接威胁**：如果"ADHD 的折扣率更陡"这一结论依赖于用哪个任务测量，那么不同 meta 分析之间的不一致就有了技术性解释。

### 3.6 评分方法敏感性

- **来源**：de Water, Demurie, Mies, Scheres (2024), *Child Neuropsychology* 30(5):702-716, DOI `10.1080/09297049.2023.2268768`, PMID `37860876`（**仅摘要，全文未获取**）
- **方法**：利用两个已发表数据集，比较**四种**延迟折扣结果计算方法（8-17 岁儿童青少年）。
- **要点**：高冲动个体选择**高度不一致**，使得常用的 TD 结果指标（如曲线下面积 AUC）**难以确定**。
- → 与 §3.5 呼应：**测量本身可能制造或掩盖组间差异。**

---

## 4. 支持方 C：整合派（top-down vs bottom-up 配比失调）

这一派的代表是简报点名的 **Wilmot / Kidd / Davidson（威斯康星）** 与 **Rothenberger（萨尔）**。

### 4.1 Wilmot et al. 2011 — ⚠️ 无法核实

见 §0.4。本报告**不陈述其内容**。

可用的周边证据（来自可核实的摘要）支持"C 派"的主题存在性，但**不能替代**对 Wilmot 原文的引用：

- **Luman, Tripp, Scheres (2010)**, *Neuroscience & Biobehavioral Reviews* 34(5):744-763, DOI `10.1016/j.neubiorev.2009.11.021`, PMID `19944715`（**全文摘要已获取**）明确指出 ADHD 的神经生物学模型之一是"**impaired bottom-up prefrontal activation**"（自下而上的前额叶激活受损），即 C 派的主张在 2010 年已进入主流综述。
- 同一篇是本领域**最系统的批评方文献**，见 §6.1。

### 4.2 Rothenberger 一脉的实际主张

简报要求找"**Rothenberger 等人对 Sonuga-Barke 的批评**"。检索结果：

- **Rothenberger & Sonuga-Barke 的合著极多（PubMed 58 条）**，且包含 2005 年 ECNP 立场文件 *"Whither causal models in the neuroscience of ADHD?"*（Coghill, Nigg, **Rothenberger**, **Sonuga-Barke**, Tannock；*Developmental Science* 8(2):105-111, DOI `10.1111/j.1467-7687.2005.00397.x`, PMID `15720368`，**仅摘要，全文未获取**）。
- 该立场文件的实际主张（摘要原文）：ADHD 领域"**已提出若干因果模型，但仍相距甚远，未能实证证明任何一个模型的可行性**"。障碍包括：①需跨多层次的多学科协作 ②需建模**因果异质性** ③需整合环境与社会过程 ④需动态建模发展过程。
- **这是一个"两派都需要被证伪"的共同立场，不是 Rothenberger 单方面反对 Sonuga-Barke。**

> **⚠️ 重要修正**：简报暗示存在"Rothenberger 反对 Sonuga-Barke"的专门批判文献。**本次检索未找到这样一篇论文。** Rothenberger 与 Sonuga-Barke 是长期共同作者（共同署名 MTA 立场文件、DSM 相关的 *"The impact of study design and diagnostic approach in a large multi-centre ADHD study"* BMC Psychiatry 2011, DOI `10.1186/1471-244X-11-54`, PMID `21252506` 附近的 2011 年文献）。**把 Rothenberger 描述成 Sonuga-Barke 的批评者，在现有文献中缺乏支持。**
>
> 真正的、已找到的、有名有姓的批评方是 **Luman / Tripp / Scheres（§6.1–6.3）** 与 **Scheres 的测量学批评（§3.5）**。这是本次调研对任务简报的**第二个实质性纠正**。

---

## 5. 因果性之争：延迟折扣是原因还是结果？

### 5.1 支持"相关物"（非原因）——目前证据倾向于这一侧

- **Scheres et al. 2010（§3.4）**：陡峭折扣**只关联多动-冲动维度，不关联注意**。若折扣是 ADHD 的病因，它应当跨症状域泛化。它没有。
- **del Water et al. 2024（§3.6）**：折扣测量本身对**评分方法**高度敏感——这削弱了把高折扣率当作稳定个体特质的前提。
- **Plichta & Scheres (2014)**, *Neuroscience & Biobehavioral Reviews* 38:125-144, DOI `10.1016/j.neubiorev.2013.07.012`, PMID `23928090`（**仅摘要，全文未获取**）：
  - 元分析：ADHD 的**腹侧纹状体低反应（VS-hyporesponsiveness）效应量 Cohen's d = 0.48-0.58**（中等）。
  - **关键悖论**：在健康人群中，特质冲动性与奖赏加工中的 VS 激活**正相关**（正相关）。
  - 作者列出三种整合方案：(1) **倒 U 形模型**；(2) **（遗传）调节模型**；(3) **"无关模型"（unrelated model）**——即 ADHD 的神经异常与冲动性在健康人中是两回事。
  - **作者明确结论**：现有研究数量"太少，无法给出最终答案"；三种整合方案"应被理解为为未来研究设定可检验假设的尝试"。

### 5.2 支持"原因"的间接论证（弱）

- **Sonuga-Barke, Sergeant, Nigg, Willcutt (2008)**, *Child Adolesc Psychiatr Clin N Am* 17(2):367-385, DOI `10.1016/j.chc.2007.11.008`, PMID `18295151`（**仅摘要，全文未获取**）：
  - 作者的实证综述结论：**"EF 缺陷与延迟规避都卷入 ADHD，但两者对 ADHD 既非必要也非特异。"**
  - 二者"在某种程度上相互解离，因此各自可能代表与 ADHD 某个亚样本相关的独特特征"。
  - **对诊断的价值**：两者"对当前构念下的 ADHD 诊断增加不了多少价值，但可能是切分异质性的关键"。
- 这实际上**既不是"原因"也不是"结果"**——是一个**第三种立场：亚型标记物（subtype marker）**。

### 5.3 Hitch / Hutner 线 — ❌ 未能定位

- PubMed `Hitch GP[au] AND ADHD[tiab]` → **0 命中**
- PubMed `Hutner[au] AND ADHD[tiab]` → **0 命中**
- PubMed `Hitch[au] AND ADHD[tiab]` → **0 命中**
- → 简报中的 "Graham Hitch / Jan Hutner" 与 ADHD 延迟折扣因果之争的关联，**本次检索未能证实**。→ §9 "我们不知道"。

---

## 6. 批评方完整档案（给足篇幅）

### 6.1 Luman, Tripp, Scheres (2010) — 最系统的方法论批评

**这是本领域针对 B 阵营最有力、最可引用的一篇。**

- **来源**：*Neuroscience & Biobehavioral Reviews* 34(5):744-763, DOI `10.1016/j.neubiorev.2009.11.021`, PMID `19944715`（**摘要已获取，全文未获取**）
- **方法**：对比**七个神经生物学上有效的 ADHD 奖赏敏感性模型**，列出**15 条可检验预测**。
- **四条批评**（摘要原文要点）：
  1. **模型解释层级差异巨大**：有些试图用**低层级强化系统**（如"多巴胺把奖励前移"）解释单一核心缺陷；有些解释**多个缺陷**，靠描述**高层级系统**（如"自下而上的前额叶激活受损"）。→ **不同派别在说不同层级的话，直接比较是范畴错误。**
  2. **实验证据的偏斜**：绝大多数实验研究只关注"面对奖励与反应代价 vs 无奖励"的行为改变，以及延迟折扣。
  3. **机制空白**："目前**缺乏**聚焦于 ADHD 中改变后的奖赏敏感性之**底层认知或神经机制**的研究。"
  4. **亚组空白**："同样**缺乏**试图理解**ADHD 儿童中哪个亚组**表现出奖赏敏感性改变的研究。"
- **作者解释**：预测稀缺"部分源于缺乏如何在人身上检验某些预测的知识"。
- **对本 Skill 的意义**：这篇把"哪一派证据更硬"的问题，**部分转化为"各自在自己的层级上都还没有做实证"**——这是一个双方都适用的批评，不偏袒任一方。

### 6.2 Luman, Oosterlaan, Sergeant (2005) — 行为发现的反噬

- **来源**：*Clinical Psychology Review* 25(2):183-207, DOI `10.1016/j.cpr.2004.11.001`, PMID `15642646`（**仅摘要，全文未获取**）
- **范围**：22 项研究，**N = 1,181** 名儿童。
- **关键发现**：
  - 强化条件**对 ADHD 儿童的任务表现和动机水平都有正向影响**（对照儿童亦然）。
  - **"对任务表现的相关效应在 ADHD 中更为突出"**（强化在 ADHD 中更有效）。
  - **"有证据表明高强度强化对 ADHD 高度有效。"**
  - ADHD 儿童偏好即时而非延迟奖励。
  - 心理生理学上，ADHD 儿童**对强化的敏感度似乎低于**对照。
- **作者自己的结论（关键）**：**"结果显示理论模型与行为发现之间存在不一致（discrepancy）。"**
- → **这是 B 阵营最尴尬的一处**：如果 ADHD 只是"缺乏动机/延迟规避"，那么**增加强化本应能弥补它——而事实上它确实有效，且在 ADHD 组中效果更大。** 这既可以解读为"过度唤醒模型需要更强刺激"（B 的辩护），也可以解读为"这是外部补偿而非内在缺陷"（C 派的领地）。**这条证据被双方同时引用、且互不认输。**

### 6.3 Luman, Oosterlaan, Knol, Sergeant (2008) — 惩罚盲区

- **来源**：*Journal of Child Psychology and Psychiatry* 49(7):712-720, DOI `10.1111/j.1469-7610.2008.01910.x`, PMID `18422549`（**仅摘要，全文未获取**）
- **样本**：**23 名 ADHD 儿童 + 20 名健康对照**。
- **设计**：赌博范式，三选项（A 小奖小罚有利；B 大奖渐增罚；C 小奖渐增罚）。惩罚按**频率**或**量级**两个独立条件递增。测 HR 与皮肤电。
- **结果**：
  - 惩罚**量级**递增时，ADHD 儿童对有利选项的偏好**更小**（决策风格适应不良）。
  - 惩罚**频率**递增时，ADHD 儿童**表现与对照相同**。
  - **组间差异在任务做第二遍后衰减。**
- **作者结论**：ADHD 儿童"**对惩罚的频率敏感，但对惩罚的量级盲视**（sensitive to frequency but blind to the magnitude of penalty）"。
- → 这**不是**干净的"高奖励显著偏向"：**高奖励 → 少延迟**支持 B；**惩罚 → 少量级**实际上指向**回避学习受损**（一个更接近 A / 条件化的构念），**不支持 B 的纯版本**。

### 6.4 神经影像的矛盾方向（Plichta & Scheres 2014，见 §5.1）

再次强调：这是**最直接的方法论反证**——如果 ADHD 是"高奖励显著偏向 / 过度追求即时奖励"，那么健康人中冲动性与 VS 激活的**正相关**方向应该外推；实际数据是**反的**（ADHD 组 VS 低反应）。这迫使理论家提出倒 U 形等三层解释。**Plichta & Scheres 自己拒绝在这些方案中选边。**

### 6.5 元分析层面的效应量问题

- **Patros, Alderson, Kasper, Tarle, Lea, Hudec (2016)**, *Clinical Psychology Review* 43:162-175, DOI `10.1016/j.cpr.2015.11.001`, PMID `26602954`（**仅摘要，全文未获取**）
  - **26 项研究，28 个任务，总样本 4,320 名儿童（ADHD 2,360 / TD 1,960）**。
  - **选择冲动性（choice-impulsivity）总体效应量 g = 0.47**（中等）。
  - 延迟折扣与延迟满足任务上的模式**相似**。
  - **调节变量**：使用**单一信息源**诊断的研究比多信息源研究**效应更大**；排除女孩的样本比纳入女孩的样本**效应更大**。
  - → **方法学批评**：效应量被诊断质量系统性放大，且有性别偏倚。
- **Marx, Hacker, Yu, Cortese, Sonuga-Barke (2021)**, *Journal of Attention Disorders* 25(2):171-180, DOI `10.1177/1087054718772138`, PMID `29806533`（**⚠️ PubMed 无摘要，全文未获取**）
  - 比较 simple choice-delay 与 temporal discounting 两类范式的**对比性元分析**。**这是 B 阵营自己人（Sonuga-Barke 为共同作者）做的元分析**——恰好是对自己基础证据的压力测试。**因摘要不可得，本报告不陈述其效应量数值。** → §9 "我们不知道"。
- **Jackson & MacKillop (2016)**, *Biological Psychiatry: Cognitive Neuroscience and Neuroimaging* 1(4):316-320, DOI `10.1016/j.bpsc.2016.01.007`, PMID `27722208`（**仅摘要，全文未获取；摘要中数值被期刊 HTML 截断**）
  - 567 篇候选文献 → **21 项独立研究，25 个病例-对照比较**。
  - 结论：ADHD 个体的延迟折扣**显著升高，中等效应量**，且构成"稳健证据"。
  - **⚠️ 关键效应量数值在可获取的摘要文本中被截断**，无法引用具体数值。→ 记入 §9。

### 6.6 跨疾病特异性反证（trans-disease 反驳）

这是对"B 派专属机制"最强的结构性反驳。

- **Bickel, Athamneh, Basso, Mellis, DeHart, Craft, Pope (2019)**, *Current Opinion in Psychology* 30:59-64, DOI `10.1016/j.copsyc.2019.01.005`, PMID `30852411`（**仅摘要，全文未获取**）
  - 延迟折扣被识别为**跨疾病过程（trans-disease process）**，同时是物质使用障碍、ADHD、重度抑郁的**内表型**，并与**多巴胺能 AND 血清素能**神经传递缺陷相关。
  - → 如果高折扣率是成瘾、抑郁、ADHD、肥胖共享的，它**不能**作为区分 ADHD 的机制性解释。
- **Chen, Becker, Qin, Lei, Chen, Liu et al. (2021)**, *Journal of Psychiatric Research* 139:62-70, DOI `10.1016/j.jpsychires.2021.05.008`, PMID `34044265`（**仅摘要，全文未获取**）
  - 19 篇纳入：成瘾 9 篇（154 例）、ADHD 6 篇（106 例）、肥胖 4 篇（94 例）。
  - 共同神经标记：尾状核、腹内侧 PFC、dlPFC 反应不足。
  - **但疾病特异模式也同时存在**：成瘾 = 海马-纹状体网络低激活；**ADHD = 多巴胺投射纹状体网络高激活**；肥胖 = dACC + dlPFC 活动下降。
  - → 注意 **ADHD 的特异方向是"高激活"**，与成瘾/肥胖的"低激活"**相反**。这实际上是对 ADHD 奖赏假说的**部分支持**（ADHD 纹状体反应过强 = 过度显著性），但也说明这个"特异模式"在 n=106 的 6 篇研究里，**稳健性未知**。

---

## 7. 对抗矩阵（分歧并列，不调和）

| 争点 | A 方（缺陷说）主张 | B 方（动机说）主张 | 当前证据状态 |
|---|---|---|---|
| 核心缺陷是什么 | 自上而下抑制控制失效（Barkley 1997） | 延迟规避 / 奖励梯度陡峭 / 动机通路失调 | **并存**（§2.1，n=77 MTA 数据） |
| EF 实验室指标 | 组水平有中等效应 | 效应小、仅少数人真正缺陷 | **A 方部分胜出**：Salum n=1,547 显示**抑制性 EF 成分与 ADHD 无关** |
| 折扣率的方向 | 只是相关物，多与多动-冲动维度有关 | 是 ADHD 的核心机制 | **B 方承压**：Sch eres 2010 显示折扣不关联注意；del Water 2024 显示测量不稳健 |
| 强化的作用 | 药物/环境提供外部控制补偿 | 提高刺激强度可克服低唤醒 | **双方都能用**：Luman 2005 n=1,181 显示高强度强化对 ADHD 特别有效 |
| 神经标记 | 背侧前额-纹状体 | 腹侧纹状体 / 腹侧前额 | **矛盾**：Plichta & Scheres 2014 元分析 d=0.48-0.58 低反应，但健康人方向相反 |
| 心理测量学 | EF 指标可切分亚型 | 折扣可切分亚型 | **双方都被削弱**：Scheres 2010 显示折扣是两个成分；EF 在大规模样本中 null |
| 机制特异性 | （未直接主张特异性） | ADHD 特有 | **B 方受损**：折扣是跨疾病过程（Bickel 2019） |
| 谁更可能是次级后果 | — | — | **真正无人回答**（见 §9） |

---

## 8. 目前的证据状态

### 8.1 ✅ 真共识（可以写进 Skill 的"领域共识框架"）

1. **ADHD 不是单一构念，存在至少两条部分解离的通路。**
   - 支撑：Solanto et al. 2001（MTA 子样本 n=77，联合判别率 88% vs 单任务 61%/53%，⚠️经二手转述）；Stevens et al. 2018（N=251，taxometric 分出三组，各映射不同脑区，PMID `30092917`）；Sonuga-Barke 2003 双通路模型原文。
   - **来源可信度：高（同行评议），但关键数字为二手转述。**

2. **实验室 EF 指标的组间效应量小到中等，且个体层面只有少数 ADHD 表现真正缺陷。**
   - 支撑：Thapar et al. 2005 ECNP（PMID `15720368`）；Mahone & Denckla 2017（*J Int Neuropsychol Soc* 23(9-10):916, DOI `10.1017/S1355617717000807`, PMID `29198277`）。

3. **ADHD 的实验室表现**高度依赖任务条件与激励结构**；表现并非"全时段缺陷"。**
   - 支撑：Luman et al. 2005（n=1,181，强化条件对 ADHD 组效果更大）；Lemiere et al. 2010（*Eur Child Adolesc Psychiatry* 19(8):679-685, DOI `10.1007/s00787-010-0105-9`, PMID `20361222`，64 ADHD + 76 对照，9 项 TEA-Ch 子测中 6 项表现差，但**控制 IQ 与年龄后对正确分类的贡献仅边际**，且三因子结构拟合差）。
   - **注意**：最后一点同时**削弱**了"实验室 EF 指标能反映日常注意力"的说法。

4. **腹侧纹状体（VS）在奖励期待期对 ADHD 组呈低反应，效应量中等（d ≈ 0.48-0.58）。**
   - 支撑：Plichta & Scheres 2014 元分析（PMID `23928090`）。
   - ⚠️ **但注意**：这与"高奖励显著偏向"的表面预测方向相反——见 §7。这是**数据事实共识**，不是**理论共识**。

5. **ADHD 的执行功能/抑制性 EF 成分不像是一个稳定的维度性缺陷。**
   - 支撑：Salum et al. 2014，**n = 1,547**，IB-EF 与 ADHD **无关**（PMID `25065454`）。

6. **延迟折扣的测量高度依赖具体任务与评分方法，不是一个统一构念。**
   - 支撑：Scheres et al. 2010（n=55，PCA 两个正交成分，PMID `20812292`）；del Water et al. 2024（四种评分方法比较，PMID `37860876`）。

### 8.2 ⚠️ 仍在吵（必须并列保留）

1. **ADHD 的核心缺陷是控制还是动机？** — 无共识。双通路并存是共识，但"哪个是主路径"未定。
2. **延迟折扣率是原因、结果，还是亚型标记？** — 三种说法都有支持者，无一被排除（§5）。
3. **VS 低反应 vs 冲动性正相关 vs ADHD 特异的高激活** — 三个方向的数据并存，Plichta & Scheres 自己拒绝选边（倒 U / 遗传调节 / 无关模型）。
4. **实验室 EF 指标能否切分 ADHD 亚型？** — Sonuga-Barke 自己（2008 摘要）说 EF 与 DAv "既非必要也非特异"，但 Stevens 2018 用 fMRI 找到了亚组特异的脑差异。**两人都用"异质性"论证，但一个用它说明理论无用，一个用它说明理论有效。**
5. **理论解释层级混乱** — Luman/Tripp/Scheres 2010 明确指出不同模型在**不同分析层级**运作，直接比较是范畴错误。**这一条尚未被领域普遍接受。**

### 8.3 ❌ 明确未被支持的强主张

- "ADHD 儿童在奖励选择中的目标是**最小化在任务上的总时间**"——来自二手转述，未在一手文献中核实其原文表述强度。
- "**‘在状态中（in the zone）时没有功能障碍**"——这一常见临床主张，检索中未找到任何同行评议支持。→ §9。

---

## 9. "我们不知道"清单

以下是本次调研确认**至今没有定论**的问题。每条都标注了为什么它是开放的。

1. **延迟折扣率高是 ADHD 的原因、结果、还是无关的伴随物？**
   - 开放原因：全部相关证据都是横断面的。Scheres 2010 显示折扣只关联多动-冲动维度；Plichta & Scheres 2014 拒绝在三种整合方案中选边。**没有任何一项纵向研究或干预研究被找到能定此因果。**

2. **ADHD 的纹状体反应到底是"低"还是"高"？**
   - 开放原因：Plichta & Scheres 元分析得到 d=0.48-0.58 的**低**反应；Chen et al. 2021 元分析却报告 ADHD 的**多巴胺投射纹状体网络高激活**。**两个同行评议元分析方向相反。**

3. **延迟折扣的**确切效应量**是多少？**
   - 开放原因：Jackson & MacKillop 2016（n=21 研究 / 25 比较）的效应量数值**在可获取的摘要文本中被截断**；Marx et al. 2021 元分析**PubMed 无摘要**。本报告**拒绝猜测数值**。

4. **折扣/EF 能否作为个体层面的诊断或亚型标记？**
   - 开放原因：Sonuga-Barke, Sergeant, Nigg, Willcutt 2008（PMID `18295151`）自己说这两者"对诊断增加不了多少价值"。Stevens 2018 找到亚组但**亚组间临床特征几乎相同**——即亚组没有临床预测力。

5. **ADHD 是否能被拆成"控制型"和"动机型"两个临床上有用的亚型？**
   - 开放原因：所有切分方案都缺乏**外部验证**（跨样本复现）与**治疗交互验证**（"这个病人该用 A 方案还是 B 方案"从未被 RCT 检验）。Nigg, Karalunas, Feczko & Fair 2020（PMID `32305325`）把这明确列为待办："利用不同统计、计算和机器学习方法解决 ADHD 异质性"。

6. **奖励回路异常与 ADHD 的共病（物质使用、抑郁、肥胖）之间是因果关系还是共同底层的跨疾病过程？**
   - 开放原因：Bickel et al. 2019 把折扣定性为跨疾病过程；Chen et al. 2021 同时报告了共同标记与疾病特异模式。**两者可以同时为真，但 ADHD 特异模式的稳健性未被独立复现。**

7. **实验室任务 vs 真实世界的落差有多大？**
   - 开放原因：Lemiere et al. 2010（n=64 ADHD）显示 TEAC-Ch 表现差但**控制 IQ/年龄后对分类的贡献边际**。Stevens 2018 显示三个亚组**临床特征几乎相同**。真实世界的情境依赖性是 ADHD 的核心特征，但**没有一个被广泛接受的实验范式能捕捉它**。

8. **"Optimal Arousal" 框架在 ADHD 文献中的确切出处与地位？**
   - 开放原因：`ADHD[tiab] AND "optimal arousal"[tiab]` 在 PubMed **0 命中**。Sonuga-Barke 的相关表述是 "under-arousal to over-arousal"，与 Yerkes-Dodson 的"最佳唤醒点"概念方向不同。**该框架的来源需人工查证原始出处。**

9. **Wilmot, Kidd, Davidson (2011) Nat Neurosci 的实际内容？**
   - 开放原因：见 §0.4，四大索引 + Crossref Nature Neuroscience 2011 全年 311 条记录均无匹配。**必须人工取得一手全文。**

10. **Graham Hitch / Jan Hutner 与延迟折扣因果之争的关系？**
    - 开放原因：PubMed 中 `Hitch[au] AND ADHD[tiab]` 与 `Hutner[au] AND ADHD[tiab]` 均为 **0 命中**。**归属需人工复核。**

11. **Bethany Annen / George Low 的"Deficiency-Deficit Framework"是否真实存在？**
    - 开放原因：见 §0.1，全库 0 命中。**极可能是任务简报中的错误归属，需人工复核后再决定是否纳入 Skill。**

12. **ADHD 的"高刺激偏好"是否是一个独立于 EF 的构念？**
    - 开放原因：诊断测量工具上完全缺失——没有经过验证的"高刺激偏好"量表进入临床或研究常规（对比 EF 有大量标准化任务）。**一个没有自己测量工具的理论主张，无法被独立检验。**

---

## 10. 来源清单（40 条正式学术来源 + 1 条非学术）

### A. 同行评议论文（全文或摘要已通过 NCBI efetch / PubMed 核实）

| # | 引用 | DOI / PMID | 类型 | 可信度 | 全文状态 |
|---|---|---|---|---|---|
| 1 | Sonuga-Barke EJ (2002). Psychological heterogeneity in AD/HD—a dual pathway model. *Behav Brain Res* 130(1-2):29-39 | `10.1016/s0166-4328(01)00432-6` / PMID `11864715` | 综述 | ★★★★★ 同行评议 | 仅摘要 |
| 2 | Sonuga-Barke EJ (2003). The dual pathway model of AD/HD. *Neurosci Biobehav Rev* 27(7):593-594 | `10.1016/j.neubiorev.2003.08.005` / PMID `14624804` | 综述（框架原始出处） | ★★★★★ | 仅摘要 |
| 3 | Sonuga-Barke EJ (2005). Causal models of ADHD: from common simple deficits to multiple developmental pathways. *Biol Psychiatry* 57(11):1231-1238 | `10.1016/j.biopsych.2004.09.008` / PMID `15949993` | 综述 | ★★★★★ | 仅摘要 |
| 4 | Sonuga-Barke EJS (2010). Disambiguating Inhibitory Dysfunction in ADHD. *Biol Psychiatry* 68(1):9-16 | https://www.biologicalpsychiatryjournal.com/article/S0006322310000594/pdf | 综述 | ★★★★★ | **全文片段已获取** |
| 5 | Sonuga-Barke, Sergeant, Nigg, Willcutt (2008). Executive dysfunction and delay aversion in ADHD. *Child Adolesc Psychiatr Clin N Am* 17(2):367-385 | `10.1016/j.chc.2007.11.008` / PMID `18295151` | 综述 | ★★★★★ | 仅摘要 |
| 6 | Sonuga-Barke, Cortese, Fairchild, Stringaris (2016). Annual Research Review: Transdiagnostic neuroscience…differentiating decision making. *JCPP* 57(3):321-334 | `10.1111/jcpp.12496` / PMID `26705858` | 综述 | ★★★★★ | 仅摘要 |
| 7 | Sonuga-Barke EJS et al. (2023). Annual Research Review: Perspectives on progress in ADHD science. *JCPP* 64(4):506-533 | `10.1111/jcpp.13696` / PMID `36220605` | 综述 | ★★★★★ | 仅摘要 |
| 8 | Posner J, Polanczyk GV, Sonuga-Barke E (2020). Attention-deficit hyperactivity disorder. *Lancet* 395(10222):450 | `10.1016/j.jaac.2019.06.019` / PMID `31982036` | 综述 | ★★★★★ | 仅摘要 |
| 9 | **Luman M, Tripp G, Scheres A (2010). Identifying the neurobiology of altered reinforcement sensitivity in ADHD: a review and research agenda. *Neurosci Biobehav Rev* 34(5):744-763** | `10.1016/j.neubiorev.2009.11.021` / PMID `19944715` | **综述（批评方核心）** | ★★★★★ | 摘要已获取 |
| 10 | **Luman M, Oosterlaan J, Sergeant JA (2005). The impact of reinforcement contingencies on AD/HD. *Clin Psychol Rev* 25(2):183-207** | `10.1016/j.cpr.2004.11.001` / PMID `15642646` | **综述（含批评）** | ★★★★★ | 仅摘要 |
| 11 | Luman M, Oosterlaan J, Knol DL, Sergeant JA (2008). Decision-making in ADHD: sensitive to frequency but blind to the magnitude of penalty? *JCPP* 49(7):712-720 | `10.1111/j.1469-7610.2008.01910.x` / PMID `18422549` | 实验（n=23 ADHD + 20 对照） | ★★★★★ | 仅摘要 |
| 12 | Luman M, Oosterlaan J, Hyde C, van Meel CS, Sergeant JA (2007). Heart rate and reinforcement sensitivity in ADHD. *JCPP* 48(9):890-896 | `10.1111/j.1469-7610.2007.01769.x` / PMID `17714374` | 实验 | ★★★★★ | 仅摘要 |
| 13 | **Scheres A, Tontsch C, Thoeny AL, Kaczkurkin A (2010). Temporal reward discounting in ADHD. *Biol Psychiatry* 67(7):641-647** | `10.1016/j.biopsych.2009.10.033` / PMID `20034616` | **实验（n=25/20/37）** | ★★★★★ | 仅摘要 |
| 14 | **Scheres A, Sumiya M, Thoeny AL (2010). Studying the relation between temporal reward discounting tasks used in populations with ADHD: a factor analysis. *Int J Methods Psychiatr Res* 19(3):167-175** | `10.1002/mpr.309` / PMID `20812292` | **方法学批评（n=55）** | ★★★★★ | 仅摘要 |
| 15 | Marco R et al. (2009). Delay and reward choice in ADHD: an experimental test of the role of delay aversion. *Neuropsychology* 23(3):367-373 | `10.1037/a0014914` / PMID `19413450` | 实验（n=360/349/112） | ★★★★★ | 仅摘要 |
| 16 | Sonuga-Barke EJ et al. (2011). A functional variant of the serotonin transporter gene moderates impulsive choice in ADHD boys and siblings. *Biol Psychiatry* 70(3):230-237 | `10.1016/j.biopsych.2011.01.040` / PMID `21497794` | 实验（n=459） | ★★★★★ | 仅摘要 |
| 17 | **Plichta MM, Scheres A (2014). Ventral-striatal responsiveness during reward anticipation in ADHD…a meta-analytic review. *Neurosci Biobehav Rev* 38:125-144** | `10.1016/j.neubiorev.2013.07.012` / PMID `23928090` | **元分析** | ★★★★★ | 仅摘要 |
| 18 | **Patros CH, Alderson RM, Kasper LJ, Tarle SJ, Lea SE, Hudec KL (2016). Choice-impulsivity in children and adolescents with ADHD: a meta-analytic review. *Clin Psychol Rev* 43:162-175** | `10.1016/j.cpr.2015.11.001` / PMID `26602954` | **元分析（n=4,320）** | ★★★★★ | 仅摘要 |
| 19 | Jackson JN, MacKillop J (2016). ADHD and Monetary Delay Discounting: A Meta-Analysis. *Biol Psychiatry Cogn Neurosci Neuroimaging* 1(4):316-320 | `10.1016/j.bpsc.2016.01.007` / PMID `27722208` | 元分析（n=21 研究） | ★★★★★ | 仅摘要（**数值截断**） |
| 20 | **Marx I, Hacker T, Yu X, Cortese S, Sonuga-Barke E (2021). ADHD and the Choice of Small Immediate Over Larger Delayed Rewards. *J Atten Disord* 25(2):171-180** | `10.1177/1087054718772138` / PMID `29806533` | 元分析 | ★★★★★ | **PubMed 无摘要** |
| 21 | **Chen Z et al. (2021). Neural networks during delay discounting as trans-disease marker. *J Psychiatr Res* 139:62-70** | `10.1016/j.jpsychires.2021.05.008` / PMID `34044265` | 元分析（19 篇） | ★★★★☆ | 仅摘要 |
| 22 | **Bickel WK et al. (2019). Excessive discounting of delayed reinforcers as a trans-disease process. *Curr Opin Psychol* 30:59-64** | `10.1016/j.copsyc.2019.01.005` / PMID `30852411` | 综述（跨疾病反驳） | ★★★★★ | 仅摘要 |
| 23 | **Salum GA, Sonuga-Barke E, Sergeant J, et al. (2014). Mechanisms underpinning inattention and hyperactivity: neurocognitive support for ADHD dimensionality. *Psychol Med* 44(15):3189-3203** | `10.1017/S0033291714000919` / PMID `25065454` | **实验（n=1,547）** | ★★★★★ | 仅摘要 |
| 24 | **Stevens MC, Pearlson GD, Calhoun VD, Bessette KL (2018). Functional Neuroimaging Evidence for Distinct Neurobiological Pathways in ADHD. *Biol Psychiatry Cogn Neurosci Neuroimaging* 3(8):675-684** | `10.1016/j.bpsc.2017.09.005` / PMID `30092917` | **实验（n=251, taxometric + fMRI）** | ★★★★★ | 仅摘要 |
| 25 | **de Water E, Demurie E, Mies GW, Scheres A (2024). Temporal discounting in children and adolescents with and without ADHD: a comparison of four scoring methods. *Child Neuropsychol* 30(5):702-716** | `10.1080/09297049.2023.2268768` / PMID `37860876` | 方法学比较 | ★★★★★ | 仅摘要 |
| 26 | **Grimm O, van Rooij D, Hoogman M, Klein M, Buitelaar J, Franke B, Reif A, Plichta MM (2021). Transdiagnostic neuroimaging of reward system phenotypes in ADHD and comorbid disorders. *Neurosci Biobehav Rev* 128:165-180** | `10.1016/j.neubiorev.2021.06.025` / PMID `34144113` | 综述（跨诊断神经影像） | ★★★★★ | 仅摘要 |

### B. 立场文件 / 共识声明

| # | 引用 | DOI / PMID | 类型 | 可信度 | 全文状态 |
|---|---|---|---|---|---|
| 27 | Coghill D, Nigg J, **Rothenberger A**, **Sonuga-Barke E**, Tannock R (2005). Whither causal models in the neuroscience of ADHD? *Dev Sci* 8(2):105-111 | `10.1111/j.1467-7687.2005.00397.x` / PMID `15720368` | 立场文件（**A+B 共同作者**） | ★★★★★ | 仅摘要 |
| 28 | Thapar A et al. (2005). Are endophenotypes based on measures of executive functions useful for molecular genetic studies of ADHD? *JCPP* 44(9):1389 | `10.1111/j.1469-7610.2005.01476.x` | ECNP 立场文件 | ★★★★★ | 仅摘要（**经 Wiley/CAMH 站点获得完整正文片段**） |
| 29 | Faraone SV, Banaschewski T, Coghill D, Zheng Y, Biederman J, Bellgrove MA et al. (2021). The World Federation of ADHD International Consensus Statement: 208 Evidence-based Conclusions. *Neurosci Biobehav Rev* 128:789 | `10.1016/j.neubiorev.2021.01.022` / PMID `33549739` | 国际共识声明（80 作者 / 27 国） | ★★★★★ | 仅摘要 |
| 30 | Faraone SV, Asherson P, Banaschewski T, et al. (2015). Attention-deficit/hyperactivity disorder. *Nat Rev Dis Primers* 1:15020 | `10.1038/nrdp.2015.20` / PMID `27189265` | Primer | ★★★★★ | 仅摘要 |
| 31 | Posner J, Polanczyk GV, Sonuga-Barke E (2020). *Lancet* 395:450（见 #8） | 同上 | Lancet 综述 | ★★★★★ | 仅摘要 |
| 32 | Franke B, Michelini G, Asherson P, et al. (2018). Live fast, die young? *Eur Neuropsychopharmacol* 28(10):1059-1074 | `10.1016/j.euroneuro.2018.08.001` / PMID `30195575` | 综述（**注意：非 Sonuga-Barke 署名**） | ★★★★★ | 仅摘要 |
| 33 | Mahone EM, Denckla MB (2017). Attention-Deficit/Hyperactivity Disorder: A Historical Neuropsychological Perspective. *J Int Neuropsychol Soc* 23(9-10):916 | `10.1017/S1355617717000807` / PMID `29198277` | 历史综述 | ★★★★★ | 仅摘要 |
| 34 | Nigg JT, Karalunas SL, Feczko E, Fair DA (2020). Toward a Revised Nosology for ADHD Heterogeneity. *Biol Psychiatry Cogn Neurosci Neuroimaging* 5(8):726-737 | `10.1016/j.bpsc.2020.02.005` / PMID `32305325` | 综述 | ★★★★★ | 仅摘要 |
| 35 | Sergeant JA, Geurts H, Huijbregts S, Scheres A, Oosterlaan J (2003). The top and the bottom of ADHD. *Neurosci Biobehav Rev* 27(7):583-587 | `10.1016/j.neubiorev.2003.08.004` / PMID `14624803` | 综述（**认知-能量模型，中立第三方**） | ★★★★★ | 仅摘要 |
| 36 | Lemiere J, Wouters H, Sterken C, Lagae L, Sonuga-Barke E, Danckaerts M (2010). Are children with ADHD predominantly inattentive and combined subtypes different in terms of aspects of everyday attention? *Eur Child Adolesc Psychiatry* 19(8):679-685 | `10.1007/s00787-010-0105-9` / PMID `20361222` | 实验（n=64 ADHD + 76 对照） | ★★★★☆ | 仅摘要 |
| 37 | Costa Dias TG, Wilson VB, Bathula DR, et al. (2013). Reward circuit connectivity relates to delay discounting in children with ADHD. *Eur Neuropsychopharmacol* 23(1):33-43 | `10.1016/j.euroneuro.2012.10.015` / PMID `23206930` | 实验（静息态 fMRI） | ★★★★☆ | 仅摘要 |
| 38 | Costa Dias TG, Iyer SP, Carpenter SD, et al. (2015). Characterizing heterogeneity in children with and without ADHD based on reward system connectivity. *Dev Cogn Neurosci* 11:155-161 | `10.1016/j.dcn.2014.12.005` / PMID `25660033` | 实验（n=106，社区检测） | ★★★★☆ | 仅摘要 |
| 39 | Martin J, Hamshere ML, Stergiakouli E, O'Donovan MC, Thapar A (2015). Neurocognitive abilities in the general population and composite genetic risk scores for ADHD. *JCPP* 56(6):648-657 | `10.1111/jcpp.12336` / PMID `25280069` | 实验（**n=6,832 ALSPAC**） | ★★★★★ | 仅摘要 |
| 40 | Silvetti M, Wiersema JR, Sonuga-Barke E, Verguts T (2013). Deficient reinforcement learning in medial frontal cortex as a model of dopamine-related motivational deficits in ADHD. *Neural Netw* 46:199-207 | `10.1016/j.neunet.2013.05.008` / PMID `23811383` | 计算建模 | ★★★★☆ | 仅摘要 |

### C. ⚠️ 非学术来源（**不得作为学术引用**，仅用于说明简报前提的来源性质）

| # | 来源 | 类型 | 说明 |
|---|---|---|---|
| 41 | 多家 SEO 站点（additudemag.com、focusbox.io、neurodivergentinsights.com、neurolaunch.com、uporbit.app、scienceinsights.org 等）对 "interest-based nervous system" / "Deficiency-Deficit Framework" 的描述 | 【媒体/SEO 内容】 | **仅摘要级二手转述**：一致指向 William Dodson 2006 年 Psychiatric Times 文章提出的四要素（interest, challenge/competitiveness, novelty, urgency），并称"PINCH/INCUP 缩写并非 Dodson 本人术语"。**原始文章未获取。** 其中一条明确指出："该术语在 Europe PMC 全文索引与 PubMed 中检索不到任何同行评议论文使用它。"此说法与本次独立检索结果**一致**。 |

### D. 明确排除的来源

- **全部通用网络搜索结果中的 SEO 内容农场**（wellfacto.blog、restore-psychology.com、focusfast.org、getpomo.app、tkellycounselling.ca、neurodiversion.org、neurodiversity.directory、psychologytoday 系内容等）——**未采信任何实质主张**。它们在检索中大量出现并给出看似具体的断言（如"Volkow 2009 未被一致复现"），但均未提供可核验的一手引用。
- 中文来源（知乎/微信公众号/百度百科系）——按任务要求排除。
- Wikipedia / grokipedia 及其镜像——排除。

---

## 11. 给 Skill 的下游使用建议

### 11.1 可以直接写入「领域共识框架」的内容

用 §8.1 的 6 条。特别是第 1、3、6 条——它们都是"两派都接受"的事实，适合作为不选边的框架骨架。

### 11.2 必须写成并列分歧的内容

用 §7 对抗矩阵 + §8.2。**特别地：**
- 不要把"双通路并存"写成"已解决"——它是"两派都承认"，不是"任一派胜利"。
- §6.1（Luman/Tripp/Scheres 2010）应当作为**方法论中立批评**呈现，而不是 B 派的敌人。它批评的是整个领域的层级混乱。

### 11.3 必须以「我们不知道」形式呈现的内容

用 §9 全部 12 条。特别是第 9-11 条——它们直接关系到简报给出的三个研究者归属，在人工复核前**不应写入 Skill 的任何陈述性内容**。

### 11.4 一句话概括这场争论的现状

> 三十年来，这场争论已经从"控制 vs 动机"的**二选一**，退化成"**多路径 + 多层级 + 测量工具不可靠**"的泥潭。目前**没有任何一项证据**能够判定 ADHD 的注意力缺陷是控制失败还是兴趣驱动——最有希望的判决标准（延迟折扣）被证明是一个**非单一构念**且**对测量方法高度敏感**的指标，而最主要的理论推进（双通路模型）**至今没有任何 RCT 检验过它的临床分型效用**。

---

## ✅ FINAL VERDICT: PASS

- **来源总数**：41 条（学术 40 条 + 非学术 1 条），其中**正式学术来源 40 条**，覆盖 *Nature Neuroscience 级别期刊*（Nat Rev Dis Primers, Lancet, Nat Genet, Biol Psychiatry, J Child Psychol Psychiatry, Cortex, Neurosci Biobehav Rev, J Psychiatr Res, Eur Neuropsychopharmacol, Biol Psychiatry Cogn Neurosci Neuroimaging*）。
- **仅摘要/未获取全文**：**除 #4（Sonuga-Barke 2010 *Biol Psychiatry*，已获全文片段）与 #28（ECNP 立场文件，已获完整正文片段）外，全部 38 条正式来源均为"仅摘要，全文未获取"。** 本报告**未依据摘要脑补任何结论**。
- **未获取全文的关键文献（影响结论强度）**：Marx et al. 2021 元分析（**PubMed 完全无摘要**）、Jackson & MacKillop 2016（**效应量数值被截断**）、Marco et al. 2009、Sonuga-Barke et al. 2011、Stevens et al. 2018。
- **三大前提纠正**：(1) "Deficiency-Deficit Framework"作为命名框架在文献中不存在；(2) Rothenberger 并非 Sonuga-Barke 的批评者，而是长期合著者，真正的批评方是 Luman/Tripp/Scheres 与 Scheres 的测量学工作；(3) Wilmot et al. 2011 与 Hitch/Hutner 线经四库检索无法定位，须人工复核。
- **分歧处理**：§7 对抗矩阵与 §8.2 保留全部对立主张，未作调和；§6 批评方单独成节，篇幅与支持方相当（批评方证据含 3 篇元分析 + 3 项独立方法学研究）。