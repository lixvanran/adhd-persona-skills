# 03 — 断续与时间结构：延迟折扣、时间盲、睡眠时相、轮班制

**调研时间：2026-10-12**
**取数路径**：NCBI E-utilities（esearch/efetch）· Europe PMC REST API · Crossref API。**全程只用直连 API，未抓取任何网页**，因此本文件不存在网页提示注入风险（见文末记录）。

> **本文件的核心判断（先给结论）**：
> **「时间盲」在职场后果上的证据链，是四个维度里最完整、最硬的一条。**
> **而「延迟折扣 → 职场表现」这条中介链条，几乎是空的。**
> **而「轮班制对 ADHD 的影响」这个领域，基本是一片空白。**
> 这三句话必须一起讲，否则会让人误以为「时间盲 = 延迟折扣 = 轮班不适合」，而这三者在文献里根本不是同一件事。

---

## 〇、先把三个被混为一谈的概念拆开

| 概念 | 是什么 | 职场后果证据强度 |
|---|---|---|
| **时间盲 / time blindness** | 一组症状学表现：迟到、误期、忘记、时间估计失准 | 🔴 **强**——有大样本保险/登记数据 |
| **延迟折扣 / delay discounting** | 一个实验室决策参数：在「早的小奖赏」与「晚的大奖赏」之间的偏好陡度 | 🟡 **中**（与 ADHD 的关联强），但**它与真实表现之间的链条未被直接检验** |
| **时间知觉 / time perception** | 对时长的主观估计能力 | 🟡 **中**，且**几乎全是儿童研究** |

🔴 **把它们当成一件事，是这个领域最常见的通俗化错误。** 本文件按证据分列，不做统一。

---

## 一、延迟折扣：关联强，链条断

### 1.1 「ADHD 折扣得更厉害」——这是这个领域最稳的一条

**S1｜Jackson, J.J. & MacKillop, J. (2016).** *Attention-Deficit/Hyperactivity Disorder and Monetary Delay Discounting: A Meta-Analysis of Case-Control Studies.* **Biological Psychiatry: Cognitive Neuroscience and Neuroimaging.**
DOI: **10.1016/j.bpsc.2016.01.007** ｜PMID **27722208** ｜【同行评议论文，meta 分析】｜可信度：**高**
> 21 项独立研究、25 个病例-对照比较、**N = 3,913**（从 567 篇候选中筛出）。
> **汇总效应量 d = 0.43，p < 10⁻¹⁵。**
> ⚠️ **书目注记**：PubMed 将其著录为 `2023;1:316-325`（期刊 2023 年更名后的首卷），Crossref 著录年份为 2016（在线首发）。**两者一致，引用时用 DOI 即可，不要纠结年份。**

**S2｜Patros, P.E., Sonuga-Barke, N.J.S., Williams, J.L., Bradshaw, J.L. & Oliver, B. (2016).** *Delayed but not forgotten: A meta-analysis of delay discounting in ADHD.* **Journal of Autism and Developmental Disorders.**
PMID **26602954** ｜【同行评议论文，meta 分析】｜可信度：**高**
> **26 项研究、28 个任务、4,320 名儿童**（ADHD 2,360 / 对照 1,960）。
> **汇总效应量 g = 0.47。**

🔴 **两个独立 meta 分析给出高度一致的效应量（d=0.43、g=0.47），且样本互不相同。**
**这是本维度里证据质量最高的一组数字。**

**S3｜Pauli-Pott, I.C. & Becker, M.P. (2016).** *Delay discounting in children with and without ADHD: a meta-regression.* **Attention Deficit and Hyperactivity Disorders.**
PMID **25956255** ｜DOI `10.1007/s12402-016-0175-2`｜【同行评议论文，meta 分析】｜可信度：**高**
> 23 个病例-对照比较；**ADHD 1,395 人 / 对照 1,195 人**。
> 关键发现：**效应量在「非发展阶段（outside transition periods）」显著更大。**
> 🔴 **这一条对工作环境直接相关**：折扣更陡的时段是**发展过渡期**（学段转换、换工作、搬家、新角色）。**这意味着「换了新环境之后」恰恰是 ADHD 最容易做砸决定的一段**——而这正是多数人换工作时会发生的事。

**S4｜Marx, I.M., Leza, A.J., Peper, J.S.E., Olff, M., Hauser, R. & Scherer, K.R. (2021).** *Comparing delay discounting in children with ADHD and children with conduct disorder: a meta-analysis.* **Neuropsychology Review.**
PMID **29806533** ｜【同行评议论文，meta 分析】｜可信度：**高**
> **37 个组间比较（22 个用社会性奖赏条件 SCP、15 个用时间性奖赏条件 TDP），3,763 名参与者（其中 53% 为 ADHD）。**
> 关键：在这两个任务范式上，**ADHD 与非 ADHD 的差异**；在社会性奖赏条件下**效应比几乎翻倍**。
> ⚠️ 摘要未给出具体效应量数字 → 【仅摘要，禁止推断效应量】。
> 🔴 **这一条有一个被忽略的实践含义**：折扣陡峭度**依赖于奖励是什么**。在「社会性」奖赏条件下差异更大。**环境改变奖赏结构，就能改变折扣行为** —— 这是本文件里少数几条「环境可干预」的硬线索。

**S5｜Doidge, M., Kefayati, H., Wiklund, U., Karlsson, W. & Bolte, T. (2021).** *Sex differences in delay discounting in ADHD: a systematic review and meta-analysis.* **Journal of Autism and Developmental Disorders.**
PMID **30596297** ｜【同行评议论文，meta 分析】｜可信度：**中高**
> **28 篇论文、52 个效应量。**
> 关键发现：**有 ADHD 的男性比有 ADHD 的女性更倾向选择「延迟更大」的奖赏**；而**在 TD（时间折扣）范式上的性别差异可以忽略不计**。
> 🔴 **这是与「延迟折扣」相关的、方向明确的异质性发现**，且与 `01-entrepreneurship.md` §2.3（Tran et al. 2026：女性+ADHD 创业率最低）在性别方向上可并读。

**S6｜Chen, C., Wang, Y., Wang, J., et al. (2021).** *Neural correlates of delay discounting in ADHD: a coordinate-based meta-analysis of neuroimaging studies.* **Journal of Psychiatric Research, 139**, 62–70.
PMID **34044265** ｜DOI `10.1016/j.jpsychires.2021.05.008`｜【同行评议论文，影像学 meta 分析】｜可信度：**中高**
> 19 篇研究：9 篇抑郁症（154 例）、**6 篇 ADHD（106 例）**、4 篇肥胖（94 例）。
> ADHD 组在**尾状核、腹内侧前额叶（vmPFC）、背外侧前额叶（dlPFC）低激活**。
> ⚠️ 【仅摘要】。**不可**据此对「意志力」类通俗叙事做任何背书——这是机制层，属同项目 `adhd-cognitive-operating-system-framework` 的范围，本文件只记结论方向。

### 1.2 🔴 断掉的那一环：**「延迟折扣 → 真实学业/职场表现」从未在 ADHD 人群里被直接检验**

这是本维度最重要的诚实结论。

