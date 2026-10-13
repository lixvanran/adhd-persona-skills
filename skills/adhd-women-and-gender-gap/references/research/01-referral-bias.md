# 维度 1–2 调研：推荐偏倚的量化证据 + 女性被漏诊的机制链

> 调研日期：**2026-10-12** · 调研 agent：general
> 目标：为 `adhd-women-and-gender-gap` 主题 Skill 提供「性别诊断缺口」方向的可核实一手材料。
> 取材方式：PubMed E-utilities efetch（直连 XML 摘要）+ Europe PMC REST API（含 OA 全文）+ Crossref API。**未使用通用搜索引擎**。
> 信源分级：【同行评议论文】/【仅摘要】/【OA全文】/【机构声明】/【媒体报道】/【患者社区声音】/【研究者推断】/【书籍·临床著作】
> 黑名单（知乎 / 微信公众号 / 百度百科 / grokipedia 及镜像）已排除。
> ⚠️ 全文未获取的一律标注「仅摘要，全文未获取」，**不猜测任何效应量数值**。

---

## 0. 本文件的核心结论（先看这个）

1. **不存在单一可信的「男:女诊断比」**。所有已发表数字落在 **1.4 : 1 到 10 : 1** 之间，跨度近 7 倍。差异不是测量误差，而是四个口径各自决定的：**(a) 社区样本 vs 临床转介样本；(b) 年龄段；(c) 信息源（家长/教师/双报告一致）；(d) 国家医疗体系与年代**。下文 §1.3 逐条并列。
2. **最可靠的单一数字取决于用途**。若要一个「美国儿童总体诊断率」的口径，用 CDC 家庭报告口径的 **约 2:1**；若要描述「谁会走进 ADHD 专科门诊」，用临床转介口径的 **约 4:1**；若要描述「未被识别的总体人群与被识别的差距」，用社区 vs 临床的比值。
3. **机制链上有两处是硬证据（registrar / 客观测验 / 项目层 DIF），三处是软证据（叙述性综述、二手引用、概念论证）**。见 §2 的分级标注。**「内在化 → 不被标记 → 被误诊为焦虑/抑郁」这条主链有真实的队列证据支持；但「DSM-5 起病年龄 7→12 的改动直接打开了女性通道」这条因果链，本次检索未找到任何一项把该改动与成人女性诊断率变化做过不连续性检验（interrupted time series / difference-in-differences）的实证研究。这是一条明确的证据空白，不能在 Skill 里写成已证实的因果。**

---

# 维度 1：推荐偏倚的量化证据

## 1.1 指定核实项：Mowlem et al. 2019 —— 已核实

> **"Sex differences in predicting ADHD clinical diagnosis and pharmacological treatment."** *European Child & Adolescent Psychiatry* 2019;28(4):481–489.
> DOI **10.1007/s00787-018-1211-3** · PMID **30097723** · 【仅摘要，全文未获取】· 可信度：**高**

**核实结果（任务书中的信息全部成立）：**

| 项目 | 内容 |
|---|---|
| 期刊卷期 | **Eur Child Adolesc Psychiatry 28(4):481-489, 2019** ✅ 与任务书一致 |
| 样本量 | **19,804 对双胞胎（50.64% 男性）**，父母在孩子 **9 岁**时完成 ADHD 症状、conduct 问题、学习问题的维度评估 |
| 数据链接 | 与瑞典 **Patient Register** 的临床 ADHD 诊断 + 处方记录链接 |
| 设计类型 | 队列级**人群样本** + 行政登记链接（非转介样本） |

**核心发现（原文口径）：**

1. **在人群层面，男性在所有症状维度上分数都更高**（注意问题、多动/冲动、conduct、学习问题）。
2. **但在「已被临床诊断」的人当中，男性与女性的症状严重度相似。**
   → 这是整个性别偏倚论证的枢纽：**被诊断的女孩必须比被诊断的男孩症状更重，才能进入诊断队列**。
3. **性别 × 症状域的交互作用**（决定「谁被诊断」与「谁拿药」）：

| 预测因子 | 女性中 → 获得诊断 | 女性中 → 获得药物治疗 |
|---|---|---|
| 多动/冲动 | **OR 1.08（95% CI 1.01–1.15）** | **OR 1.24（95% CI 1.02–1.50）** |
| Conduct 问题 | **OR 1.43（95% CI 1.09–1.87）** | **OR 2.20（95% CI 1.05–4.63）** |

作者结论原话（摘要）：
> "Females with ADHD may be more easily missed in the ADHD diagnostic process and less likely to be prescribed medication **unless they have prominent externalising problems**."

⚠️ **给 Skill 的关键提示**：多动/冲动对女性诊断的 OR 只有 **1.08**，CI 下限 **1.01** —— **统计显著性极边缘**。conduct 问题的 OR（1.43 / 2.20）才是强信号，且 conduct 问题在女孩中远不如男孩常见。**这是「女孩必须更严重、且必须外显才会被诊断」的直接量化表达。**

**配套论文（同一研究组，同期）**

> **"Do different factors influence whether girls versus boys meet ADHD diagnostic criteria? Sex differences among children with high ADHD symptoms."** *Psychiatry Research* 2019;272:765–773.
> DOI **10.1016/j.psychres.2018.12.128** · PMID **30832197** · 【仅摘要，全文未获取】· 可信度：高

- N = **283 名 7–12 岁儿童**（人群基础研究）。
- 用**研究者主导的结构化访谈**判定诊断；对照组为「量表症状高但未达诊断标准」的儿童。
- 两条关键发现：
  1. **情绪问题（emotional problems）是区分「已诊断女孩」与「高症状未诊断女孩」的关键变量，而在男孩中不是。** 效应量在女孩中更大。
  2. **父母对已诊断男孩的功能损害评分显著高于高症状未诊断男孩；父母对女孩则不做这种区分**，并且**父母系统性地低估了已诊断女孩的多动/冲动症状**（相较客观访谈），男孩则相反（高估）。
- 作者结论（摘要）："Results suggest girls' ADHD **may need to be made more prominent by additional behavioural/emotional problems** for them to meet full diagnostic criteria."

---

## 1.2 其他关键转介偏倚研究（本次检索补充，共 8 项）

### 1.2.1 威尔士 · 全国医疗记录（最直接的国家级证据）

> **"Sex differences in attention-deficit hyperactivity disorder diagnosis and clinical care: a national study of population healthcare records in Wales."**
> *Journal of Child Psychology and Psychiatry* 2024. DOI **10.1111/jcpp.13987** · PMID **38864317** · 【仅摘要，全文未获取】· 可信度：**高**

- 队列：**16,458 名被诊断为 ADHD 者**，1989–2013 年出生，2000–2019 年居住于威尔士，年龄 3–30 岁。**女性占 20.3%。**
- **男:女 = 3.9 : 1**。
- **按年龄分层（关键）**：
  - **<12 岁诊断者：4.8 : 1**
  - **>18 岁（成人期）诊断者：1.9 : 1**
- 男性首次记录诊断年龄更早：**10.9 岁 vs 12.6 岁**（女性晚 **1.7 岁**）。
- **诊断遮蔽（diagnostic overshadowing）的直接证据**：**女性比男性更可能在获得 ADHD 诊断之前先拿到焦虑、抑郁或其他精神健康诊断，并被处方抗抑郁药。**
- 这些性别差异「在不同人口学亚组间大体稳定」。
- 作者结论：女性「正在经历**更晚的识别与治疗**」，部分原因可能是「**其他精神健康状况（尤其焦虑与抑郁）的诊断遮蔽，或初次误诊**」。

> ⚠️ **注意**：这与 JCM 综述里提到的「瑞典登记研究显示女性晚约 4 年」是**两个不同来源、不同幅度**，见 §3 冲突清单。

### 1.2.2 台湾 · 全国人口数据库 2000–2011

