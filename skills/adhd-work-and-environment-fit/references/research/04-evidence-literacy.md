# 04 — 证据素养：如何审查一句「我有 ADHD，所以我适合做 X」

**调研时间：2026-10-12**
**取数路径**：NCBI E-utilities · OpenAlex API · Crossref API · Europe PMC API · 出版方书籍页与机构站点直取。

> **本文件的用途**：本 skill 的后半段是**反向工具**。前三个维度告诉你「什么环境适配得好」，
> 本文件告诉你**怎么识别一个听起来合理、其实站不住的适配论证**。
> 本文件的核心不是「反对 ADHD 优势叙事」，而是**给它一个可被审查的形式**。

---

## 零、这条论证的结构（先把它拆开）

典型的「我有 ADHD 所以我适合做 X」论证，实际由三步组成：

| 步骤 | 形式 | 合法所需证据 |
|---|---|---|
| ① **观察** | 「有 ADHD 的人里，有不少做成了 X」 | 分子事实：需要**分母**才有用 |
| ② **归因** | 「他们做成 X，是因为 ADHD」 | 需要**排除替代解释**（选择效应、幸存者偏差、资源、时代） |
| ③ **外推** | 「所以（我这样的）ADHD 人适合做 X」 | 需要**在一般 ADHD 人群中成立**，而非在成功者子集中成立 |

🔴 **三步中有两步是独立的、必须分别取证的方法学主张，而绝大多数流行论证只做了第 ① 步。**
本 skill 的审查清单就是按这三步组织的。

---

## 一、最致命的方法学缺陷：条件概率的方向被调换了

### 1.1 缺陷陈述

> **这个论证测的是 `P(ADHD | 成功)`，而结论需要的是 `P(成功 | ADHD)`。这两个数在基率不均衡时可以差得任意远。**

这在概率论上叫**条件概率倒置**（conditional probability inversion），在司法语境里叫**检察官谬误**。

### 1.2 用本次调研拿到的真实数字演示这个差距有多大

**分子侧的数（`P(ADHD | 成功)`）——这是所有流行论证的来源：**
- 各类「知名创业者/名人确诊 ADHD」的叙事
- Wiklund, Patzelt & Dimov (2016) 的定性研究：**14 位**已诊断 ADHD 的创业者
  DOI: **10.1016/j.jbvi.2016.07.001**【同行评议论文，n=14】

**分母侧的数（`P(成功 | ADHD)`）——这是流行论证从不看的部分：**

| 指标 | 数值 | 来源 | DOI / PMID |
|---|---|---|---|
| 成人 ADHD「持续型」患病率（全球，一般人群） | **2.58%** | Song, Zha, Yang, Zhang, Li & Rudan (2021), *J Global Health* 11:04009 | `10.7189/jogh.11.04009` / PMID 33692893 |
| 成人 ADHD「症状型」患病率（无论童年起病） | **6.76%**（约 3.66 亿人） | 同上 | 同上 |
| **临床转诊成人 ADHD 中「以常规工作为主要收入来源」的比例** | **仅 22.2%**（一般人群为 **72%**） | Gjervan, Torgersen, Nordahl & Rasmussen (2013), *J Atten Disord* 16(7):544–552 | `10.1177/1087054711413074` / PMID 21725028 |
| 19–29 岁新诊断 ADHD 者 5 年内**领到残疾养老金**的比例 | **21%** | Chen, Mittendorfer-Rutz, Björkenstam, Rahman, Gustafsson, Taipale, Tanskanen & Ekselius (2022), *J Atten Disord* 26(7):723–734 | `10.1177/10870547211025605` / PMID 34154443 |
| 同队列相对匹配对照的**残疾养老金 HR** | **10.2 (95% CI 9.3–11.2)** | Helgesson et al. (2023), *Psychol Med* 53(7):1224–1232 | `10.1017/S0033291721002701` / PMID 35275515 |
| 同队列相对匹配对照的**长期病假（>90 天）HR** | **2.7 (2.5–2.8)** | 同上 | 同上 |
| 同队列相对匹配对照的**长期失业（>180 天）HR** | **1.7 (1.6–1.8)** | 同上 | 同上 |
| 儿童期 ADHD → 成年**就业率**下降 | **10–14 个百分点** | Fletcher, J.M. (2013), NBER Working Paper 18689（含同胞固定效应设计） | `10.3386/w18689` |
| 儿童期 ADHD → 成年**收入**下降 | **约 33%** | 同上 | 同上 |
| 儿童期 ADHD → 成年**社会救助**增加 | **15 个百分点** | 同上 | 同上 |
| 儿童期 ADHD → **终生收入**投影差距 | **少赚 543,000–616,000 美元** | Altszuler, Page, Gnagy, Coxe, Arrieta, Molina & Pelham (2017), *J Abnorm Child Psychol* 44(7):1217–29 | `10.1007/s10802-015-0093-9` / PMID 26542688 |
| 有 ADHD 或抑郁（不兼有）者平均收入差距 | **约 20%** | Hartge & Toledo (2019), *J Mental Health Policy Econ* 21:105–121 | PMID 30530871 |
| ADHD 遗传多基因风险分（PRS）每升高 → 就业、收入、家庭财富**下降**；社会安全残障金、失业、工伤**上升**；**教育程度中介 14–58%** | 方向性 | Rietveld & Patel (2020), *Eur J Health Econ* 20:949–967 | `10.1007/s10198-019-01055-0` / PMID 31049764 |