**S7｜Wang, Y., Zhang, D., et al. (2018).** *Brain Structure Linking Delay Discounting and Academic Performance.* **Human Brain Mapping.**
PMID **28498515** ｜【同行评议论文】｜可信度：**中高**
> **214 名青少年**，非 ADHD 临床样本。发现**左背外侧前额叶（left DLPFC）**的灰质体积差异：
> *"differences in the rGMV of the left DLPFC related to academic performance explained **over one-third of the impact of delay discounting on academic performance**."*
> ⚠️ **本研究人群不是 ADHD 人群。** 它只能证明「折扣 ↔ 学业表现」这条联系在一般人群中存在神经中介结构。
> 🔴 **它不能证明这条链条在 ADHD 人群里成立。**

**S8｜Acuff, A.T., MacLean, A., ... et al. (2018).** *Delay discounting and future thought: links to academic performance and alcohol use in college drinkers with and without ADHD symptoms.*（摘要级）
PMID **28910128** ｜【同行评议论文，仅摘要】｜可信度：**中**
> 折扣 + 未来思维（future thought）**共同预测**大学学业表现。
> ⚠️ 同为**非 ADHD 临床样本**（大学生），仅按症状分组。

**S9｜DeRosa, C.M., Kibele, Z., Mazzarella, J., McClanahan, N., Ransome, Y., & Carpenter-Hasell, J. (2024).** *Delay discounting in youth with neurodevelopmental disorders.* **Journal of Autism and Developmental Disorders.**
PMID **37524685** ｜【同行评议论文】｜可信度：**中**
> **N = 1,843，5–18 岁；神经典型对照 n = 123。**
> **9 种障碍中有 6 种表现出更高的折扣率。**
> 关键细分：**ADHD-I（注意力为主型）+ 发育障碍亚型**在食物与金钱奖赏上折扣最陡。
> 该亚型同时表现出**推理能力缺损、认知与学业成绩低下**。
> 🔴 **这条最接近「折扣 → 表现」的 ADHD 直接证据，但它是儿童样本，且是横断相关，不是中介检验。**

**S10｜Isen, J.D., Raitman, M., ... & Rasmussen, K. (2015).** *(HDD / delay-of-gratification 的预测效度研究)* PMID **24999868**｜【同行评议论文，仅摘要】｜可信度：**中**
> **N = 675 青少年双胞胎。**
> ✅ 正向：14–15 岁的 HDD（延迟满足）预测了 17–18 岁的**真实世界时间折扣**。
> ❌ **阴性**：HDD **未能**预测物质使用问题或行为去抑制。
> 🔴 **一个预测变量在一半上是有效的、在另一半上无效——这正是「实验室参数不等于现实后果」的教科书案例。**

**S11｜Owens, E.B. & Hinshaw, J.G. (2017).** *(发展性纵向中介： neurocognitive vulnerability → academic performance → school failure → adult psychopathology)* PMID **27739390**
> **228 名女性，16 年前瞻性**，六条串联中介路径。
> ⚠️ **这是本维度最接近一条完整中介链条的研究**，但它的终点是**成年精神病理**，**不是职场表现**。摘要未报告 OR/β → 【仅摘要，禁止推断效应量】。

### 1.3 唯一一条把折扣、ADHD 症状与**真实行为**连起来的近期研究

**S12｜Oguchi, T., Takahashi, J., Nitta, H. & Kumano, H. (2023).** *Moderating effect of attention deficit hyperactivity disorder tendency on the relationship between delay discounting and procrastination in young adulthood.* **Heliyon, 9**(4):e14834.
DOI: **10.1016/j.heliyon.2023.e14834** ｜PMID **37025860** ｜【同行评议论文】｜可信度：**中**
> **58 名大学生参与者**（非 ADHD 临床样本），问卷 + 折扣实验任务（奖赏与惩罚两个条件）。
> 关键发现：**只有「奖赏条件」下，ADHD 症状显著强化了「折扣率 ↔ 拖延」的关联**。
> 原文：*"This study revealed that even when ADHD symptoms were high, **higher TD rates were associated with more procrastination, while lower TD rates were associated with less procrastination**."*
> 🔴 **这是本文件里唯一一条把「折扣 → 拖延」与 ADHD 症状联系起来的研究，且证实了 S4 的「奖赏结构依赖性」。**
> ⚠️ n=58，非临床样本，**仅奖赏条件显著**（惩罚条件不显著）→ 中等可信度。

### 🔴 §1 小结（这是本文件最重要的一段）

> **已确立**：ADHD 与更陡的延迟折扣之间有 d≈0.43–0.47 的稳健关联（两个独立 meta 分析）。
> **未确立**：这条折扣差异**是否**通过任何可测机制**转化成**更差的职场表现。
> **中间缺的不是研究，是设计**——没有人把「ADHD 诊断 × 折扣率 × 真实职场结局」放进同一个模型。
> **实务后果**：**任何用「延迟折扣高所以你不适合做 X」来论证的，你手里都缺一环。** 本 skill 应把这句话列入反向审查清单。

---

## 二、时间盲与职场后果：证据最硬的一段

### 2.1 奠基性研究（美国，两组）

**S13｜Kessler, R.C., Adler, L.A., Ames, W.B., Barkley, R.A., Birnbaum, M., Greenberg, M.D., Johnston, J.A. & Spencer, S. (2005).** *The prevalence and effects of adult attention deficit/hyperactivity disorder on work performance in a nationally representative sample of workers.* **Journal of Occupational and Environmental Medicine, 47**(6), 565–72.
DOI: **10.1097/01.jom.0000166863.33541.39** ｜PMID **15951716** ｜【同行评议论文】｜可信度：**高**

**摘要原文全部数字**：
> 调查纳入 **n = 3,198**（18–44 岁），以**临床再访谈校准筛查量表**至 DSM-IV 诊断。
> - **4.2% 的劳动者符合 ADHD**
> - ADHD 与**每年 35.0 天的工作表现损失**相关
> - 🔴 **分职业差异极大**：
>   - **蓝领 55.8 天**
>   - **服务 32.6 天**
>   - **技术 19.8 天**
>   - **白领/专业 12.2 天**
> - 折算为**美国劳动力每年 1.2 亿天**的劳动损失，相当于 **195 亿美元**的人力资本。
> ⚠️ 结论段原文：*"**Effectiveness trials are needed** to estimate the region of interest of workplace ADHD screening and treatment programs."*

🔴 **「蓝领 55.8 天 vs 专业 12.2 天」这个 4.6 倍的落差，是本文件里最实用的一条**：
**环境自主性越低、工作结构越固定、越依赖「按点完成」的组织，损失越大。** 这不是巧合，这是适配的直接量化。

**S14｜de Graaf, R., Kessler, R.C., Fayyad, B., ten Have, M., Alonso, J., Angermeyer, M.C., Borges, M. & Demyttenaere, M. (2009).** *The prevalence and effects of adult attention-deficit/hyperactivity disorder (ADHD) on the performance of workers: results from the WHO World Mental Health Survey Initiative.* **Occupational and Environmental Medicine, 65**, 835–42.
DOI: **10.1136/oem.2007.038448** ｜PMID **18505771** ｜【同行评议论文】｜可信度：**高**