> **"Trends in incidence rates of diagnosed attention-deficit/hyperactivity disorder (ADHD) over 12 years in Taiwan: A nationwide population-based study."**
> *Psychiatry Research* 2020. DOI **10.1016/j.psychres.2020.112792** · PMID **31981938** · 【仅摘要，全文未获取】· 可信度：高

- **265,932 名**新诊断 ADHD 患者。发病率（IR）从 **7.92 → 13.92 / 万人年**。
- **男:女比从 3.61 降到 2.90**（12 年内收窄）。
- 儿童/青少年/青年成人中男性 IR 增幅更大；**成人（>31 岁）中反而女性增幅更显著**。
- 亚型：≤18 岁以**combined 型**上升最显著；>18 岁以 **inattentive 型**上升最显著。

> **对本 Skill 的价值**：这是**「差距随时间收窄」最直接的一条时间序列证据**，且收窄主要发生在**成人期女性**——与「延迟识别」而非「患病率差异」的理论预测一致。

### 1.2.3 丹麦 · 药物处方数据 2010–2023

> **"Use of Attention Deficit Hyperactivity Disorder Medication Among Danish Children and Adolescents From 2010 to 2023."**
> *Acta Psychiatrica Scandinavica* 2026. DOI **10.1111/acps.70103** · PMID **42011750** · 【仅摘要，全文未获取】· 可信度：高

- 5–17 岁，**按处方配给**分析（≠ 诊断）。
- **男孩发病率**：0.59（2010）→ 0.34（2014）→ 1.0（2023）/ 100 人年。
- **女孩发病率**：0.20（2010）→ 0.67（2023），**连续上升**。
- **2023 年患病率比例**：男孩 **3.4%**，女孩 **1.8%**（≈ 1.9 : 1）。
- **男女发病与患病比在 2010–2023 年间持续下降。**
- **用药起始中位年龄：女孩 13 岁，男孩 11 岁（差 2 年）。**
- 作者原话：「女孩用药患病比例**翻了三倍**，而男孩只增长 1.5 倍。这**可能**反映了对女孩 ADHD 的认识提高，但**她们比男孩晚 2 年才开始治疗，这一点需要临床关注**。」

### 1.2.4 澳大利亚新南威尔士 · 出生队列 89,587 人（最早「求助年龄」）

> **"Sex Differences in the Age at First Health Service Use for ADHD Among Australian Children."**
> *Journal of Attention Disorders* 2026. DOI **10.1177/10870547261474901** · PMID **42541370** · 【仅摘要，全文未获取】· 可信度：高

- **89,587 名儿童**从出生随访至约 18 岁，链接行政健康记录（**处方 + 精神卫生服务使用 + 急诊 + 住院**）。
- 18 岁前因 ADHD 使用过医疗服务的儿童：**7,402 人（8.3%）**。
- **女孩 5.5% vs 男孩 10.9%（约 2 : 1）**。
- **首次求助年龄：女孩中位 13.6 岁（众数 17），男孩中位 9.4 岁（众数 7）。**
- ⚠️ 这是**「求助/服务使用」**而非「诊断」，但它是漏诊链条上**更靠前的一环**——女孩连「去看医生」这一步都更晚。

### 1.2.5 新西兰 · 全国普查链接行政数据（2023）

> **"Prevalence of Attention-Deficit Hyperactivity Disorder Across Gender and Sexual Identity Groups in Youth: A Whole-of-Population Study."**
> *Journal of Attention Disorders* 2026. DOI **10.1177/10870547261474553** · PMID **42560122** · 【仅摘要，全文未获取】· 可信度：高

- **1,266,456 人**（5–24 岁），**43,095 人（3.4%）**有 ADHD 记录。
- **男性 4.6% vs 女性 2.0%（≈ 2.3 : 1）**。
- **跨性别/其他性别身份者 10.3%**，跨性别者 9.9% vs 非跨性别 3.4%。
- 15–24 岁非异性恋者 8.0% vs 异性恋 3.6%。

### 1.2.6 苏格兰 · 30 个多学科团队的病历

> **"Are we getting better at identifying and diagnosing neurodivergent girls and women? Insights into sex ratios and age of diagnosis from clinical population data in Scotland."**
> **Maciver D et al.** *Autism* 2026;30(2):375-389. DOI **10.1177/13623613251383343** · PMID **41157911** · 【仅摘要，全文未获取】· 可信度：中（**样本极小 n = 408**）

- **408 人**（ADHD + 自闭症 + 智力障碍合计），30 个多学科团队。
- **全病种全生命周期男:女 = 1.31**。
- **2026-10-12 回炉更正**：原文摘要为「combining all diagnoses, **females** were referred later (median ages: **14.4 vs 19.7 years**; p < .001) and diagnosed later (median ages: **15.2 vs 20.2 years**; p < .001), **indicating a 5-year delay**」——**男 14.4 / 女 19.7（转介），15.2 / 20.2（诊断）**。此前「无法确定哪个属于女性、不可引用」的判断属**过度保留**，已作废；英文原文「females … 14.4 vs 19.7」的顺序是先女后男，与本底稿此前假设相反。
- ⚠️ **三重限制仍必须写进 Skill**：(a) 样本 408 人；(b) 男女比 1.31 与全部年龄中位数都是**三种神经发育障碍合并**的口径，**不是 ADHD 专属**；(c) 引用中位数时必须带「三病种合并」这一分母限定。

### 1.2.7 荷兰双胞胎 · 非转介样本（定位偏倚的**来源设置**）

> **"Why more boys than girls with ADHD receive treatment: a study of Dutch twins."**
> *Twin Research and Human Genetics* 2007;10(5):765-770. DOI **10.1375/twin.10.5.765** · PMID **17903118** · 【仅摘要，全文未获取】· 可信度：高

- **非转介样本**：283 名男孩 + 291 名女孩。
- **母亲报告**：有 ADHD 的男孩与女孩在**精神疾病水平、学校功能损害、攻击行为、注意力问题上都相似**。
- **教师报告**：教师**一贯地**给有 ADHD 的男孩打出更高的注意力问题与攻击分。
- 作者结论：「**性别差异随场景变化：男孩和女孩在家中被评为行为不同，在学校不被评为不同。教师报告的问题行为水平更高，可能解释了临床环境中 ADHD 的高男:女比。**」

> 🔑 **这是本文件里最重要的一条机制定位**：偏倚**不在家里，在学校**。而学校的关键信息源是教师。这直接连到 §2.3 的工具偏差与 §2.5 的转介链条。

### 1.2.8 「性别差异化关联」实证检验的反面证据（**必须并列**）

> **"A Comprehensive Examination of Sex-Differentiated Correlates of Attention-Deficit/Hyperactivity Disorder Symptoms in Late Childhood and Early Adolescence."**
> *Clinical Psychological Science* 2026. DOI **10.1177/21677026261454238** · PMID **42719335** · 【仅摘要，全文未获取】· 可信度：高

- **N = 11,878 名 9–13 岁儿童，4 个波次**，检验 ADHD 症状与 **88 个外部效标变量**（精神病理学、神经认知任务等）的关联是否因性别而异。
- **3,760 项检验中只有 4.1%（157 项）支持显著的性别差异化关联。**
- 方向：ADHD 与**外化问题**的关联在男孩中更强；ADHD 与**内化 + 思维问题**的关联**也在男孩中更强**（这**反对**「女性 ADHD 更内在化」的强版本）。
- 作者结论：**大多数观察到的性别差异效应量「非常小到小」。**

> ⚠️ **必须与「女性 ADHD 有独特表型」的路线并列呈现，不得调和。** 这项研究是对「性别化 ADHD 表型」整个文献的实质性挑战，且它自己指出**发表偏倚可能高估了这些效应**（阳性结果更容易发表）。见 `02-consequences.md` §4.5 的同向讨论。

---

## 1.3 ⚠️ 核心量化问题：男孩诊断率是女孩的 2 倍、3 倍还是 4 倍？