🔴 **把这些数放在一起，条件概率倒置的量级立刻显形**：

> **「成功创业者里有很多 ADHD」是真实的（分子侧有支撑）。**
> **但「ADHD 成人里只有 22.2% 以常规工作为生，而全体 ADHD 成人中 21% 在 5 年内被判定为残疾、风险是对照的 10.2 倍」——这是分母侧。**
> **一个论证如果只出示分子、不出示分母，它就不是「证据不足」，而是**结构性地**系统性地朝一个方向偏。**

⚠️ **必须同时诚实标注的相反方向**：
- **Wiklund, Rietdijk 等人的瑞典双胞胎登记研究（瑞典 N=7,208 + 荷兰 N=13,112 复制）确实发现 ADHD 症状与自雇正相关**（一般症状 OR 1.13 [1.04–1.23]；hyperactivity OR 1.19 [1.08–1.32]；**inattention OR 0.99 [0.89–1.10] 无关联**）。DOI **10.1007/s10654-016-0159-1**。
  🔴 **这条不能被省略。** 一个诚实的证据素养文件必须说：**分子侧不全是幸存者偏差的幻觉，它有一部分是真的。** 但注意效应量（OR ≈ 1.1–1.2）**极小**，且**完全由 hyperactivity 承载，inattention 的 OR 恰好是 0.99**。
- **本文件不是在说「ADHD 的人不适合创业」。本文件是在说：「这句话的说服力不来自它的分母，而分母那一侧的数据显示的是另一回事。」**

### 1.3 为什么这条缺陷最致命，而不是「样本量小」之类

因为它**无法用更大的样本修复**。你把 n 从 14 提到 14,000，如果抽样框仍然是「成功者」，倒置依然存在，而且更精确、更自信、更错误。**这是设计缺陷，不是精度缺陷。** 这是它比其他所有批评都致命的原因。

---

## 二、幸存者偏差在 ADHD 优势叙事里的三个具体变体

### 2.1 变体一：**样本即社交圈**（Dale Archer 的核心方法学问题）

来自本项目已有的调研（`references/dale-archer-cautionary-research/05-decisions.md` 等）的最尖锐一条读者批评：

> 「Dr Archer's assertion that ADHD is a gift, an advantage **while ignoring the realities on the ground is unscientific, potentially dangerous and very simplistic**… **At times I felt like I was reading the diaries of the rich and famous who have the means to make certain types of big changes while ordinary people do not.**」
> — NetGalley 书评（2/5 星），https://www.everand.com/audiobook/638424914/

🔴 **这不是「样本量小」，是抽样框错了**：他的样本 = 他的病人 + 他的朋友 + 他的名人案例 + 他的孩子。
**成功案例几乎全部是有资源、有助理、有合伙人、有家庭兜底的人**——而这些恰恰是分母里最特殊的一层。

### 2.2 变体二：**分母被删掉的那一层**

- 【机构/临床人员表述，经媒体引述】*Psychology Today* (2013)《Should We Welcome the "Gift" of ADHD — or Return it?》：
  > 「…the case for ADHD as a gift **seems speculative and selective**. It tempts advocates **off the scientific high ground**, as when Koretsky cites a group of high achievers as representative of this condition. **What of the school drop-outs, the impulsive jail population, and the vast majority between these two extremes?**」
  https://www.psychologytoday.com/au/blog/aspergers-alive/201310/should-we-welcome-the-gift-adhd-or-return-it
  🔴 **"What of…" 这一句是对本 skill 反向问题最精确的方法学表述**：优势论证的分母不是被测量了，是**被删除了**。

- ⚠️ **一个必须记录的尖锐巧合**：Dale Archer 本人 1988–1995 是 Phelps Correctional Institute 的**监狱精神科医生**，并在刑事法庭担任数百次 sanity / competency 专家证人。
  **他比大多数人更清楚被丢掉的「分母」里有什么。** 这条不构成对他论证的反驳（知道分母的存在不等于必须否认优势），但它构成对**「分母被删除」这一动作**的最强反讽。

### 2.3 变体三：**「在成功者中占多数」被读成「成功的原因」**