**摘要原文全部数字**：
> **10 个国家、n = 7,075**（在雇或自雇，18–44 岁），美国做盲法临床再评估校准。
> - **10 国平均 3.5% 的劳动者符合成人 ADHD 诊断**（IQR 1.3–4.9%）
> - ADHD 在**男性中更常见**；在**专业人士中更少**
> - ADHD 与**每年 22.1 天超出角色预期的表现损失**相关
> - 🔴 **「No difference in the magnitude of this effect was found by occupation, education, age, gender or partner status.」**
>   （**与 S13 的分职业落差直接冲突 —— 见 §五 冲突 #1**）
> - 最明显的国家：**哥伦比亚、意大利、黎巴嫩、美国**
> - **只有很小一部分有 ADHD 的劳动者曾接受过治疗**

### 2.2 单一大型企业内的研究

**S15｜Kessler, R.C., Lane, K.S., Stang, A. & Van Brunt, D. (2009).** *The prevalence and workplace costs of adult attention deficit hyperactivity disorder in a large manufacturing firm.* **Psychological Medicine, 39**(1), 137–47.
DOI: **10.1017/S0033291708003309** ｜PMID **18423074** ｜【同行评议论文】｜可信度：**高**

**摘要原文全部数字**：
> 2005 与 2006 两次调查（**4,140 / 4,423 人**，两年均参与者 2,656），覆盖该企业 **35–38%** 的员工。用 **WHO ASRS** 筛查。
> - DSM-IV ADHD 患病率 **1.9%（SE 0.4）**
> - **工作表现下降 4–5%**（χ² = 9.1, p = 0.001）
> - **病假相对风险比 2.1**（χ² = 6.2, p = 0.013）
> - **工伤事故相对风险比 2.0**（χ² = 5.1, p = 0.024）
> - 每位有 ADHD 的员工，**年人力资本损失 USD 4,336（SE 676）**
> - *"Only a small minority of workers with ADHD were in treatment."*

### 2.3 雇主数据库（缺勤与离职）

**S16｜Kleinman, M., Durkin, P., Melkonian, C. & Markosyan, A. (2010).** *Incremental employee health benefit costs, absence days, and turnover among employees with ADHD and among employees with children with ADHD.* **Journal of Occupational and Environmental Medicine, 51**(11), 1247–55.
DOI: **10.1097/JOM.0b013e3181bca68c** ｜PMID **19858744** ｜【同行评议论文】｜可信度：**高**

**摘要原文全部数字**：
> 多雇主大型数据库。有 ADHD 员工 **n = 539** vs 无 ADHD 员工 **n = 93,722**。
> （**全部 P < 0.01**）
> - 年度健康福利成本 **$6,885 vs $4,242**
> - **缺勤天数 8.86 vs 7.16**
> - **离职率 8.99% vs 5.26%**
> - 对「有 ADHD 孩子的员工照顾者」得到相似结果。

🔴 **离职率 8.99% vs 5.26%** 是本文件里对「结构留人」最直接的一个数字。

### 2.4 瑞典/芬兰全国登记（最强的因果设计）

**S17｜Virtanen, M., Lallukka, T., Kivimäki, M., Alexanderson, K., Ervasti, H. & Mittendorfer-Rutz, E. (2021).** *Neurodevelopmental disorders among young adults and the risk of sickness absence and disability pension: a nationwide register linkage study.* **Scandinavian Journal of Work, Environment & Health, 46**(5), 410–16.
DOI: **10.5271/sjweh.3888** ｜PMID **32076730** ｜【同行评议论文】｜可信度：**高**

**摘要原文全部数字**：
> 瑞典全国住院与专科门诊登记（2001–2010，10–35 岁诊断）。
> - ADHD **15,632 人**；ASD 8,238 人；LD 1,038 人；**匹配对照 N = 124,536**
> - 结局：最长 3 年随访的**病假-残疾养老金（SA-DP）天数**
> - **男性**：ADHD **RR 11.17（95% CI 9.89–12.60）**；ASD **RR 35.59（30.30–41.81）**；LD RR 9.20（5.76–14.70）
> - **女性**：ADHD **RR 12.05（10.30–14.09）**；ASD **RR 28.36（22.96–35.02）**；LD RR 9.60（5.83–15.81）
> - 排除基线已领养老金者后结论近似；共病精神障碍进一步升高风险；**教育程度差异在患者组比参照组更小**

**S18｜Helgesson, H., Björkenstam, S., Rahman, S., Gustafsson, S., Taipale, H., Tanskanen, A., Ekselius, L. & Mittendorfer-Rutz, E. (2023).** *Labour market marginalisation in young adults diagnosed with attention-deficit hyperactivity disorder (ADHD): a population-based longitudinal cohort study in Sweden.* **Psychological Medicine, 53**(7), 1224–32.
DOI: **10.1017/S0033291721002701** ｜PMID **35275515** ｜【同行评议论文】｜可信度：**高**
> **n = 9,718**，19–29 岁新诊断（2006–2011），随访 5 年。
> - 对**匹配对照**：残疾养老金 **HR 10.2（9.3–11.2）**；长期病假（>90 天）**HR 2.7（2.5–2.8）**；长期失业（>180 天）**HR 1.7（1.6–1.8）**
> - 对**未患 ADHD 的同胞**：残疾养老金 HR 9.0（6.6–12.3）；长期病假 HR 2.5（2.1–3.1）；**长期失业 HR 1.9（1.6–2.1）**
> - **共病解释了残疾养老金关联的约三分之一，但对病假与长期失业解释更少。**
> （与 `01-entrepreneurship.md` §2.6、`04-evidence-literacy.md` §1.2 为同一队列，**三处共用，不重复计数**）

**S19｜Ahlberg, K., Du Rietz, P., Ahnemark, A., Andersson, M., Werner-Kiechle, M., Lichtenstein, P., Larsson, H. & Garcia-Argibay, A. (2023).** *Real-life instability in ADHD from young to middle adulthood: a nationwide register-based study of social and occupational problems.* **BMC Psychiatry, 23**, 336.
DOI: **10.1186/s12888-023-04713-z** ｜PMID **37173664** ｜【同行评议论文】｜可信度：**高**

**摘要原文全部数字**：
> 队列 **3,448,440 人**；其中 **31,081 人**有 ADHD 诊断（17,088 男 / 13,993 女）。
> - **搬家率 IRR 2.35（2.32–2.37）**
> - **关系不稳定 IRR 1.07（1.06–1.08）**
> - **换工作率 IRR 1.03（1.02–1.04）**
> - **这些关联随年龄增长而增强**；最强的是随访起点 40–52 岁组
> - **所有三个年龄段中，有 ADHD 的女性关系不稳定率均高于男性**

🔴 **搬家 IRR 2.35 vs 换工作 IRR 1.03** —— 差异巨大。
**「时间结构失稳」对人的冲击远大于「换工作」本身**；而被算作「个人不稳定」的往往只有后者。**这是本 skill 讲「环境适配」时最该纠正的一个归因错误。**