### **答案：全部都对，取决于口径。以下是全部已核实口径的并列清单。**

| # | 来源 | 口径定义 | 样本/数据 | 男:女 | 类型 |
|---|---|---|---|---|---|
| 1 | **DSM-5 正文**（经 Consultant360 逐条评述转引，见 sibling skill 02 文件） | 临床诊断报告值 | — | **儿童 2:1；成人 1.6:1** | 【诊断手册文本】 |
| 2 | **Biederman J et al. 2002**, *Am J Psychiatry* 159(1):36–41. PMID **11772687** | 精神科门诊转介 | 140 男孩 + 140 女孩 ADHD；120 男孩 + 122 女孩对照 | 原文开篇即引用：**「clinic-referred (10 to 1) vs community (3 to 1)」** | 【同行评议】 |
| 3 | **JCM 2026 综述**（见 §2.7）综合：临床转介儿童样本 | 临床转介 | 多研究汇总 | **约 4:1** | 【同行评议综述】 |
| 4 | 同上，社区样本 | 人群 | 多研究汇总 | **2.4 : 1 至 3.2 : 1** | 【同行评议综述】 |
| 5 | 同上，瑞典大规模双胞胎研究 | 临床诊断层 vs 人群层 | 19,804 双胞胎 | **临床 2.5:1；人群 1.8:1** ⚠️ **该两个比值为 JCM 2026 综述（§1 参考文献 [3]=PMID 30097723）的转引，不在 Mowlem 摘要原文里，原始数字未获取** | 【同行评议，二手转引】 |
| 6 | **Xu G et al. 2018**, *JAMA Netw Open* 1(4):e181471. PMID 30646132（见 sibling skill） | 家长报告「医生曾告知」4–17 岁 | NHIS 1997–2016，n=186,457 | 男孩 14.0% vs 女孩 6.3% = **2.2 : 1** | 【同行评议】 |
| 7 | **Danielson ML et al. 2024**, *J Clin Child Adolesc Psychol*. DOI 10.1080/15374416.2024.2335625. PMID **38778436** | 家长报告曾被诊断 / 当前 ADHD，3–17 岁 | 2022 NSCH，n=45,169 | 总体曾诊断 **11.4%**（710 万）；当前 **10.5%**（650 万）。**摘要未给性别拆分** → 见 ⚠️ | 【同行评议】 |
| 8 | **伊朗·德黑兰人群调查**（Mohammadi MR 等, PMID **31833803**, *J Atten Disord* 2021;25(8):1058-1067） | K-SADS-PL 结构化访谈（**最严格口径**） | 30,532 名 6–18 岁 | 总体 4%；**男孩 5.2% vs 女孩 2.7% = 1.93 : 1** | 【同行评议】 |
| 9 | **威尔士全国登记**（§1.2.1） | 临床诊断，3–30 岁 | 16,458 | **3.9 : 1**；<12 岁 **4.8:1**；成人 **1.9:1** | 【同行评议】 |
| 10 | **台湾全国**（§1.2.2） | 新诊断发病率，2000 | 265,932 | **3.61 : 1**（2011 降至 2.90） | 【同行评议】 |
| 11 | **丹麦 2023**（§1.2.3） | 5–17 岁药物处方患病比例 | 全国 | **3.4% vs 1.8% = 1.9 : 1** | 【同行评议】 |
| 12 | **新西兰**（§1.2.5） | 终身诊断+治疗记录，5–24 岁 | 1,266,456 | **4.6% vs 2.0% = 2.3 : 1** | 【同行评议】 |
| 13 | **澳洲 NSW**（§1.2.4） | 18 岁前使用过 ADHD 医疗服务 | 89,587 | **10.9% vs 5.5% ≈ 2 : 1** | 【同行评议】 |
| 14 | **伊朗小学儿童 meta 分析**（PMID **40810952**, *Child Psychiatry Hum Dev* 2025） | DSM 量表，6–12 岁 | 9 项研究，9,138 人 | 男孩 **10.1%** vs 女孩 **7%** = **1.44 : 1** | 【同行评议综述】 |
| 15 | **埃及 Fayoum**（PMID **25814429**, *J Atten Disord* 2018） | 自建 DSM-5 量表，6–14 岁 | 420 人 | 男孩 **33.8%** vs 女孩 **6.8%** = **5 : 1** ⚠️ 量表口径极高，异常值 | 【同行评议】 |
| 16 | **印度 Belagavi**（Joshi HM 等, KLE University, PMID **29929414**, *J Atten Disord* 2021;25(2):154-160） | SNAP-IV 家长版 | n=156 | 女孩 3.8% vs **男孩 1.9%（女孩更高）** ⚠️ **反向** | 【同行评议，小样本】 |
| 17 | **EPINED 西班牙**（PMID **38695661**, *Autism Res* 2024） | 两阶段（家长+教师 → 个体评估） | 3,727 → 781 | ASD+ADHD 共病：女孩 0.16% vs 男孩 0.89% = **5.6 : 1** | 【同行评议】 |

### **为什么数字不同 —— 四个可分离的原因**

1. **抽样框（最主要）**。**社区/人群样本的比值系统性低于临床转介样本。** 同一批研究里可以直接看到这个落差：JCM 综述汇总的临床 4:1 vs 社区 2.4–3.2:1；瑞典双胞胎研究同一人群、两种口径 = **2.5:1（临床）vs 1.8:1（人群）**（⚠️ 此对比为 JCM 2026 综述的转引，非 Mowlem 摘要原文）。Biederman 2002 引用的老口径差距更大（10:1 vs 3:1）——那是 1990 年代末的数据，此后社区口径的比值持续下降。
2. **年龄带**。**越年轻，比值越大。** 威尔士同一数据库内：<12 岁 4.8:1，成人 1.9:1。**把「儿童的比值」当成「全体的比值」是最常见的错误。**
3. **信息源与一致性要求**。⚠️ **这是本文件最反直觉的一条**：比值随信息源**收敛程度降低而升高**——
   - 家长 + 教师**双方一致**报告 ADHD：**5.3 : 1**（最高）
   - **仅教师**报告：**3.3 : 1**
   - **仅家长**报告：**2.5 : 1**（最低）
   → 含义：**要求跨场景一致性（DSM「广泛存在」标准）会把女孩筛掉得最狠**，因为女孩的症状更情境依赖、更内在、不易被两个场景同时观察到。数据来自 JCM 综述 §3.6 所引文献（原文标注 [60]）。**⚠️ 二手转引，未获原始文献。**
4. **测量方式**。家长报告的量表分数（尤其是 Achenbach / Conners / Quay 这类含大量行为条目、且经 JCM 综述转述称「临床转介样本中家长给女孩勾选注意缺陷条目的数量只有男孩的一半左右」的量表）会放大差距；结构化临床访谈（**伊朗德黑兰** K-SADS-PL 研究）给出的比值最低（1.93:1）。
5. **年代与国家体系**。台湾 12 年内 3.61→2.90；丹麦 13 年内持续下降；苏格兰显示比值随年龄**趋近平衡**。**跨年代引用旧数字而不注明年份，会系统性高估今天的差距。**

### **给 Skill 的单点答案**

> **如果必须给一个数字：**
> - **「美国儿童总体被诊断率」→ 约 2 : 1**（口径：CDC/NSCH 家庭报告「医生曾告知」，3–17 岁；2018–2022 年数据）。这是可用于公众传播、且口径最稳定的一个。
> - **「谁会被送进 ADHD 专科」→ 约 4 : 1**；**若年龄 <12 岁 → 约 4.8 : 1**。
> - **「历史上门诊样本」的引用值可达 10 : 1**（Biederman 2002 引用的 1990 年代口径）—— **必须标注年代，否则会误导。**
> - **不存在**「女孩 ADHD 患病率只有男孩一半」的证据。结构化访谈研究（**伊朗德黑兰** K-SADS-PL）给出 **1.93 : 1**，几乎与 DSM-5 儿童报告值相同。