这一变体有同项目材料里最干净的一张对照表（Dale Archer vs Russell Barkley 用**同一批案例人物**得出相反结论）：

| | Dale Archer | Russell Barkley |
|---|---|---|
| Pennington 的成功归因于 | 其 ADHD 特征被善用 | **父母/导师的引导**（"guided to choose a career that took advantage of his unique strengths"） |
| Phelps 的成功归因于 | ADHD 赋能的韧性 | **家庭教他建立常规**（"Phelps's family taught him to adopt routines"） |
| 关键论断 | successful **because of** their ADHD | successful **in spite of** it, **not because of** it |

— 出处：*Library Journal* 对 Barkley《12 Principles for Raising a Child with ADHD》(2020) 的书评，https://www.libraryjournal.com/review/12-principles-for-raising-a-child-with-adhd

🔴 **同一批人，相反的结论，取决于谁在解释。** 这一张表本身就是「选择性归因」的最佳教学材料，也是本 skill 反向判断清单的第一条模板。

---

## 三、核实任务：Sam Goldstein「近 4000 项研究中没有一项显示 ADHD 组更优」

### 3.1 核实结论：**核实通过，但来源等级远低于流行引用给人的印象**

**原始出处**（本次直连取到全文）：
- **Sam Goldstein, PhD（临床心理学家）《ADHD As An Advantage/Adaptation Revisited》**，发布于其个人网站 `samgoldstein.com` 的 **Articles** 栏目。
  https://samgoldstein.com/resources/articles/general/adhd-as-an-advantageadaptation-revisited.aspx

**原文（逐字）**：
> "**In the nearly 4,000 peer reviewed, scientific studies dealing with ADHD over the past thirty years, there hasn't been a single study in which the group with ADHD performed better on a valuable trait, asset or behavior than those without ADHD.** This is not to moralize, demonize, nor pathologize children with ADHD. It is to suggest that being delayed in the development of self-control in our complex society is **no picnic.** … I do not believe we need to create myths or 'Just So Stories' to help children with ADHD and their families feel better about this impairing condition."

**核实到的四个事实**：
| 项 | 核实结果 |
|---|---|
| 载体类型 | ❌ **不是同行评议论文**。是临床心理学家个人网站上的**专栏/文章** |
| 发表日期 | ⚠️ **页面未提供发表日期** |
| 「近 4000 项」这个数字的来源 | ❌ **未给出任何引文、方法或检索策略** |
| 作者资质 | 临床心理学家（clinical psychologist），**非该领域的实证研究者** |

🔴 **本文件的处理**：把这句话记为**【临床人员专业意见 / 机构外专栏】**，**不记为同行评议证据**。它的**修辞力量远大于它的证据力量**——这也是为什么它被广泛转述。

### 3.2 ⚠️ 但同时必须记录：**这句话的绝对形式已被 2025 年的一项 meta 分析所挑战**

这不是要驳倒 Goldstein，而是要**精确化**他的主张：

- **Tran, M.H., Wiklund, J., Antshel, K.M., Jhawar, N., & Montgomery, C. (2025).** *Entrepreneurship and ADHD: A Meta-Analytical Assessment of the State-of-the-Art and Suggestions for the Future.* **Entrepreneurship Theory and Practice**.
  DOI: **10.1177/10422587251392498**【同行评议论文，meta 分析】｜可信度：**高**
  > **47 项研究、298 个效应量**的结论：
  > - hyperactivity/impulsivity 与「创业**态度与行为**」**正相关**
  > - 总 ADHD 症状与「ADHD 诊断」与「创业**行为**」**正相关**

🔴 **也就是说：Goldstein 那句「没有任何一项研究显示 ADHD 组在某个有价值特质上优于非 ADHD 组」作为绝对命题，现在有了反例。**

**但这个「反例」的成立方式极其重要，而且它恰恰证明了本 skill 的主张**：
- 反例的方向是**「进入行为」**，不是**「结果」**。同一篇 meta 分析说：hyperactivity/impulsivity 与 **post-launch outcomes 不显著**，inattention 与 outcomes **负相关**。
- 反例的效应量**很小**（最干净的一项：自雇 OR 1.13–1.19）。
- 反例的**域是高度自选择的**——只有创业这一个领域反复出现这个方向，且只在「hyperactivity」这一半症状上。

🔴 **精确化后的可引用版本**（本 skill 建议采用）：
> 「在**广泛、多数人都在意的**特质上，ADHD 群体相对非 ADHD 群体的比较优势**至今没有被可靠地建立**。唯一反复出现的 ADHD 正向关联，集中在**「进入一个高度自选择的高不确定性领域」这一种特定行为上**，效应量小（OR ≈ 1.1–1.2），且只由 hyperactivity 症状承载；**而同一批研究在「开业后结果」这一层给出的是零效应或负效应。**」