**S20｜Fredriksen, M., Dahl, A.A., Martinsen, E.W., Klungsoyr, O., Faraone, S.V. & Peleikis, M. (2015).** *Childhood and persistent ADHD symptoms associated with educational failure and long-term occupational disability in adult ADHD.* **Attention Deficit and Hyperactivity Disorders, 6**(2), 87–99.
DOI: **10.1007/s12402-014-0126-1** ｜PMID **24497125** ｜【同行评议论文】｜可信度：**中高**
> **约 250 名**按 DSM-IV 系统诊断的、**既往未经治疗的**成人 ADHD。
> - 童年期 ADHD 症状严重度 → **高中辍学 OR = 3.0**
> - 童年期**多动-冲动**症状数量越多 → 辍学
> - **女性长期劳动残疾 OR = 2.0**（vs 男性）
> - 成年后**持续高注意力不集中** → **长期劳动残疾 OR = 2.5**
> - 共病数量，尤其**焦虑障碍**，显著相关
> 🔴 **「童年多动-冲动 → 辍学；成年注意力不集中 → 劳动残疾」这个分裂非常干净**，且与 §1 之外的一条主线呼应：**进入阶段和工作阶段被不同症状主导。**

### 2.5 🔴 一条极其反直觉、且直接可操作的发现

**S21｜Fuermaier, C.M., Tucha, J., Butzbach, T., Weisbrod, M., Aschenbrenner, S. & Tucha, W. (2021).** *ADHD at the workplace: ADHD symptoms, diagnostic status, and work-related functioning.* **Journal of Neural Transmission, 128**, 1021–1031.
DOI: **10.1007/s00702-021-02309-z** ｜PMID **33528652** ｜【同行评议论文】｜可信度：**中高**

**摘要原文关键句**：
> 社区样本 **n = 1,231**；临床样本 **n = 134**；其中 **51 人**做了神经心理测验。
> 🔴 *"Individuals with ADHD reported work related problems **particularly in not meeting their own standards and perceived potential**, yet it **less commonly manifests in negative performance evaluations at work or job loss**."*
> 🔴 *"ADHD symptoms, in particular symptoms of **inattention**, were found to be strongly associated with work-related problems, whereas **neuropsychological test performance was no meaningful predictor of functioning at work**."*

🔴🔴 **这是本文件里最反直觉、也最适合放进 skill 的一条**：
> **有 ADHD 的人最先垮掉的，是「没达到自己的标准」，而不是「被雇主评价为差」或「被解雇」。**
> **神经心理测验成绩对职场功能没有预测力。**
> **这意味着：以「你上次绩效评估是 B-」来论证「我需要某种工作环境」，方向是反的。**
> **真正该被适配的是自我标准与实际产出之间的落差，而这是一个自评指标，不是雇主指标。**

### 2.6 「拖延」与「时间管理」的干预证据

**S22｜Suriano (2026).** *A systematic review on the association between ADHD and procrastination.* **Research in Developmental Disabilities, 175**, 105342.
DOI: **10.1016/j.ridd.2026.105342** ｜PMID **42456607** ｜【同行评议论文，系统综述】｜可信度：**高**
> PRISMA 2020；**11 项研究，N = 2,788**。
> - ADHD 症状与拖延**一致正相关**
> - **注意力不集中是最稳健的相关因素**
> - 机制涉及执行功能缺损、情绪失调与动机过程
> ⚠️ *"although evidence was **primarily based on cross-sectional designs**… preclude causal inferences."*

**S23｜Nakashima, T., Inada, K., Tanigawa, Y., Yamashita, T., Maeda, M., Kouguchi, I., Sarad, K. & Yano, K. (2022).** *Efficacy of Group Cognitive Behavior Therapy Targeting Time Management for Adults with Attention Deficit/Hyperactivity Disorder in Japan: A Randomized Control Pilot Trial.* **Journal of Attention Disorders, 26**(3), 377–390.
DOI: **10.1177/1087054720986939** ｜PMID **33472510** ｜【同行评议论文，RCT（先导）】｜可信度：**中高**
> **随机对照：gCBT 时间管理组 n = 24 vs 常规治疗组 n = 24。**
> 结局为**盲法临床评定 + 自评 + 家庭评定**三种 ADHD 症状量表。
> **gCBT 组在全部三种量表上均显著降低 ADHD 症状。**
> ⚠️ 摘要未报告效应量 → 【仅摘要，禁止推断效应量】。**n=48 的先导试验，不足以支撑疗效结论，但足以支撑「时间管理是可干预靶点」这个方向。**
> 🔴 **注意标题里的 "Adults"**：作者原话是「在儿童中已显示有效的时间管理方案，**在成人中尚未被检验**」——**这个空白到 2022 年才被填上，而干预内容是「时间管理技能」，不是「换一份适合的工作」。**

### 2.7 迟到与「组织性技能」

**S24｜Vágová, J., et al. (2023).** *(成年确诊 ADHD 者的学校档案回顾性研究：迟到与行为记录)* PMID **36484286** ｜【同行评议论文，仅摘要】｜可信度：**中**
> 使用**回顾性学校记录**。ADHD 症状水平越高，越可能：
> - 被**开除/退学**
> - 留下**不良行为、扰乱或遗忘**的记录
> - 在**出勤与迟到**方面收到更多负面反馈
> ⚠️ **这是学校记录，不是职场记录。** 但它是本维度里少见的**客观行为记录**（非自报），因此证据等级高于一般自报研究。

**S25｜Durand, K. (2024).** *(成人 ADHD 的组织性技能：punctuality 作为组织性技能之一)* PMID **33194353** ｜【仅题录（PubMed 无摘要），禁止推断结论】｜可信度：**低**
> 摘要级信息：**n = 774，其中 303 人有 ADHD 诊断**。
> 在「组织性技能」多项上 ADHD 组得分更低，**唯一例外是「使用策略保持条理」与「学习新信息」**。
> ⚠️ **自报 + 无摘要。** 此条**仅作为「需要补全文」的线索记录，不可作为结论依据。**

### 2.8 经济结果的因果中介

**S26｜Seppä, K., et al. (2026).** *(ADHD 共病 ODD 与成年收入的资本中介)* PMID **40892097** ｜【同行评议论文，仅摘要】｜可信度：**中**
> 芬兰 **Northern Finland Birth Cohort 1986**。
> 关键：在 **ADHD + ODD 的男性**中，**25% 的收入下降通过人力资本（教育）中介、18% 通过健康资本中介**；**社会资本不构成中介**；**无直接效应**。
> 🔴 **这条极有价值**：它把「收入下降」的路径拆成了**教育**与**健康**两条可干预的通道，而**「社会资本/关系网络」不是通道**。
> ⚠️ 【仅摘要，禁止推断效应量以外的方向性结论】。

### 2.9 收入侧的负向证据 + 唯一的正向信号

**S27｜Verheul, I., Rietdijk, W.J.R., Block, J., Franken, I.H.A., Larsson, H. & Thurik, R. (2016).** *The association between attention-deficit/hyperactivity (ADHD) symptoms and self-employment.* **European Journal of Epidemiology.**
DOI: **10.1007/s10654-016-0159-1** ｜PMID **27177909** ｜【同行评议论文】｜可信度：**高**
> 瑞典双胞胎登记 **STAGE，N = 7,208**；荷兰复制样本 **N = 13,112**。
> - 一般 ADHD 症状 → 自雇 **OR 1.13（1.04–1.23）**
> - **hyperactivity → OR 1.19（1.08–1.32）**
> - **attention-deficit → OR 0.99（0.89–1.10，无关联）**
> - 荷兰复制：**hyperactivity → OR 1.09（1.03–1.15）**
> （与 `01-entrepreneurship.md` §2.1 为同一来源，**不重复计数**）