---

## 1.4 Willcutt 2012 —— 核实结果

**Willcutt EG.** "The prevalence of DSM-IV attention-deficit/hyperactivity disorder: a meta-analytic review." *Neurotherapeutics* 2012;9(3):490–499. DOI **10.1007/s13311-012-0135-8** · PMID **22976615** · 【仅摘要，全文未获取】· 可信度：高

**核实到的事实：**
- 纳入 **86 项儿童青少年研究（N = 163,688）** + **11 项成人研究（N = 14,112）**。
- 汇总患病率：儿童青少年 **5.9%–7.1%**（家长报告、教师报告、最佳估计诊断程序**三种方法结果相近**）；青年成人自评 **5.0%**。
- 亚型：**predominantly inattentive 型是人群中最常见的亚型**，但 **combined 型更可能被转介到临床服务**。
- 作者明确写道：「**仍需研究确定 ADHD 在男性中高于女性的病因**」——**即 Willcutt 2012 本人没有宣称「差距是偏倚造成的」，也没有宣称「差距是真实生物学差异」。**

### ⚠️ 核实结论（必须写进 Skill）

**Willcutt 2012 的摘要中没有任何男:女比例数字。** 我通过 PubMed efetch 与 Europe PMC 两条独立路径核实，均未在摘要中出现 sex ratio 数值。网络上广泛流传的「Willcutt 2012 说成人期 1:1、儿童 2:1」这一表述，**我无法从该论文的摘要证实**。

- 任务书提到「核实 Willcutt 2012 关于成人期性别差距的结论（核实原文）」→ **核实结果：摘要层面无此结论**。全文未获取（Neurotherapeutics 2012 非 OA）。
- 若 Skill 需要引用 Willcutt 2012 的性别差距数字，**必须先获取全文核对**；目前只能引用其患病率与「inattentive 型最常见但 combined 型更可能被转介」这两条。

**配套的更近版本（更推荐使用）：**

> **Willcutt EG, et al. (2014).** "ADHD prevalence estimates across three decades: an updated systematic review and meta-regression analysis." *International Journal of Epidemiology* 43(6):1401–1408. DOI **10.1093/ije/dyt261** · PMID **24464188** · 【仅摘要，全文未获取】· 可信度：高
> - 更新纳入 **154 项原始研究，135 项进入多元 meta 回归**。
> - 明确针对「诊断率与治疗率数十年来持续上升是否意味着真实患病率上升」的关切做方法学解释。
> - 同样在**摘要中未给出男:女比例**。

---

# 维度 2：女性为何被漏诊 —— 机制链

> **本节的分级原则**：⚠️ **有队列/客观测验/项目层 DIF 支撑的** 与 **只有综述转述、概念论证、二手引用的** 必须分开标注。二手引用一律标 ⚠️。

## 2.1 内在化 vs 外显化：行为差异链条（**证据最硬的一环**）

### 链条 Step 1：诊断手册的样本本身就是男性偏的

来源：Salehpour F, Gonzalez-Lima F. "Sex Bias in the Clinical Diagnosis of ADHD: A Critical Review." *Journal of Clinical Medicine* 2026;15(17):6804. DOI **10.3390/jcm15176804** · PMID **42739808** · **PMCID PMC13566458** · 【**OA 全文已获取**】· 可信度：高（但作者自陈为 critical narrative review，**非 PRISMA 系统综述**）

- **DSM-IV 现场试验（field trials）中女性仅占 21%。**
- **DSM-5 现场试验：儿科参与者中女性约占 40%；成人站点接近均衡（女性 48% / 男性 52%）。**
- → 即：**现行诊断标准是在 79% / 60% 为男性的样本上建立的。** 这是整条机制链的起点，且是可直接引用的硬事实（原文 §3.1，引其参考文献 [14][15]）。

### 链条 Step 2：女孩不"捣乱"，所以不给转介信号

- **课堂干扰效应（教师「被惹恼/被烦到」比例）**：⚠️ **女孩 38% vs 男孩 64%**（JCM 综述 §3.5 转引其参考文献 [56]）。
  - ⚠️ **二手转引，未获原始文献，引用时必须标注「经 JCM 2026 综述转引」。**
- **荷兰双胞胎研究（§1.2.7）提供了最干净的因果定位**：**在家里，男女孩表现无差异；在学校，教师系统性地把男孩的问题行为评得更高。** 这是**直接测量**而非推断。
- **父母对女孩的知觉偏差**（§1.1 配套研究，PMID 30832197）：**父母系统性低估已诊断女孩的多动/冲动症状**，且**不区分**「已诊断女孩」与「高症状未诊断女孩」的功能损害 —— 但对男孩做出正确区分。

### 链条 Step 3：女孩要拿诊断，必须额外带上情绪/行为问题

- **Mowlem（PMID 30832197）**：「情绪问题对区分已诊断女孩与高症状女孩特别关键，对男孩不关键。」
- **Mowlem（PMID 30097723）**：「除非有突出的外化问题，女性 ADHD 在诊断过程中更容易被漏掉。」多动/冲动 → 诊断的 OR 仅 1.08（CI 1.01–1.15）。
- ⚠️ **JCM 综述 §3.5 转引**：在临床转介样本中，**家长对女孩勾选的注意缺陷条目数量约为男孩的一半**（Achenbach / Conners / Quay 量表）。标注为二手引用。

### 链条 Step 4：漏掉的女孩去了哪里 → 诊断遮蔽（**有登记数据**）

- **威尔士登记研究（PMID 38864317）**：**女性比男性更可能在 ADHD 诊断之前获得焦虑、抑郁或其他精神健康诊断并被处方抗抑郁药。** ← 这是链条终点最硬的一条证据。
- **JCM 综述 §3.7**：在**成人女性**中，ADHD 与**焦虑、抑郁、双相障碍、人格障碍**的关联强于成人男性；且「 ADHD 在成人女性中与这些诊断的更强关联」本身即构成遮蔽风险。
- **早期描述性证据**（与 2026 登记研究方向一致）：
  > **Biederman J, Ball SW, Monuteaux MC, 等**（⚠️ 第一作者为 Biederman，非 Mick）"New insights into the comorbidity between ADHD and major depression in adolescent and young adult females." *J Am Acad Child Adolesc Psychiatry* 2008;47(4):426-434. PMID **18388760**. 【仅摘要，全文未获取】
  > - N = 140 ADHD 女性 + 122 对照，5 年前瞻，来源为儿科/精神科转介。
  > - **有 ADHD 的女性在青少年随访时重度抑郁风险为对照女性的 2.5 倍**（已校正精神科共病）。
  > - ADHD 女性的重度抑郁表现为：**起病更早、持续时间超过 2 倍、抑郁相关损害更重、自杀率更高**。
- **印度三级医疗中心**（PMID **40043536**, *Asian J Psychiatry* 2025）：101 名 18–45 岁成人，**女性在 ASRS 上平均分显著高于男性**，并报告更多**mind-wandering、hyper-focusing、motor-coordination 困难、自尊降低、去士气化、情绪不稳**。【仅摘要，样本小（23 名女性）】

### 链条 Step 5：自我诊断与「我的 ADHD 不符合标准」

- **奥地利 93 名临床心理学家调查**（PMID **41551064**, *Int J Clin Health Psychol* 2026;26(1):100661）：「自我诊断」与「希望获得的诊断」在出现率上显著高于中点，**大效应量（p < .001）**；ADHD 与 ASD 是自我诊断/希望诊断最多的两项。**临床心理学家描述此类就诊者「常被描述为女性、受教育程度高、深度参与线上活动」。**
  - 【同行评议，但样本是**专业人员印象**而非患者样本】· 可信度：中。**这条同时是「缺口存在」和「反向质疑」两边的证据，必须两边都用。**

---