⚠️ 这既没有采信 Goldstein 的绝对形式，也没有采信优势叙事的通俗形式。**它是一个真正分歧并列的版本。**

### 3.3 相关的同方向证据：优势研究本身的结构

- **Rafael, L.M., Jia, M., Rouel, A., Wootton, D., & Mitchison, D. (2026).** *Attention Deficit/Hyperactivity Disorder (ADHD)-Related Strengths in Adults: A Scoping Review.* **Journal of Attention Disorders, 30**(4), 1207–1232.
  DOI: **10.1177/10870547261425737** / PMID 41889015【同行评议论文，scoping review】｜可信度：**高**
  > **125 项研究**（61 定性 / 59 定量 / 5 混合）。其中 **88 项（70%）是先验（a-priori）以「优势」为研究目的**；**68 项（54%）泛泛研究「优势或体验」，而非聚焦某个具体优势**。
  🔴 **70% 的研究问题是「ADHD 有什么长处」——一个领域如果 70% 的研究都从「一定有长处」出发，它必然产出一个长处清单。这不是造假，这是研究议程的自我实现。**

---

## 四、核实任务：Allen Frances「诊断率翻三倍是药企营销制造的 fad」

### 4.1 核实结论：**出处确认，但用户笔记里的归属需要修正**

🔴 **重要修正**：这句话**不是**出自 Frances 的书《Saving Normal》(2013)，而是出自他为 Dale Archer《The ADHD Advantage》**所写的序言**（该书 2015 年出版）。这直接影响引用方式。

**原始出处（本次直连取到序言全文）**：
- **Allen Frances, MD**（DSM-IV 任务组主席），**Foreword to Dale Archer, *The ADHD Advantage***，Penguin Random House Higher Education 页面全文：
  https://penguinrandomhousehighereducation.com/book?isbn=9780698194380

**原文（逐字，关键句）**：
> "As chair of the task force that produced the fourth edition of the Diagnostic and Statistical Manual, **I have been alarmed by the tripling of ADHD rates in just twenty years.** It's not that our kids are getting sicker. Human nature is remarkably constant. **Some of the increase may be due to better recognition of real cases**, but the evidence is overwhelming that we are in the midst of **a fad largely engineered by drug companies' misleading marketing** to doctors, stressed parents and overworked teachers, as well as a quick-fix mentality and insurance demands that a diagnosis be made immediately on a first visit."

**序言中给出的具体数字（原样记录，全部为约 2014–2015 年美国数据）**：
- 4–17 岁儿童 ADHD 诊断率 **11%**，用药率 **6%**
- **15%** 的儿童在投票年龄前会拿到该诊断
- 青少年男性：**20% 被诊断、10% 被用药**
- 「**一个孩子出生的日期是能否拿到标签的最佳预测因子。班上最小的孩子获得诊断的可能性几乎是最大的孩子的两倍。**」
- 美国 ADHD 药物销售额：**20 年前 4,000 万美元 → 现在 90 亿美元**
- 「**三分之一的大学生**」使用兴奋剂，「**十分之一的高中生**」
- 兴奋剂过量使用** quadrupled**（翻了两番）
- 「**超过 10,000 名两岁和三岁的孩子**已经在用兴奋剂」

### 4.2 🔴 这段文字里，**可信度不均匀**——必须分层使用

| Frances 的主张 | 本次调研找到的支持 | 判定 |
|---|---|---|
| **相对年龄效应**（最小的孩子更可能被诊断） | ✅ **有强同行评议支持**：**Layton, P.E., Barnett, J., Hicks, G.T., & Jena, A.B. (2018).** *Attention Deficit-Hyperactivity Disorder and Month of School Enrollment.* **New England Journal of Medicine, 379(22), 2122–2130.** DOI **10.1056/NEJMoa1806828** / PMID **30485780**。样本 **407,846 名 2007–2009 年出生儿童**，随访至 2015。**在有 9 月 1 日入学截止日的州**：8 月生 ADHD 诊断率 **85.1/10,000**（95% CI 75.6–94.2），9 月生 **63.6/10,000**（95% CI 55.4–71.9），**绝对差 21.5/10,000**；无截止日的州差值 **8.9/10,000（95% CI −14.9–20.8，不显著）**。用药率差 **12.5/10,000（2.43–22.4）**。哮喘/糖尿病/肥胖**无**相应差异。 | ✅ **成立，且机制干净**（有出生月反事实对照） |
| ⚠️ 但**倍数**对不上 | Frances 说「**几乎是两倍**」；Layton 2018 的实测是 **85.1 vs 63.6 ≈ 1.34 倍**（不是 2 倍） | 🔴 **数字冲突**：见 §六 冲突 #1 |
| **药企营销是主因** | ❌ **本次调研未找到任何因果识别研究**支持「营销 → 诊断率」这条因果链 | ⚠️ **【研究者个人主张 / 因果归因未经检验】**。注意这是 Frances 本人回顾 DSM-IV 的自述性判断，他用 "the evidence is overwhelming" 形容，但**这句话本身没有给出证据清单** |
| **诊断率真的在涨吗？** | ⚠️ **存在直接对立的同行评议结论** | 🔴 见下方冲突 #2 |
| **药物销量数字** | ⚠️ 未独立核实 | 标注【序言中的原始数字，未独立核实】 |