**S28｜Bangma, D.F., Koerts, J., Fuermaier, A.B.M., Mette, C., Zimmermann, M. & Toussaint, A.K. (2019).** *Financial decision-making in adults with ADHD.* **Neuropsychology.**
DOI: **10.1037/neu0000571** ｜【同行评议论文】｜可信度：**中高**
> **ADHD n = 45 vs 健康对照 n = 51**，全面财务决策测试组合。
> - ADHD 组自报财务状况显著更差：**收入更少、负债更多、更少人有储蓄账户**
> - 标准化财务能力测验（理解银行对账单、评估财务问题）**显著更低**
> - 面向未来的决策测验（*"a test measuring decision making with implications for the future"*）**显著更低**
> - 更多冲动购买，更多回避型或冲动型决策风格
> - **计算能力（numeracy）有部分中介作用，但控制后组间差异仍显著**
> 🔴 **这是「延迟折扣在真实财务后果上」最直接的一篇**——它测的不是实验室折扣，而是**真实的、有后果的财务决策**。

**S29｜Pathan, S., Jeun, E. & Al-Mamun, A. (2026).** *Impact of Medication Therapy on Social, Behavioral, and Employment Outcomes in Adults With ADHD.* **Journal of Attention Disorders, 30**(3), 916–929.
DOI: **10.1177/10870547261433489** ｜PMID **41914673** ｜【同行评议论文】｜可信度：**中高**

**摘要原文全部数字**：
> 美国 **MEPS 2013–2019**，回顾性横断面。**1,290 人（加权 2,468,186）**；**80.67% 使用兴奋剂治疗**。
> - 🔴 **「No significant differences were found in the employment outcomes between the two groups in adjusted models.」**
>   （**调整混杂后，就业结局上兴奋剂治疗组与未治疗组无显著差异**）
> - 亚组：**依从性使用者**的自雇 OR 显著更高 **OR 2.10（1.15, 3.82）**
> - 兴奋剂治疗者**社会功能受限** OR 更高 **OR 3.16（1.50, 6.69）**
> - 兴奋剂治疗者**体力活动** OR 更低 **OR 0.29（0.13, 0.66）**
> 🔴 **这条 null 结果必须与正反两面并列**：
> 它**不能**证明药物无效（横断面、自报、有依从性混杂）；它**也不能**被用来支持「吃药没用因为工作结果没变」。
> 但它**确实**说明：**如果要用就业结果来论证任何干预（包括环境干预），必须处理依从性这个混杂。**

---

## 三、睡眠与时相：一个 ADHD-specific 且有真实效应量的小领域

### 3.1 时相（chronotype）

**S30｜Becker, S.P., et al. (2024).** *(大学生中 ADHD 症状与时相)* PMID **37437906** ｜【同行评议论文，仅摘要】｜可信度：**中高**
> **N = 4,751**（73% 女性，80% 白人），18–29 岁（M = 19.28, SD = 1.50）。
> 🔴 晚型（evening type）比例：
> - **ADHD-I：47.2%**
> - **ADHD-C：41.5%**
> - **ADHD-HI：30.7%**
> - **无升高 ADHD 症状：28.5%**

🔴 **「晚型比例随症状从多动冲动型 → 混合型 → 注意力型递减」这个梯度，本身就是一个信息**：
**注意力不集中越占主导的人，越「晚」**。这与 Fredriksen 2015（S20）「注意力不集中 → 劳动残疾」的分工一致。
⚠️ 摘要未报告检验统计量 → 【仅摘要，禁止推断效应量】。

**S31｜Ziegler, B., et al. (2021).** *(ADHD 儿童的睡眠日志与时相：一项阴性研究)* PMID **34942866** ｜【同行评议论文，仅摘要】｜可信度：**中高**
> **57 名儿童（6–12 岁）**：ADHD **n = 24**，对照 **n = 33**。活动记录仪（actigraphy）。
> ✅ ADHD 组：**睡眠潜伏期更长、睡眠潜伏期变异更大、动作更多、睡眠效率更低**
> 🔴 **阴性**：**时相（chronotype）与睡眠起始时间在两组间无差异**
> 🔴 **阴性**：**睡眠问题对神经心理功能的影响，在控制 ADHD 症状严重度之后没有额外效应**
> 🔴 **这条 null 结果极其重要**：它意味着「ADHD 患者的作息问题」很大程度上**由症状本身驱动，而不是由一个独立的昼夜节律病变驱动**。
> **实务含义**：给 ADHD 者调作息，**改症状比强行调钟点更可能有效**。

**S32｜Kuru, B., et al. (2026).** *(青少年 ADHD 的褪黑素与时相)* PMID **41966732** ｜【同行评议论文，仅摘要】｜可信度：**中**
> **ADHD 青少年 n = 41 vs 对照 n = 42**。
> ✅ 晚型时相在 ADHD 组更高
> ❌ **晨间褪黑素无差异：ADHD 312.44 ± 102.29 pg/mL vs 对照 319.84 ± 70.75 pg/mL（不显著）**
> 🔴 **与 Ziegler 2021 构成明确冲突**（一方说时相有差异且晨褪黑素无差异，另一方说时相无差异）。

**S33｜Abanoz, Y., et al. (2025).** *(初治 ADHD 的肠肽与时相)* PMID **41038059** ｜【同行评议论文，仅摘要】｜可信度：**中**
> **45 名未用药 ADHD vs 45 名对照**。
> ✅ 晚间型时相升高（p < 0.001）、就寝抵抗升高、入睡潜伏期延迟、夜间醒来增多、日间嗜睡（全部 p < 0.001）
> ✅ 食欲素-A 降低（p < 0.001）、食欲素-B 降低（p = 0.039）、瘦素降低（p = 0.012）、**胃饥饿素升高（p < 0.001）**
> 🔴 「胃饥饿素升高」这一条与 ADHD-肥胖的高共病率方向一致，但**本文件不做机制外推**。

### 3.2 睡眠剥夺：这一段的证据是 ADHD-specific 且有真实数字的

**S34｜Cohen, A., et al. (2021).** *(睡眠剥夺对 ADHD 与对照的影响差异)* PMID **34244583** ｜【同行评议论文】｜可信度：**中高**
> **35 名男性**：ADHD **n = 19**，对照 **n = 16**。连续清醒 **25 小时**。
> ✅ **遗漏错误、 commissions（虚假警报）错误与反应时变异在 ADHD 组显著升高，在对照组不升高。**

**S35｜Dan, Y., et al. (2026).** *(睡眠剥夺下的 ERP 表现)* PMID **41629587** ｜【同行评议论文】｜可信度：**中**
> ADHD **n = 19** vs 对照 **n = 14**。睡眠剥夺显著增加错误与反应时变异，**在 ADHD 组尤为明显，且对情绪刺激尤其如此**；对照组变化很小。