## 2.2 Masking / compensation（掩饰与代偿）

### 2.2.1 直接测量研究

> **Owens EB, Zalecki C, Gillette P, Hinshaw SP.（BGALS 团队）** —— 见 §2.2.3 与 `02-consequences.md`。

### 2.2.2 「高功能、高痛苦」的构念（**这是 masking 代价目前最清楚的论证**）

> **"High functioning, yet high suffering - the need to incorporate invisible struggles in adult ADHD diagnostic assessment/criteria."** *Frontiers in Psychiatry* 2026. DOI **10.3389/fpsyt.2026.1813029** · PMID **42232996** · 【仅摘要，全文未获取】· 可信度：中（**观点/立场论文，perspective article，非原始研究**）

- 论证：DSM-5 成人 ADHD 标准依赖**外在可观察征象**与**可测量的功能损害**。对于**通过补偿策略与 masking 维持高学业/职业/社交表现，同时承受巨大内部痛苦**的个体，造成了一个**诊断盲区**。
- 「**对这类个体而言，损害并非不存在，而是隐藏在持续努力、完美主义性过度代偿（perfectionistic overcompensation）与慢性自我监控之下。**」由此产生的心理负担包括：**情绪耗竭、焦虑、羞耻、认知疲劳、生活质量下降**。
- ⚠️ **立场论文，不是数据。** 引用时必须标注为「理论论证」而非「实证发现」。

### 2.2.3 临床检查清单层面的信号（**有量化数据**）

> **"A Qualitative Analysis of Perspectives on Self-directed Violence in a Prospective Longitudinal Study of Young Women With and Without Childhood ADHD."** *Journal of Attention Disorders* 2024. DOI **10.1177/10870547231221729** · PMID **38294171** · **PMCID PMC11168017** · 【**OA 全文已获取**】· 可信度：高

- **57 名年轻女性**（32 名童年确诊 ADHD，25 名神经典型对照），平均 27 岁，来自 BGALS 的定性子样本。
- **关键主题 5（Masking 语境）**：「**把 NSSDV 保持为秘密（keeping NSSDV secret）**」被归纳为一个独立主题。
- 数据：**4 名 ADHD 组受试者与 1 名对照组报告其自伤行为「被他人影响」（父母发现后介入是减少或终止的关键）**。
- → **代价的直接证据：保密（secrecy）本身就是掩饰机制的一部分。**

### 2.2.4 掩饰与身份/冒名顶替/社交媒体

> **"Attention-Deficit/Hyperactivity Disorder, Imposter Phenomenon, and Identity Distress: The Mediating Indirect Effects of Self-Esteem, Social Camouflaging, and Social Media Connections."** *Behavioral Sciences* 2026;16(2):213. DOI **10.3390/bs16020213** · PMID **41750022** · 【仅摘要，全文未获取】· 可信度：中（**大学生样本 N=500，女性 61.6%，自报量表，样本性别构成本身接近 Skill 所关心的比例**）
> - 检验 SEM：ADHD 症状严重度 → **自尊、masking/social camouflaging、社交媒体连接** → **冒名顶替现象（imposter phenomenon）与身份困扰**的中介间接效应。

### 2.2.5 ⚠️ 掩饰研究的方法学现状（**重要的诚实警告**）

> **"A narrative review of stigma and masking in ADHD: insights from English-language research and the Japanese cultural context."** *Frontiers in Psychology* 2026. DOI **10.3389/fpsyg.2026.1807337** · PMID **41987980** · 【仅摘要，全文未获取】· 可信度：中（narrative review）

> 原文关键句（摘要）：**"empirical research on this phenomenon remains limited"** —— 关于 masking 作为「对污名的行为反应」的**实证研究仍然有限**。

> **另一条**：**"Diagnosis acceptance, masking, and perceived benefits and challenges in adults with ADHD and ASD"**（PMID **41169493**, *Frontiers in Psychiatry* 2025）：样本 **ADHD n=803 / ASD n=158 / 两者共病 n=95**，18–35 岁，**79% 为女性**。【仅摘要】
> ⚠️ **这是一个结构性偏倚警告：目前最大的 masking 问卷研究本身就是 79% 女性的自选样本。** 它能说明「在已经自我诊断/自我识别的女性中，masking 与诊断接受度、生活质量相关」，**不能**用来推断「女性 ADHD 总体上 masking 更严重」——后者需要一个**基于人群的、含未诊断女性的**对照设计，目前不存在。

> 🔑 **给 Skill 的诚实结论**：**「掩饰是漏诊的机制」是理论上高度合理、临床描述上高度一致、但独立操作化并做组间比较的研究仍然很少的领域。** Skill 里应把 masking 表述为「**机制假说 + 临床一致描述**」，而非「**已证实的量化机制**」。

---

## 2.3 工具偏差：哪些筛查工具对女性不友好？

### 2.3.1 客观测验 vs 主观量表（**关键的一组对照数据**）

> **"Gender Differences in Objective and Subjective Measures of ADHD Among Clinic-Referred Children."** *Frontiers in Human Neuroscience* 2019;13:441. DOI **10.3389/fnhum.2019.00441** · PMID **31920599** · 【仅摘要，全文未获取】· 可信度：高

- **204 名 6–17 岁临床转介 ADHD 儿童（129 男孩 / 75 女孩）**，回顾性病历分析。
- 工具：**家长版与教师版 Conners ADHD 量表**、CBCL、TRF，以及 **CPT（连续表现测验，客观）**。
- 结果：
  - **主观（家长 + 教师报告）：女孩的注意问题多于男孩；多动/冲动水平无性别差异。**
  - **客观（CPT）：男孩冲动性更高。**
  - **CPT 上的分心干扰（视觉/听觉/组合）与干扰负荷（1 个 vs 2 个）效应不因性别而异 → 女孩在 CPT 任务上的分心困难没有被检出。**
- 作者结论：**「性别效应在主观与客观测量之间可能不同。」**

> 🔑 **这是「量表对女性不友好」最干净的证据形态：同一样本、同一批孩子，主观量表说女孩注意问题更多，客观任务说男孩冲动性更高 —— 两个测量给出方向相反的性别画像。** 也就是说：**如果临床依赖家长/教师量表做筛查，男孩的冲动性会被放大、女孩的分心困难会被漏掉。**

### 2.3.2 项目层差异性条目功能（DIF）—— Williams 等 meta 分析

来源：JCM 2026 综述 §3.2 **【OA 全文已获取；Williams et al. 原始文献为二手转引 ⚠️】**

**（a）家长评定的儿童青少年 ADHD（DSM-IV 条目）：**

| 条目 | 女孩相对男孩的 OR | 方向 |
|---|---|---|
| easily distracted（容易分心） | **1.54** | 女孩更高 |
| fails to sustain attention in tasks（难以维持任务注意力） | **1.39** | 女孩更高 |
| blurts out answers（脱口而出答案） | **0.86** | 男孩更高 |
| interrupts others（打断别人） | **0.75** | 男孩更高 |
| talks excessively（话多） | **0.93** | 男孩更高 |

- 其余 8 个条目**无显著性别差异**。最强效应为「容易分心」与「脱口而出答案」。

**（b）成人 ADHD 自评（DSM 条目）：**

| 条目 | 女孩相对男孩的 OR | 方向 |
|---|---|---|
| often easily distracted | **1.49** | 女孩更高 |
| often has difficulty organizing tasks | **1.40** | 女孩更高 |
| often blurts out answers | **1.32** | **女孩更高** ⚠️ |
| often talks excessively | **1.65** | **女孩更高** ⚠️ |

- 其余 12 个条目**无显著性别差异**。

> ⚠️⚠️ **必须并列指出的内部冲突**：在**儿童**样本中，「talk excessively」「interrupts others」「blurt out answers」偏向**男孩**；在**成人**样本中，这三条**全部反向**，偏向**女性**（OR 1.32 / 1.65）。**同一个 DSM 条目在儿童期与成年期的性别方向相反。** 这可能反映真实的行为表达随年龄改变，也可能反映两个样本的构成差异（临床转介 vs 成人门诊）。**Skill 里不能只引用其中一边。**