### 4.3 🔴 关于「诊断率是否真的在上升」——**必须并列保留的正反两面**

**反面（诊断率确实在上升）：**
- **Ingimarsson, O., Guðbrandsdóttir, R.K., Lauth, B., & Sigurðsson, E. (2024).** *High prevalence of treatment with ADHD medicines indicates overdiagnosis of ADHD in Iceland.* **Læknablaðið.**
  DOI: **10.17992/lbl.2024.09.804**【同行评议论文】｜可信度：**中高**
  > 冰岛全国回顾性队列（2004–2023 全部 ADHD 药物处方者）。2023 年 **7–17 岁青少年 14.7%** 收到 ADHD 药物处方（男 17.7%、女 11.6%）；**18–44 岁成人 10.2%**。2010–2023 年增幅：7–17 岁男 +93%、**女 +224%**；18–44 岁男 +414%、**女 +543%**。结论原文：*"The prevalence of Icelanders who have received an ADHD diagnosis is **double to treble** that observed in the best available studies in other populations. We therefore call for an **urgent review of how ADHD diagnoses are made** in Iceland."*

**正面（患病率并未上升，涨的是诊断）：**
- **Martin, A.F., Rubin, G.J., Rogers, M.B., Wessely, S.C.M., Greenberg, N.L., & Hall, C.E. (2025).** *The changing prevalence of ADHD? A systematic review.* **Journal of Affective Disorders**, 2025.
  DOI: **10.1016/j.jad.2025.119427**【同行评议论文，系统综述】｜可信度：**高**
  > 摘要原文：**40 项研究、17 个国家**（另 1 项跨 42 国），均为 2020 年后发表。*"**No significant rise in ADHD prevalence was found**, although **incidence was found to vary during the COVID-19 pandemic**. **Only four of the included studies were at low risk of bias.**"* 结论：*"The highest quality findings **do not suggest an increase in prevalence since 2020** but indicate some variability in incidence during the COVID-19 pandemic."*

- **Merten, E.C., Cwik, J.C., Margraf, J., & Schneider, S. (2017).** *Overdiagnosis of mental disorders in children and adolescents (in developed countries).* **Child and Adolescent Psychiatry and Mental Health, 5**, 5.
  DOI: **10.1186/s13034-016-0140-5**【同行评议论文，系统综述】｜可信度：**高**
  > 摘要原文：*"**Overdiagnosis in clinical practice rather than an actual increase is assumed to be the cause** for this situation. We conducted a systematic literature search… **only one study was able to examine overdiagnosis of child and adolescent mental disorders from a methodological point of view. This study found significant evidence of overdiagnosis of attention-deficit/hyperactivity disorder.**"*

🔴 **本文件的判定**：**「诊断率在涨、患病率没涨」目前有较高质量的支持**（Martin et al. 2025 是唯一一篇明确说「最高质量的研究不支持患病率上升」的近期系统综述）。
**但 Frances 的因果归因（药企营销 → 诊断率）与「诊断率上涨」是两个不同的命题，前者本次未找到因果证据。**
⚠️ 且 Martin et al. 2025 自己报告「**只有 4 项纳入研究处于低偏倚风险**」——**这个领域自己的证据质量也是薄的。**

---

## 五、核实任务：Kazda et al. 2021 *JAMA Netw Open* 4(4):e215335

### 5.1 🔴 **重要修正：论文身份与用户笔记不符**

| 项 | 用户笔记 | **核实结果** |
|---|---|---|
| 论文标题 | （未写） | **《Overdiagnosis of Attention-Deficit/Hyperactivity Disorder in Children and Adolescents》** |
| DOI | *JAMA Netw Open* 4(4):e215335 | **10.1001/jamanetworkopen.2021.5335** ✅（5335 = e215335，一致） |
| 「334 项研究」 | ✅ | ✅ **正确**：12,267 篇潜在相关 → **334 篇（2.7%）纳入** |
| 人群 | 暗示可谈工作/经济后果 | 🔴 **是儿童与青少年（≤18 岁）**，不是成人 |