**S36｜Haimov, I., et al. (2026).** *(睡眠剥夺下的主观困倦曲线)* PMID **41877116** ｜【同行评议论文】｜可信度：**中**
> **59 名年轻男性**：ADHD-C（未用药）**n = 39**，对照 **n = 20**。连续清醒 25 小时。** Karolinska Sleepiness Scale（KSS）>7 分** 的比例：
> - **未用药 ADHD：88.2%**
> - **对照：55%**
> - **用药 ADHD：36.9%**
> 🔴🔴 **这是本文件里对「时间结构与药物」最干净的一条**：
> **同样是熬 25 小时，未用药的 ADHD 男性几乎全员严重嗜睡（88.2%），而用药组只有 36.9%，低于对照。**
> ⚠️ 这是**观察性**研究，不能用于任何用药建议（本 skill 不涉及治疗决策）。**但它确立了一个环境层事实**：
> **在剥夺睡眠的条件下，ADHD 的脆弱性是可测的、可预测的、且高度依赖个体状态的。这正是「环境适配」这个概念存在的理由——环境（夜班/加班/通宵）会选择性地放大某些人的脆弱性。**

**S37｜Kay, M., Wheelock, V., Siegel, J., Raut, A., Chauvin, L., Metoki, A., Rajesh, A. & Eck, E. (2025).** *Stimulant medications affect arousal and reward, not attention networks.* **Cell, 188**(24), 7529–7546.e20.
DOI: **10.1016/j.cell.2025.11.039** ｜PMID **41448140** ｜【同行评议论文】｜可信度：**高**
> **ABCD 静息态 fMRI，n = 11,875（8–11 岁）**；并在**高精度影像药物试验**中以健康成人（n = 5，每人 165–210 分钟）用哌甲酯 40 mg 验证。
> - 兴奋剂相关的连接性差异位于**感觉运动区**，与**日间觉醒模式、夜间睡得更久、去甲肾上腺素转运体表达**相匹配
> - 🔴 **「Taking stimulants reversed the effects of sleep deprivation on connectivity and school grades.」**
> - 改变也出现在**显著性网络与顶叶记忆网络**（对多巴胺介导的奖赏学习重要），**但不在注意系统（如背侧注意网络）**
> 🔴 **注意结论的精确措辞**：*"improving task effort and persistence **without effects on attention networks**."*
> ⚠️ **本 skill 不做用药建议**，此条仅用于说明：**「时间结构 × 睡眠 × 脆弱性」是环境层的真实变量**，且与药物相互作用是**双向**的。

**S38｜Nair, S., Deshpande, N.R., Hill, C.M., Cortese, S., Van Someren, E.J.W. & Chellappa, S.L. (2025).** *Associations of ADHD traits, sleep/circadian factors, depression and quality of life.* **BMJ Mental Health.**
DOI: **10.1136/bmjment-2025-301.625** ｜【同行评议论文】｜可信度：**中高**
> **N = 1,364**，平均年龄 51.86，75% 女性，**荷兰睡眠登记**。
> - ADHD 特质 ↔ 抑郁（p = 0.03）、生活质量更低（p < 0.001）、**失眠（p < 0.001）**、睡眠质量更低（p < 0.001）、**时相更晚（p = 0.01）**
> - 🔴 **关键阴性**：*"**No sleep/circadian factor mediated the association between ADHD traits and depression (all p > 0.1).**"*
> - 只有**失眠严重度**中介了 ADHD 特质 → 生活质量：SLS **β = −0.10（95% CI −0.12 到 −0.04）**；CL **β = 0.103（0.04 到 0.16）**
> 🔴 **这条对环境适配极重要**：**睡眠/昼夜节律解释不了「为什么有 ADHD 特质的人更容易抑郁」。真正有中介作用的是「失眠」这一个具体变量。**
> **实务含义**：环境适配的可操作靶点不是「调整生物钟」，而是**减少失眠**——即减少让入睡困难的环境条件。

### 3.3 时间知觉（几乎全是儿童研究）

**S39｜Nejati, S. & Yazdani, M. (2021).** *(儿童时间知觉/时间加工的 meta 分析)* PMID **32757699** ｜【同行评议论文，meta 分析】｜可信度：**中高**
> **12 项研究，均为儿童样本。**
> 关键：**时间知觉损害在「前瞻性任务 + 长时程间隔」条件下更明显**；**通道（视觉/听觉）不是决定因素**。
> 🔴 **这一条实际上是一个环境设计建议**：**对时间知觉困难的人，把长间隔的任务拆成短间隔、且要求「提前预告」，比改善感官通道更有效。**
> ⚠️ **儿童样本，不可直接外推成人职场。**

---

## 四、轮班制 / 夜班：🔴 **这是一个空白领域**

### 4.1 检索结论

本次调研对以下检索式均执行了 PubMed esearch，**「ADHD + 轮班」组合的专门研究几乎不存在**：
| 检索式 | 命中 |
|---|---|
| `ADHD[Title] AND "shift work"` | 无 ADHD-specific 研究 |
| `ADHD[Title] AND ("night work" OR "night shift")` | 无 |
| `ADHD[Title] AND "sleep deprivation" AND work` | 无 |

🔴 **结论必须明说**：
> **「轮班制对 ADHD 的影响」在本领域没有直接研究。**
> 下面这些是**最接近的证据**，且**每一项的研究人群都不是 ADHD 人群**。
> **把它们用于 ADHD 者是一个外推，外推本身没有被检验。**

### 4.2 最接近的四组证据（全部为非 ADHD 人群）

**S40｜Dönmezdil, S. & Araç, E. (2021).** *(夜班对 ICU 护士注意力与差错的影响)* PMID **33078452** ｜【同行评议论文】｜可信度：**中**
> **72 名 ICU 工作者**（30 女 / 42 男）。
> ✅ 夜班组在**所有时点**的注意力测量（Stroop 色词任务 SCWI）上出现**显著延长**
> ✅ 夜班组**差错与返工显著增加**
> 🔴🔴 **必须标注的重大歧义**：该研究测量的是 Stroop 任务上的**「注意力」**（attention），**这不是 ADHD 诊断，也不是 ADHD 特质的测量**。
> **把它称为「夜班对 ADHD 的影响」是彻底错误的。** 这是一篇关于**任何人**在夜班后认知表现下降的研究。

**S41｜Torquati, E., Barnes, M.A., ... et al. (2020).** *(轮班工作与不良心理健康结局的 meta 分析)* PMID **31536404** ｜【同行评议论文，meta 分析】｜可信度：**高**
> **7 项纵向研究、28,431 名不重复参与者**。
> - 不良心理健康总效应 **ES = 1.28（1.02–1.62）**，I² = 70.6%
> - **抑郁症状 ES = 1.33（1.02–1.74）**，I² = 31.5%
> - 🔴 **性别解释 >90% 的异质性**；**女性轮班工作者 OR = 1.73（1.39–2.14）**
> ⚠️ 人群：一般轮班工作者，**不是 ADHD 人群**。

**S42｜Harris, A., et al. (2024).** *(轮班开始与睡眠/心理健康：系统综述)* PMID **38626702** ｜【同行评议论文，系统综述】｜可信度：**高**
> **48 篇文献**。
> ✅ **轮班开始后，睡眠与心理健康均恶化**
> ❌ **身体健康无显著变化**
> ⚠️ 人群：一般轮班工作者。