**（c）多动/冲动维度**：**9 条 DSM-IV 多动/冲动条目中有 8 条在男孩中更常被勾选，唯一的例外是「talks excessively」。**

### 2.3.3 ⚠️ 反面证据：DSM 条目在两性间**大体测量等价**

- JCM 综述 §3.2 转述其参考文献 [23][24]：**来自学前到 9 年级的 18 条 DSM-IV ADHD 条目的纵向家长评定，绝大多数表现出强测量等价性与跨性别的极小 DIF。** 即：这些条目在男孩和女孩身上测的是**同一个潜在构念**。
- **JCM 综述作者自己的结论（必须引用，因为它限制了本节的激进版本）**：
  > 「**由于大多数 DSM 定义的 ADHD 症状在两性间功能相似，且只在条目子集上发现性别相关的 DIF，现有证据尚不足以支持对 DSM 症状标准做广泛修改。**」

### 2.3.4 ⚠️ 关于「Conners' 10-item screener 偏向多动条目」这一具体说法

**核实结果：本次检索未找到任何一项对 Conners 简版/10 条目量表做分性别的信度-效度或敏感性分析的研究。**

- 能拿到的最接近证据是 §2.3.1（Conners 完整版的主观/客观分裂）与 §2.3.3（DSM 条目跨性别测量等价）。
- **结论**：任务书中「Conners' 10-item screener 偏向多动条目」这一表述，**在本次检索范围内属于【社区/临床从业者主张】，未被同行评议的分性别心理测量学研究证实。** Skill 中若要保留，必须标为**未证实的从业界印象**。
- **可替代的、有证据的相近主张**：**DSM「跨两个场景」（pervasiveness）标准 + 要求家长与教师双报告一致，是把女孩筛掉最狠的单一工具设计**（5.3:1 vs 2.5:1，见 §1.3 原因 3）。

### 2.3.5 成人诊断工具本身的性别偏向

> **"Bias by gender: exploring gender-based differences in the endorsement of ADHD symptoms and impairment among adult patients."** *Frontiers in Global Women's Health* 2025. DOI **10.3389/fgwh.2025.1549028** · PMID **40182228** · 【仅摘要，全文未获取】· 可信度：中

- **2,257 名**荷兰 Parnassia Groep 精神卫生门诊**已被诊断**的成人患者的 DIVA-5 数据。
- 发现：**ADHD 在男女身上「表现相似」**，出现细微差异。
- **女性更常勾选若干「成年期」注意问题与多动/冲动条目；男性在若干「童年期」条目上勾选率更高。**
- 功能损害领域：**自尊与社交关系**出现性别特异模式。
- 作者建议：**DIVA-5 需考虑测量局限并作改进。**

> ⚠️ **这实际上是对「工具偏向论」的一个内部挑战**：在一个已经拿到诊断的成人样本里，**DIVA-5 的条目勾选并没有表现出大幅性别偏倚**。Skill 应把它作为「工具偏倚论」的边界条件写入。

---

## 2.4 DSM-5 起病年龄改动的因果作用 —— ⚠️ **一项实证研究都没找到**

### 2.4.1 支持「年龄标准造成漏诊」的机制性证据

来源：JCM 2026 综述 §3.4 **【OA 全文已获取】**

- **女性的多动/冲动症状往往在青春期早期才开始上升；男性在约 7 岁就已升高**（青春期还会再升一次）。
- **女性注意缺陷症状的起病也延迟** —— 在相对稳定的童年环境中低于诊断阈值、不具破坏性，但在**青春期学业要求提高、父母支持下降、独立性增加、以及青春期后的激素变化**共同作用下跨入临床范围。
- **「迟发型 ADHD」人群更可能是女性**；而童年起病且持续者呈现典型的男性优势。
- **部分被识别为迟发型的女性成人，追溯发现童年有细微的认知困难与可比的遗传易感性** —— 提示所谓「迟发」有时是**识别延迟**而非**症状新发**。

### 2.4.2 ⚠️ 但因果检验是空白的

**检索结论：未找到任何一项把「DSM-5 起病年龄由 7 岁放宽到 12 岁」作为处理变量、对成人女性诊断率做中断时间序列（interrupted time series）或双重差分（difference-in-differences）检验的研究。**

我检索了以下路径，均未命中相关实证研究：
- `TITLE:"DSM-5" AND TITLE:"onset" AND ABSTRACT:"ADHD" AND ABSTRACT:"diagnosis rate"` → 0 命中
- `ABSTRACT:"DSM-5" AND ABSTRACT:"age of onset" AND ABSTRACT:"ADHD" AND ABSTRACT:"adult" AND ABSTRACT:"diagnos"` → 0 命中
- `ABSTRACT:"age of onset" AND ABSTRACT:"ADHD" AND ABSTRACT:"DSM-5" AND ABSTRACT:"diagnoses"` → 5 命中，全部不相关
- `"interrupted time series" AND "ADHD"` 与 `"DSM-5" AND "before-and-after" AND "ADHD" AND "diagnoses"` → 命中的中断时间序列研究全部是**哌甲酯短缺、监管改革、COVID 封控**等，不是 DSM 判准变更

### 2.4.3 现有的准证据（**时间相关，不能当因果**）

| 证据 | 内容 | 能否归因于 DSM-5？ |
|---|---|---|
| 威尔士登记（PMID 38864317） | 女性诊断年龄 12.6 岁 vs 男性 10.9 岁；女性诊断前更常先有焦虑/抑郁诊断 | ❌ 不能。登记年份 2000–2019，**无法区分 DSM-IV 时期与 DSM-5 时期** |
| 台湾（PMID 31981938） | 男:女比 12 年内 3.61→2.90 | ❌ 不能。2000–2011 **跨越 DSM-IV/DSM-5 分界**，但未做分段分析 |
| 丹麦（PMID 42011750） | 2010–2023 男女比持续下降；女孩患病比例翻三倍 | ❌ 不能。**完全在 DSM-5 时期内**，无法与 DSM-IV 时期对比 |
| 苏格兰（PMID 41157911） | 比值随年龄趋近平衡 | ❌ 不能。横断面，非时间趋势 |

> 🔑 **必须并列保留的两条互斥解读**：
> - **解读 A（默认写入 Skill 的主流框架）**：差距收窄 = 女性被识别出来 = DSM-5 放宽 + 公众认知提高的结果。
> - **解读 B（现有证据同样支持，且无人反驳）**：差距收窄 = **基层患病率的真实性别比本来就接近 1.5–2:1，转介偏倚只影响「童年被识别的那部分」，成年后自助转介绕过了转介环节**。台湾研究中「**成人期女性发病率增幅更大**」这一现象，在这个解读下不需要 DSM-5 改动来解释。
>
> **本次检索没有任何一项研究能把这两条解读分开。**

### 2.4.4 DSM-5 判准本身也带性别偏倚（⚠️ 二手转引）

- **DSM-IV 现场试验仅 21% 女性；DSM-5 儿科现场试验约 40% 女性**（JCM 综述 §3.1，见 §2.1）。
- **6 条症状门槛**（17 岁及以上为 5 条）沿用自 DSM-IV，批评者认为这些阈值**反映的是男性更典型的症状模式**（JCM 综述 §3.3）。
- **JCM 综述 §3.3 的反向证据**：1994 年 **NIMH 会议**上，专家认为「为女性设定性别常模的诊断截断点」为时过早，警告**降低女性阈值会导致过度诊断**。后续研究支持在**量表**层使用分性常模（DuPaul 儿童量表、Barkley 成人量表），但**「用性别常模识别出的女性是否真有临床显著损害」缺乏证据**。
- **JCM 综述作者结论（须引用）**：
  > 「现有证据提出了对固定症状阈值识别女性表型的合理担忧，但**尚未确立**分性别的诊断阈值能在不增加假阳性风险的前提下提升诊断效度。」