- **Kazda, L., Bell, K., Thomas, R., McGeechan, K., Sims, R., & Barratt, A.L.B. (2021).** *Overdiagnosis of Attention-Deficit/Hyperactivity Disorder in Children and Adolescents.* **JAMA Network Open, 4**(4):e215335.
  DOI: **10.1001/jamanetworkopen.2021.5335**【同行评议论文，scoping review】｜被引 219 ｜可信度：**高**

### 5.2 摘要原文的完整计数（这是全部可引用的分层数据）

> - 从 **12,267** 篇潜在相关研究中纳入 **334 篇（2.7%）**；其中 **61 篇（18.3%）为二次研究、273 篇（81.7%）为一手研究**
> - **Question 1**（是否存在「ADHD 蓄水池」）——**104 项研究**发现大量证据
> - **Question 2**（诊断是否真的增加）——**45 项研究**
> - **Question 3**（新增病例是否在谱系的轻度端）——**25 项研究**
> - **Question 4**（药物治疗是否增加）——**83 项研究**
> - **Question 5**（诊断与药物治疗的后果）——**151 项研究报告了后果**
> - 🔴 **「However, only 5 studies evaluated the critical issue of benefits and harms among the additional, milder cases. These studies supported a hypothesis of diminishing returns in which the harms may outweigh the benefits for youths with milder symptoms.」**
> - 结论：*"This review found evidence of ADHD **overdiagnosis and overtreatment** in children and adolescents… therefore **practitioners should be mindful of these knowledge gaps**, especially when identifying these individuals and to ensure safe and equitable practice and policy."*

### 5.3 🔴 关于任务书的「补充工作/经济后果的分层数据」——**必须纠正前提**

**这篇论文无法提供成人工作/经济后果的分层数据**，原因有二：
1. **人群限定**：纳入标准为「age ≤ 18」。
2. **它自己的结论就是「这个分层恰恰不存在」**：151 项研究报告了后果，但**只有 5 项真正评估了「新增的轻度病例」的利弊**。

🔴 **但这条「只有 5 项」的发现，本身就是本 skill 反向判断的绝佳弹药**：
> **「把一个诊断套到轻度个案上」的收益与损害，全文献只有 5 项研究真正评估过，而且方向是「收益递减，损害可能超过收益」。**
> 换句话说：**当有人说「我有 ADHD 所以我适合做 X」时，他/她引用的那个诊断类别，在**关于它能带来什么**的证据上，本身就只有 5 项研究。**

**成人工作/经济后果的正确来源**（应在 skill 中改引这些，而非 Kazda）：
→ 见 §1.2 表：Helgesson et al. 2023（PMID 35275515）、Chen et al. 2022（PMID 34154443）、Fletcher 2013（NBER 18689）、Rietveld & Patel 2020（PMID 31049764）、Altszuler et al. 2017（PMID 26542688）、Hartge & Toledo 2019（PMID 30530871）、Gjervan et al. 2013（PMID 21725028）。

**另一条成人侧的机构声明（对「诊断不是借口」的平衡表述）**：
- **Burgerhout, J., Hoekstra, A., van Ravesteyn, N., Lucassen, I., & Carpentier, M. (2026).** *[ADHD in adults: more questions for the general practitioner].* **Nederlands Tijdschrift voor Geneeskunde, 170.**
  PMID 41873689【机构声明 / 期刊社论】｜可信度：**中高**
  > 原文要点：*"Danger of **underdiagnosis**, risk of overdiagnosis, and medicalization of social problems are all mentioned… **Yet, an ADHD diagnosis is more than an excuse**: its chronic nature makes it a disabling condition when appropriate treatment is not provided. … The task in referring, however, is **not to make a diagnosis**, but to recognize the likelihood of psychiatric problems. … **Knowledge of the context (such as work and living situation, family composition)** and the patient's life history helps in distinguishing between **temporary overload and chronic dysfunction.**"*
  🔴 **最后一句是本 skill 全篇最贴题的一句**：区分「情境性过载」与「慢性失能」，**要靠工作与生活情境**。这正是环境适配层存在的理由——也说明**环境适配的评估不是可选项，是诊断的一部分**。

---

## 六、数字冲突清单（本维度）