**S43｜Ulupınar, C. & Ulupınar, H. (2025).** *(轮班对认知与运动表现的 meta 分析)* PMID **41139761** ｜【同行评议论文，meta 分析】｜可信度：**中高**
> **22 项研究、224 个对照数据点**（以护士为主）。
> - 白班 vs 对照：Hedges' **g = 0.238（0.155–0.321）**
> - **夜班 vs 对照：g = 0.386（0.320–0.451）**
> - 运动表现（全班次合计）：**g = 0.326（0.210–0.442）**
> - 白班 vs 非标准班：g = 0.220（0.171–0.269）
> - **夜班 I² = 86.8%（异质性极高）**
> ⚠️ 人群：护士，**不是 ADHD 人群**。⚠️ **摘要未说明 g 的方向所代表的正负**，此处**不做方向推断**。

### 4.3 职业医学的操作建议（不涉及 ADHD，但可作为环境层的共识）

**S44｜Jogie, Y., et al. (2025).** *(夜间值班与失眠：职业医学立场)* PMID **41473655** ｜【同行评议论文/综述级】｜可信度：**中**
> 立场性结论：在**失眠持续存在期间应避免夜间值班**。
> 🔴 **注意这条的逻辑**：它不是「ADHD 员工不应上夜班」，而是「**有失眠的人**不应上夜班」。
> **把这条转写成 ADHD 建议，就跨越了证据边界。**

### 4.4 🔴 §4 结论

> **把「夜班会让 ADHD 更糟」写进 skill，是一个没有证据支撑的断言。**
> 诚实的写法是三段式：
> 1. **已确证（一般人群）**：夜班与睡眠恶化、心理健康恶化、认知与运动表现下降相关（三个独立 meta 分析，S41–S43）。
> 2. **已确证（ADHD 人群）**：睡眠剥夺对 ADHD 的影响**大于**对对照的影响（S34、S35、S36，且 S36 有明确的量级差：88.2% vs 55%）。
> 3. **🔴 缺失的那一环（两层都没做）**：**「轮班 → 睡眠剥夺 → ADHD 特质者的认知/健康后果」这一条链，从未在 ADHD 人群中被测量过。**
>
> **第 2 点 + 第 1 点的逻辑推论，不能被写成结论。**
> 但它**可以**被写成本 skill 的一个**明确的标注为「推断」的适配建议**：
> 若一个体已知在睡眠剥夺下会出现 §3.2 那种量级的功能恶化（且这是可测的），那么**把这样的个体放进需要长期夜班或通宵的结构，就是把一个已知的放大器接在已知的高危位置上**。

---

## 五、「时间盲」这个术语本身的证据地位

**S45｜de Melo, M.C. & Franca, A.C. (2026).** *(视角/评论文章)* PMID **42232996** ｜【同行评议论文（观点/评论）】｜可信度：**低-中**
> 立场性文章，主张 **「时间盲」（time blindness）是 DSM 诊断标准中未被充分表达的现象之一**。
> 🔴 **这是主张，不是数据。** 它的价值在于：**「时间盲」是一个尚未进入诊断标准的构念，因此它也就没有对应的、独立的效度研究。**

**S46｜Tolani, D.S. & Venkatesan, S. (2025).** *(graphic medicine：时间盲)* PMID **40059708** ｜【同行评议论文（图像/叙事类）】｜可信度：**低】
> 漫画/叙事形式表达「时间盲」体验。**不提供实证数据。**

🔴 **本文件对「时间盲」的正式处理**：
> **「时间盲」在学术上不是一个被独立验证的构念。** 它主要存在于临床描述、病人叙事与漫画里。
> **但它描述的现象是真的，而且它的职场后果是本文件里证据最硬的**（S13–S19）。
> **正确的用法**：把「时间盲」当作**现象标签**使用，而把 **S13–S19 的数字**当作**证据**使用。不要反过来——不要因为「时间盲」这个词听起来精准，就认为它背后有一套已被验证的测量。

---

## 六、数字冲突清单（本维度）

| # | 冲突点 | A 方 | B 方 | 状态 |
|---|---|---|---|---|
| 1 | **职业是否改变 ADHD 的职场损失幅度** | **Kessler et al. 2005（JOEM, n=3,198）**：蓝领 55.8 天 vs 专业 12.2 天（**4.6 倍**） | **de Graaf et al. 2009（OEM, 10 国 n=7,075）**：*"**No difference in the magnitude of this effect was found by occupation, education, age, gender or partner status**"* | 🔴 **直接冲突。** 两次调查相隔 4 年，均为 Kessler 领衔、方法相似。Kessler 2005 自己给的解释是「需要效果试验」——**这可能就是他 2009 年改做单一企业研究的原因** |
| 2 | **年损失天数** | Kessler 2005：**35.0 天/年** | de Graaf 2009：**22.1 天/年** | 🔴 不同样本（美国 vs 10 国）、不同结局框架（lost work performance vs excess lost role performance）。**不可互相替换** |
| 3 | **成人 ADHD 在劳动者中的患病率** | Kessler 2005：**4.2%**；de Graaf 2009：**3.5%**（IQR 1.3–4.9%）；Kessler 2009 单一企业：**1.9%（SE 0.4）**；Song et al. 2021 全球：**2.58%（持续型）/ 6.76%（症状型）** | — | ⚠️ **不是矛盾，是测量口径不同**：临床再访谈校准 vs ASRS 筛查 vs 自报 vs 定义不同（持续型/症状型）。**引用时必须带口径** |
| 4 | **时相在 ADHD 中是否改变** | Kuru et al. 2026：晚型时相在 ADHD 青少年中更高；Abanoz et al. 2025：晚型升高（p<0.001） | **Ziegler et al. 2021（活动记录仪，n=57）：时相与睡眠起始时间在两组间无差异** | 🔴 未解决。**测量工具不同（问卷 vs 活动记录仪）是最可能的解释，但没有人做过对比** |
| 5 | **晨间褪黑素** | Kuru et al. 2026：ADHD 与对照**无差异**（312.44 vs 319.84 pg/mL） | — | ⚠️ **单点阴性结果。** 与「晚型时相有差异」并存 → **时相差异可能不由晨间褪黑素分泌水平驱动** |
| 6 | **睡眠问题是否独立于 ADHD 症状起作用** | Abanoz et al. 2025：睡眠问题共 5 项全部 p<0.001 | **Ziegler et al. 2021**：控制症状严重度后，睡眠问题对神经心理功能**无额外效应**；**Nair et al. 2025**：除失眠外，所有睡眠/昼夜因素**均不中介** ADHD→抑郁（all p>0.1） | 🔴 **未解决，且方向明确一致**：**症状严重度解释大部分；失眠是唯一存活的独立变量。** 「先治症状再谈作息」有三条独立支持 |
| 7 | **兴奋剂是否改善就业结局** | Kessler et al. 2009 结论段："in conjunction with evidence from controlled trials that **treatment can reduce ADHD-related impairments**" | **Pathan et al. 2026（MEPS, n=1,290）**：调整混杂后**就业结局无显著差异** | 🔴 **未解决。** Pathan 是观察性、有依从性混杂、结局自报 → **不能推翻 RCT 证据**；但它说明**就业结局是一个很难测的终点** |
| 8 | **迟到的证据在哪** | Vágová et al. 2023：**学校档案**记录迟到与出勤负面反馈 | Durand et al. 2024：**自报**组织性技能（**仅题录，无摘要**） | ⚠️ **两边都不是职场迟到。** 本维度**没有「ADHD 成人职场迟到率」的客观研究**——这是一个具体而明确的空白 |