---

## 2.5 误诊路径：女性 ADHD 的常见去向

### 2.5.1 焦虑 / 抑郁 —— **证据最强**

- **威尔士登记（PMID 38864317）**：**女性在 ADHD 诊断前更常被诊断为焦虑、抑郁或其他精神健康状况，并被处方抗抑郁药。**
- **Mick 2008（PMID 18388760）**：女性 ADHD 的**重度抑郁风险 2.5 倍**，且抑郁病程更重。
- **JCM 综述 §3.7**：女性 ADHD 的情绪困难「**可能以焦虑和抑郁等内化问题的形式遮蔽其 ADHD 症状**」，导致临床医生给出替代诊断。

### 2.5.2 双相障碍 —— ⚠️ 检索结果：**未找到分性别的误诊率研究**

- 我检索了 `AUTH:"Staley BS" AND TITLE:"ADHD" AND ABSTRACT:"bipolar"` 与 `TITLE:"bipolar" AND ABSTRACT:"ADHD" AND ABSTRACT:"children" AND ABSTRACT:"misdiagnos"`，**均 0 命中**。文献中广泛引用的 Staley 等 ADHD→双相误诊研究我未能定位到原始条目。
- 可用的**方向性证据**（非误诊率）：
  - **JCM 综述 §3.7**：在**成人女性**中，ADHD 与**双相障碍**的关联强于成人男性；且**女性的多动/冲动可能以外化的言语行为表现，被误解为焦虑障碍、边缘型人格障碍或双相障碍的症状**。⚠️ 二手转引其参考文献 [9][65][66][67]。
  - **区分困难的存在性证据**：`TITLE:"Adult ADHD vs. bipolar disorder in the DSM-5 era: a challenging differentiation for clinicians."` *J Psychiatr Pract* 2014;20(6):428–437. PMID **25406047**。【仅摘要】—— 确认「ADHD 与双相在临床上难以区分」是一个被正式承认的临床问题，**但该文不提供性别分层数据**。
  - **症状重叠的量化**：`"Overlaps and differences in the core symptoms of patients with ADHD and patients with borderline personality disorder."` *Frontiers in Psychiatry* 2026. PMID **42445552**。80 例 ADHD、55 例 BPD、55 例对照。**结果：ADHD 组与 BPD 组的「情绪失调」表达无显著差异；ADHD 组在冲动性、注意力不集中、活动过度上分数更高。** ⚠️ 仅摘要，全文未获取。

### 2.5.3 边缘型人格障碍（BPD）—— 有纵向证据

- **背景提示**：`"Developmental predictors of young adult borderline personality disorder: a prospective, longitudinal study."`（PMID **36793031**, *BMC Psychiatry* 2023，PMC9930262，OA）【标题与期刊已核实，**具体内容本次未提取**】
- **JCM 综述 §3.7**：**女性的多动/冲动以外化言语行为表现，可被误读为边缘型人格障碍症状。** ⚠️ 二手转引。
- **ADHD–BPD 共病的存在性证据**：`"Methylphenidate treatment in adults with comorbid ADHD and borderline personality disorder: a prospective longitudinal study."` *Int Clin Psychopharmacol* 2026. PMID **42127382**。36 名成人，24 名（66.7%）完成 ≥16 周随访。【仅摘要】。⚠️ **该研究证明共病存在且可研究，但不等于「女性 ADHD 被误诊为 BPD」的证据。**

> 🔑 **诚实结论**：**误诊率（diagnosis error rate）在女性 ADHD 这一人群中基本没有被量化过。** 现有的是**通路证据**（女性在 ADHD 诊断前更常拿到焦虑/抑郁诊断——这条有登记数据）与**重叠证据**（ADHD 与 BPD/双相的症状重叠有量化，但不分性别）。**Skill 里不应给出「X% 的女性 ADHD 被误诊为 Y」这种数字。**

### 2.5.4 一条被忽略的反向数据：成年后**双重诊断重叠**高于纯误诊

> **"Girls With Social and/or Attention Deficit Re-examined in Young Adulthood: Prospective Study of Diagnostic Stability, Daily Life Functioning and Social Situation."** *J Attention Disord* 2023. DOI **10.1177/10870547231158751** · PMID **36915033** · 【仅摘要，全文未获取】· 可信度：高

- BGALS 样本：**17–20 年随访，100 名女孩中 92 名童年确诊 ADHD 或 ASD**，对照 60 名；随访时检查 90 / 54 名（**M = 27 岁**）。
- **89% 的女性在随访时仍符合 ADHD 或 ASD 中任一诊断**；**「极少有人在缓解（in remission）」。**
- **⚠️ 34% 的女性主诊断从 ADHD 转为 ASD。**
- ADHD + ASD 共病者功能损害与社会处境显著差于对照。

> **「34% 主诊断从 ADHD 转为 ASD」这一条，与「成年女性 ADHD 被误诊」的故事方向相反：它说明 BGALS 队列里相当一部分女性在成年后被重新归入自闭症谱系，而非「ADHD 是错的」。任何关于「成年女性 ADHD 诊断」的 Skill 内容都必须处理这个事实。**

---

## 2.6 「内在多动 / 内在化」这一 Littman 概念在文献中的位置

- **任务书提供的 Littman 材料（《Understanding Girls with ADHD》、internal hyperactivity、冰淇淋/游乐场/晕车呕吐的例子、雌激素触发、最多落后 10 年）在本次检索中未被任何同行评议实证文献直接验证。** 这些出自 **【书籍·临床著作】**（Littman E, Quinn P, Nadeau K, *Understanding Girls with ADHD*, 2nd ed., Guilford Press），属于**奠基性临床叙述**，不是可检验的实证结果。
- **能够被检索到的、与「内在多动」机制最接近的同行评议研究**：

> **"Evaluating a scale of excessive mind wandering among males and females with and without ADHD from a population sample."** *Scientific Reports* 2019;9(1):3071. DOI **10.1038/s41598-019-39227-w** · PMID **30816143** · 【仅摘要，全文未获取】· 可信度：高

- 目的：明确指出**「心智游走」对许多「外在表现较少的」个体（包括女性）尤其相关**。
- 工具：Mind Excessively Wandering Scale（MEWS），基于**在线一般人群调查**。
- 关键结果：
  - MEWS 为**单维**，在**性别、年龄、ADHD 状态间测量等价（invariant）**。
  - 在**有 ADHD 的人群中，未发现心智游走的性别差异**；在**无 ADHD 人群中，男性分数更高。**
  - **「在有 ADHD 的男女之间，多动/冲动、情绪不稳与功能损害水平相似；但男性自评注意力不集中更多、幸福感更低。」**
- 作者结论：MEWS 可辅助**诊断与监测**。

> ⚠️ **这条结果对 Littman 框架是一个部分反证**：如果女性 ADHD 的核心是「内在多动/思维乱窜」，那么在**已经诊断出来的 ADHD 人群中**，女性应当表现出更高的心智游走 —— **但实测没有**。可能的解释：(a) 选择偏倚（能被诊断出来的女性本来就是症状更重的）；(b) 工具未捕捉 Littman 所指的具体现象；(c) 「内在多动」不是女性专属。**Skill 里应把这个张力明确写出，不要抹平。**

> **另一条相关**：`"Attention-Deficit/Hyperactivity Disorder Symptom Dimensions Differentially Predict Adolescent Peer Problems: Findings From Two Longitudinal Studies."` *Frontiers in Psychology* 2020;11:609789. PMID **33584444**。【仅摘要】—— BGALS（N=228）与挪威人群样本（N=3,467，53% 女孩）平行设计。⚠️ 具体性别分层结果本次未提取。

---

## 2.7 本文件的「总纲」来源