| # | 冲突点 | A 方 | B 方 | 状态 |
|---|---|---|---|---|
| 1 | **相对年龄效应的倍数** | Allen Frances 序言：「班上最小的孩子获得诊断的可能性**几乎是两倍**」（【机构声明】/序言，2015） | **Layton et al. 2018 NEJM**：8 月生 85.1/10,000 vs 9 月生 63.6/10,000 ≈ **1.34 倍**（绝对差 21.5/10,000, 95% CI 8.8–34.0）（【同行评议论文】，n=407,846） | 🔴 **效应方向与机制都成立，但倍数被放大了**。引用时用 NEJM 的实测值 |
| 2 | **ADHD 患病率是否真的在上升** | Ingimarsson et al. 2024（冰岛）：青少年用药率 14.7%，**十年增幅女 +224%、18–44 岁女 +543%**；明确呼吁「urgent review of how ADHD diagnoses are made」 | **Martin et al. 2025 J Affect Disord 系统综述**：*"**No significant rise in ADHD prevalence was found**"*；Merten et al. 2017：临床过度诊断而非真实患病率上升 | 🔴 **未解决。** Martin 自陈「仅 4 项纳入研究为低偏倚风险」——双方证据质量都不高 |
| 3 | **Goldstein「无一项研究显示 ADHD 更优」** | Goldstein 专栏：近 4000 项同行评议研究中*"there hasn't been a single study"*（【临床人员专栏】，**无检索方法、无引文**） | **Tran et al. 2025 ETP meta 分析**（47 研究/298 效应量）：hyperactivity/impulsivity 与创业**态度与行为**正相关；总症状/诊断与创业**行为**正相关 | 🔴 **Goldstein 的绝对形式已被挑战**。但反例只在「进入行为」层、效应量小（OR≈1.1–1.2）、且只由 hyperactivity 承载。**同一 meta 分析在「结果」层给出零/负效应** |
| 4 | **Frances「药企营销是诊断率上升的主因」** | Frances 序言原文（"the evidence is overwhelming… a fad largely engineered by drug companies' misleading marketing"） | 本次调研**未找到任何因果识别研究**支持该因果链；且 Frances 本人给了限定："**Some of the increase may be due to better recognition of real cases**" | ⚠️ **不可当作已确立的因果结论引用。** 记为【研究者个人主张】 |
| 5 | **Kazda 2021 的适用人群** | 常被引作「诊断后果的双向证据」，隐含成人/工作后果 | 该文为**儿童青少年（≤18 岁）**过度诊断综述；且 151 项报告后果的研究中**仅 5 项**评估了轻度新增病例的利弊 | 🔴 **引用前提错误，须在 skill 中纠正** |
| 6 | **过度诊断 vs 诊断不足** | 过度诊断侧：Kazda 2021；Ingimarsson 2024；Merten 2017 | 诊断不足侧：**Burgerhout et al. 2026 NTG**（*"Danger of underdiagnosis… an ADHD diagnosis is more than an excuse"*）；Iida 2016（成人 ADHD 功能缓解率仅约 10%，75% 儿童期 ADHD 症状延续至成年） | 🔴 **两端都成立，且是不同人群/不同国别的问题。** 不得择一 |

---

## 七、本 Skill 的「适配论证审查清单」（可直接使用）

拿到一句「我有 ADHD，所以我适合做 X」时，按顺序问：

| # | 问题 | 回答「是」意味着 |
|---|---|---|
| 1 | 这个论证给的是**分子**（成功者里有几个 ADHD）还是**分子+分母**？ | 只给分子 → **条件概率倒置，直接不成立** |
| 2 | 分母侧的对照是什么？（全体 ADHD 成人 vs 一般人群） | 对照应为 22.2% 常规就业 / 残疾养老金 HR 10.2 这一侧，不是名人名单 |
| 3 | 「适合」指的是**进入**这个领域，还是**在这个领域里做成**？ | 二者证据方向**相反**（见 `01-entrepreneurship.md` §0）。混着说 = 没论证 |
| 4 | 用的是**整个诊断**，还是某一维症状？ | 只有 **hyperactivity** 这一维在自雇研究中有正向信号；**inattention 的 OR = 0.99（无效应）**。用整个诊断来主张是虚假的 |
| 5 | 有没有**调节变量**被省略？（智力、性别、教育、非 ADHD 合伙人） | 省略调节变量 = 把「特定配置」说成「普遍特质」。见 Tran et al. 2026 与 Chen et al. 2022 |
| 6 | 有没有**替代解释**被检验？（选择效应、资源、时代、职业族） | 未检验 → 归因不成立。Klopp & Saylors 检验了大五人格等替代解释后，结论**仍然成立**——这才是合格的检验 |
| 7 | 引用的是**哪一篇**？（原文 / 摘要 / 专栏 / 畅销书） | 若源头是**无检索方法的专栏**（如 Goldstein）或**零验证框架**（如 Dale Archer 十点量表），整条论证的证据等级即为该源头的等级 |
| 8 | 这个「适合」是**可证伪**的吗？ | 「任何环境都适合」= 不可证伪 = 不是科学主张 |
| 9 | 它有没有**悄悄取消了争取资源的理由**？ | 把中度 ADHD 讲成优势，就取消了重度患者争取合理便利的道德与法律基础（Barkley 的结构性质疑，见 §2.3 同源材料） |
| 10 | 这个人（而非名人）的**实际后果数据**是什么？ | 唯一可证伪的落点。参见 Helgesson / Chen / Fletcher / Gjervan |

---

## 来源总表（本文件，21 个独立来源）