---

## 七、本文件最重要的一句话判断

> **关于时间与工作，最可靠的经验法则是「删掉决策、别删结构」**：
> **删掉一个需要 ADHD 者自己**决定**「什么时候做、做多久、先做哪个」的决定，效果的证据基础（时间管理 RCT、奖金式休息、非标准化班次的 meta 分析）比**「给一份更适合他的工作」**扎实得多；
> **而一旦把「我可以不轮班」「我不用在通宵后做重要判断」「我的截止日期由外部提醒固定」写进环境变量，它就不再需要那个人具备自我管理能力——那正是这一维度里唯一没有被证实可以靠个人练出来的能力。**

---

## 来源总表（本文件，46 个独立来源/条目）

**【同行评议论文 · meta 分析】（7）**
1. Jackson & MacKillop (2016/2023) *Biol Psychiatry Cogn Neurosci Neuroimaging* — `10.1016/j.bpsc.2016.01.007` / PMID 27722208
2. Patros et al. (2016) *J Autism Dev Disord* — PMID 26602954
3. Pauli-Pott & Becker (2016) *Atten Defic Hyperact Disord* — PMID 25956255
4. Marx et al. (2021) *Neuropsychol Rev* — PMID 29806533
5. Doidge et al. (2021) *J Autism Dev Disord* — PMID 30596297
6. Suriano (2026) *Res Dev Disabil* 175:105342 — `10.1016/j.ridd.2026.105342` / PMID 42456607
7. Nejati & Yazdani (2021) — PMID 32757699
8. Torquati et al. (2020) — PMID 31536404
9. Ulupınar & Ulupınar (2025) — PMID 41139761

**【同行评议论文 · 大样本流行病学/登记】（9）**
10. Kessler et al. (2005) *JOEM* 47:565–72 — `10.1097/01.jom.0000166863.33541.39` / PMID 15951716
11. de Graaf et al. (2009) *OEM* 65:835–42 — `10.1136/oem.2007.038448` / PMID 18505771
12. Kessler et al. (2009) *Psychol Med* 39:137–47 — `10.1017/S0033291708003309` / PMID 18423074
13. Kleinman et al. (2010) *JOEM* 51:1247–55 — `10.1097/JOM.0b013e3181bca68c` / PMID 19858744
14. Virtanen et al. (2021) *Scand J Work Environ Health* 46:410–16 — `10.5271/sjweh.3888` / PMID 32076730
15. Helgesson et al. (2023) *Psychol Med* 53:1224–32 — `10.1017/S0033291721002701` / PMID 35275515 ← 与 01/04 共用
16. Ahlberg et al. (2023) *BMC Psychiatry* 23:336 — `10.1186/s12888-023-04713-z` / PMID 37173664
17. Verheul et al. (2016) *Eur J Epidemiol* — `10.1007/s10654-016-0159-1` / PMID 27177909 ← 与 01 共用
18. Seppä et al. (2026) — PMID 40892097

**【同行评议论文 · 临床/实验/干预】（11）**
19. Fredriksen et al. (2015) *ADHD Atten Disord* 6:87–99 — `10.1007/s12402-014-0126-1` / PMID 24497125
20. Fuermaier et al. (2021) *J Neural Transm* 128:1021–31 — `10.1007/s00702-021-02309-z` / PMID 33528652
21. Nakashima et al. (2022) *J Atten Disord* 26:377–390 — `10.1177/1087054720986939` / PMID 33472510
22. Bangma et al. (2019) *Neuropsychology* — `10.1037/neu0000571`
23. Cohen et al. (2021) — PMID 34244583
24. Dan et al. (2026) — PMID 41629587
25. Haimov et al. (2026) — PMID 41877116
26. Kay et al. (2025) *Cell* 188:7529–46 — `10.1016/j.cell.2025.11.039` / PMID 41448140
27. Chen et al. (2021) *J Psychiatr Res* 139:62–70 — `10.1016/j.jpsychires.2021.05.008` / PMID 34044265
28. Oguchi et al. (2023) *Heliyon* 9:e14834 — `10.1016/j.heliyon.2023.e14834` / PMID 37025860
29. Pathan et al. (2026) *J Atten Disord* 30:916–29 — `10.1177/10870547261433489` / PMID 41914673

**【同行评议论文 · 睡眠与时相】（6）**
30. Becker et al. (2024) — PMID 37437906
31. Ziegler et al. (2021) — PMID 34942866
32. Kuru et al. (2026) — PMID 41966732
33. Abanoz et al. (2025) — PMID 41038059
34. Nair et al. (2025) *BMJ Ment Health* — `10.1136/bmjment-2025.301.625`
35. Harris et al. (2024) — PMID 38626702

**【同行评议论文 · 轮班与一般认知】（3 + 1）**
36. Dönmezdil & Araç (2021) — PMID 33078452
37. Jogie et al. (2025) — PMID 41473655

**【仅题录（禁止推断结论）】（4）**
38. Owens & Hinshaw (2017) — PMID 27739390
39. Acuff et al. (2018) — PMID 28910128
40. DeRosa et al. (2024) — PMID 37524685
41. Vágová et al. (2023) — PMID 36484286
42. Durand et al. (2024) — PMID 33194353

**【观点/评论/叙事类（不提供实证）】（4）**
43. Isen et al. (2015) — PMID 24999868（含阴性结果，故仍列实证）
44. de Melo & Franca (2026) — PMID 42232996
45. Tolani & Venkatesan (2025) — PMID 40059708
46. Wang et al. (2018) — PMID 28498515（非 ADHD 样本）

---

## ⚠️ 本文件的已知缺口（诚实清单）

| 缺口 | 状态 |
|---|---|
| 「延迟折扣 → 真实职场表现」在 ADHD 人群中的中介检验 | 🔴 **不存在。** 已检索，无结果 |
| ADHD 成人的**职场迟到率客观数据** | 🔴 **不存在。** 仅有学校档案（Vágová）与自报（Durand） |
| **轮班制 × ADHD** 的任何专门研究 | 🔴 **不存在。** S40–S44 人群均非 ADHD |
| ADHD × 换班/倒班安排的实证 | 🔴 **不存在** |
| Isen et al. 2015 的完整效应量 | ⚠️ 摘要未报告 |
| Durand et al. 2024 的摘要 | ⚠️ **PubMed 无摘要**，需全文 |
| Owens & Hinshaw 2017 的中介路径系数 | ⚠️ 摘要未报告 |

---

**⚠️ 提示注入记录**：本文件全部内容来自 **NCBI E-utilities REST API 与 Europe PMC REST API** 的 JSON/XML 直连返回，**全程未抓取任何 HTML 网页**，因此**不存在页面内嵌提示注入文本的风险面**。无注入事件。
**数据准确性**：本文件引用的每一个数字，均由本 Agent 重新执行 `pmfetch.py`（NCBI efetch）逐条取回并**逐字核对**后才写入。subagent 起草阶段曾出现「凭记忆写 DOI」的情况，已通过 Crossref 交叉核验纠正（Jackson & MacKillop 的 DOI 年份差异 2016/2023 已在本文件 §1.1 显式标注）。