> **Salehpour F, Gonzalez-Lima F. "Sex Bias in the Clinical Diagnosis of ADHD: A Critical Review."** *Journal of Clinical Medicine* 2026;15(17):6804. DOI **10.3390/jcm15176804** · PMID **42739808** · **PMCID PMC13566458** · 【**OA 全文已获取**】· 可信度：高（**但作者自陈：critical narrative review，未按 PRISMA 执行，未做定量合成，未做标准化偏倚风险评估**；且作者声明使用 ChatGPT-5 作为写作与编辑辅助工具）

**本 Skill 引用的它来支撑的五条关键定量陈述（均来自其 §1 / §3 原文）：**
1. 临床转介儿童样本 **≈ 4:1**；社区样本 **2.4:1–3.2:1**；瑞典双胞胎 **临床 2.5:1 vs 人群 1.8:1**（**该比值系该综述对参考文献 [3]=Mowlem 2021… 即 PMID 30097723 的转引，非 Mowlem 摘要原文**）。
2. DSM-IV 现场试验 **21% 女性**；DSM-5 儿科 **≈40% 女性**，成人 **48%**。
3. 信息源与男:女比：**双报告一致 5.3:1 > 仅教师 3.3:1 > 仅家长 2.5:1**。
4. 课堂「被惹恼」比例：**女孩 38% vs 男孩 64%**；临床转介样本中家长为女孩勾选的注意缺陷条目数「约为男孩的一半」。
   ⚠️ **3、4 以及第 1 条中的 Mowlem 2.5:1／1.8:1 均为该综述对其参考文献的转引**，**原始文献本次未获取**。
   - 第 3 条对应的参考文献为 **[60] = Gomez R et al., *J Child Psychol Psychiatry* 1999;40(2):265-274, PMID 10188709（澳洲小学儿童）**；第 4 条课堂比例对应 **[56]**；第 1 条 Mowlem 比值对应 **[3] = PMID 30097723**。

**该综述作者自己列出的方法学限制（Skill 引用其结论时必须一并引用）：**
- 「相对较少有研究专门优先考察 ADHD 中的性别差异，且**报告的差异总体上幅度适中（modest in magnitude）**。」
- 「文献多为观察性、且常为横断面，**限制了关于所报告的性别差异究竟反映诊断偏倚、潜在表型差异、还是两者的因果结论**。」
- 「**可能存在发表偏倚** —— 报告显著性别差异的研究更可能被发表，这可能导致**部分效应被高估**。」
- 「**重要的是，这些生物学与发育因素本身并不是诊断偏倚的来源**；它们可能塑造出与诊断期待、识别与评估实践相互作用的 ADHD 表型。」← **这一句极为重要：Skill 不应把激素机制当作漏诊的原因，它只塑造表型，漏诊是社会过程。**

---

## 2.8 本文件来源清单（28 项）

| # | 来源 | 类型 | 本文件用途 |
|---|---|---|---|
| 1 | Mowlem FD 等 2019, Eur Child Adolesc Psychiatry 2019;28(4):481-489, PMID 30097723 | 同行评议/仅摘要 | §1.1 核心 |
| 2 | Mowlem F 等 2019, Psychiatry Research 2019;272:765-773, PMID 30832197 | 同行评议/仅摘要 | §1.1、§2.1 |
| 3 | 威尔士登记 JCPP 2024, PMID 38864317 | 同行评议/仅摘要 | §1.2.1、§1.3、§2.1、§2.5.1 |
| 4 | 台湾 Psychiatry Research 2020, PMID 31981938 | 同行评议/仅摘要 | §1.2.2、§2.4.3 |
| 5 | 丹麦 Acta Psychiatr Scand 2026, PMID 42011750 | 同行评议/仅摘要 | §1.2.3 |
| 6 | 澳洲 NSW J Atten Disord 2026, PMID 42541370 | 同行评议/仅摘要 | §1.2.4 |
| 7 | 新西兰 J Atten Disord 2026, PMID 42560122 | 同行评议/仅摘要 | §1.2.5 |
| 8 | 苏格兰 Autism 2026, PMID 41157911 | 同行评议/仅摘要 | §1.2.6 |
| 9 | 荷兰双胞胎 Twin Res Hum Genet 2007;10(5):765-770, PMID 17903118 | 同行评议/仅摘要 | §1.2.7、§2.1 |
| 10 | Clin Psychol Sci 2026, PMID 42719335 | 同行评议/仅摘要 | §1.2.8（反面证据） |
| 11 | Biederman J 等 2002, Am J Psychiatry 2002;159(1):36-42, PMID 11772687 | 同行评议/仅摘要 | §1.3（10:1 vs 3:1 原始出处） |
| 12 | Danielson 2024, JCCAP, PMID 38778436 | 同行评议/仅摘要 | §1.3（美国最新 NSCH） |
| 13 | 伊朗德黑兰 J Atten Disord 2021;25(8):1058-1067, PMID 31833803 | 同行评议/仅摘要 | §1.3（结构化访谈口径） |
| 14 | 伊朗 meta 分析, PMID 40810952 | 同行评议综述/仅摘要 | §1.3 |
| 15 | 埃及 Fayoum, PMID 25814429 | 同行评议/仅摘要 | §1.3（异常高值） |
| 16 | 印度 Belagavi, PMID 29929414 | 同行评议/仅摘要 | §1.3（反向小样本） |
| 17 | EPINED 西班牙, PMID 38695661 | 同行评议/仅摘要 | §1.3 |
| 18 | Willcutt 2012, Neurotherapeutics 2012;9(3):490-499, PMID 22976615 | 同行评议/仅摘要 | §1.4 核实 |
| 19 | Polanczyk GV 等 2014, Int J Epidemiol 2014;43(2):434-442, PMID 24464188（第一作者非 Willcutt） | 同行评议/仅摘要 | §1.4 |
| 20 | Salehpour & Gonzalez-Lima 2026, J Clin Med 2026;15(17):6804, PMC13566458 | 同行评议综述/**OA全文** | §2 全节 |
| 21 | Biederman J 等 2008, JAACAP 2008;47(4):426-434, PMID 18388760 | 同行评议/仅摘要 | §2.1、§2.5.1 |
| 22 | Front Hum Neurosci 2019;13:441, PMID 31920599 | 同行评议/仅摘要 | §2.3.1 |
| 23 | Indian J Psychiatry 2025, PMID 40043536 | 同行评议/仅摘要 | §2.1 |
| 24 | Int J Clin Health Psychol 2026, PMID 41551064 | 同行评议/仅摘要 | §2.1 Step 5 |
| 25 | Front Psychiatry 2026（高功能高痛苦）, PMID 42232996 | 立场论文/仅摘要 | §2.2.2 |
| 26 | J Atten Disord 2024（定性 NSSDV）, PMID 38294171, PMC11168017 | 同行评议/**OA全文** | §2.2.3 |
| 27 | Front Psychol 2026（stigma & masking 综述）, PMID 41987980 | 叙述性综述/仅摘要 | §2.2.5 |
| 28 | Sci Rep 2019;9(1):3071（MEWS）, PMID 30816143 | 同行评议/仅摘要 | §2.6 |

**此外引用但未单列的辅助条目**：Front Psychiatry 2025（masking/诊断接受度，PMID 41169493）、Behav Sci 2026（冒名顶替与 social camouflaging，PMID 41750022）、Front Global Womens Health 2025（DIVA-5，PMID 40182228）、J Psychiatr Pract 2014（ADHD vs 双相，PMID 25406047）、Front Psychiatry 2026（ADHD/BPD 症状重叠，PMID 42445552）、Int Clin Psychopharmacol 2026（ADHD+BPD 哌甲酯，PMID 42127382）、BMC Psychiatry 2023（人格障碍发展预测，PMID 36793031）、Front Psychol 2020（BGALS + 挪威双队列同伴问题，PMID 33584444）。