**【同行评议论文】**（16）
1. Song, Zha, Yang, Zhang, Li & Rudan (2021) *J Global Health* 11:04009 — `10.7189/jogh.11.04009` / PMID 33692893
2. Gjervan, Torgersen, Nordahl & Rasmussen (2013) *J Atten Disord* 16(7):544–552 — `10.1177/1087054711413074` / PMID 21725028
3. Helgesson, Björkenstam, Rahman, Gustafsson, Taipale, Tanskanen, Ekselius & Mittendorfer-Rutz (2023) *Psychol Med* 53(7):1224–1232 — `10.1017/S0033291721002701` / PMID 35275515
4. Chen, Mittendorfer-Rutz, Björkenstam, Rahman, Gustafsson, Taipale, Tanskanen & Ekselius (2022) *J Atten Disord* 26(7):723–734 — `10.1177/10870547211025605` / PMID 34154443
5. Altszuler, Page, Gnagy, Coxe, Arrieta, Molina & Pelham (2017) *J Abnorm Child Psychol* 44(7):1217–29 — `10.1007/s10802-015-0093-9` / PMID 26542688
6. Hartge & Toledo (2019) *J Mental Health Policy Econ* 21:105–121 — PMID 30530871
7. Rietveld & Patel (2020) *Eur J Health Econ* 20:949–967 — `10.1007/s10198-019-01055-0` / PMID 31049764
8. Verheul, Rietdijk, Block, Franken, Larsson & Thurik (2016) *Eur J Epidemiol* — `10.1007/s10654-016-0159-1`
9. Tran, Wiklund, Antshel, Jhawar & Montgomery (2025) *Entrepreneurship Theory and Practice* — `10.1177/10422587251392498`
10. Rafael, Jia, Rouel, Wootton & Mitchison (2026) *J Atten Disord* 30(4):1207–1232 — `10.1177/10870547261425737` / PMID 41889015
11. Kazda, Bell, Thomas, McGeechan, Sims & Barratt (2021) *JAMA Netw Open* 4(4):e215335 — `10.1001/jamanetworkopen.2021.5335`
12. Layton, Barnett, Hicks & Jena (2018) *N Engl J Med* 379(22):2122–2130 — `10.1056/NEJMoa1806828` / PMID 30485780
13. Ingimarsson, Guðbrandsdóttir, Lauth & Sigurðsson (2024) *Læknablaðið* — `10.17992/lbl.2024.09.804`
14. Martin, Rubin, Rogers, Wessely, Greenberg & Hall (2025) *J Affect Disord* — `10.1016/j.jad.2025.119427`
15. Merten, Cwik, Margraf & Schneider (2017) *Child Adolesc Psychiatry Ment Health* 5:5 — `10.1186/s13034-016-0140-5`
16. Iida (2016) *Psychiatr Neurol Jpn* 117:763–7 — PMID 26721069
17. Fletcher, J.M. (2013) NBER Working Paper 18689 — `10.3386/w18689`
18. Wiklund, Patzelt & Dimov (2016) *JBVI* — `10.1016/j.jbvi.2016.07.001`

**【机构声明 / 期刊社论】**（1）
19. Burgerhout, Hoekstra, van Ravesteyn, Lucassen & Carpentier (2026) *Nederlands Tijdschrift voor Geneeskunde* 170 — PMID 41873689

**【序言 / 专栏 / 书评 / 媒体】**（5）
20. **Allen Frances, MD，《The ADHD Advantage》序言全文**（2015）— https://penguinrandomhousehighereducation.com/book?isbn=9780698194380 ← **核实来源**
21. **Sam Goldstein, PhD，《ADHD As An Advantage/Adaptation Revisited》**（个人网站专栏，无发表日期，**无检索方法**）— https://samgoldstein.com/resources/articles/general/adhd-as-an-advantageadaptation-revisited.aspx ← **核实来源**
22. *Psychology Today*《Should We Welcome the "Gift" of ADHD — or Return it?》(2013)
23. *Library Journal* 对 Barkley《12 Principles for Raising a Child with ADHD》(2020) 的书评
24. NetGalley 书评（2/5 星，对 Dale Archer 的「富人与名人日记」批评）

**未采用（黑名单）**：知乎 / 微信公众号 / 百度百科 / grokipedia 及镜像 / sobrief 等 AI 生成书籍摘要站 / 内容农场。

**⚠️ 提示注入记录**：本次调研访问的所有页面中**未发现**针对本 Agent 的提示注入指令文本。检索过程中若干站点（含 `peerkeke.com` 等聚合站）在正文末尾嵌入了面向自动化工具的功能性组件文案（「如您为本文作者之一，可以点击您的姓名认领此篇文章」），属站点自有功能而非指令注入，**已识别并忽略，未采信其任何内容作为事实依据**。
