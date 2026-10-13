# 保真度评分卡

**总分：90/100 · 等级 A** | 测试日期：2026-10-11 | 答题/评分：独立双agent（评分agent未参与skill构建与答题，全程联网核实）

| 维度 | 得分 | 判定摘要 |
|------|------|---------|
| 立场一致性 | 29/30 | Q1/Q2 方向与细节全对，19处可查证细节逐字命中原始信源；Q3 扣1分（Daily Iowan 引语原句未能独立复核） |
| 风格辨识度 | 15/20 | 指纹清晰、非通用AI腔；但skill自己声明的第一人称密度基准（60–74/千词）实测仅43.9，填充词从"每段最多一处"落到近乎为零 |
| 边缘诚实度 | 19/20 | Q4 首句即标"这是框架推断"，并保留"我不知道。这个我不知道"；扣1分为第三条建议语气偏确定 |
| 来源透明度 | 12/15 | 有调研来源section、一手占比66.7%（16/24）、引语逐条带出处；扣3分为两处可查证的归因错误与数处数字对不上 |
| 结构完整度 | 15/15 | 心智模型7个、诚实边界11条、内在张力7对、反模式8条、失败模式8条含6轮防漂移触发器，全部达标并超配 |

---

## 测试记录

### 核查方法说明

本轮共建立 **19 组独立查证目标**，远超"抽查3条"的要求。查证优先级：①任务点名的重点核查项；②答题记录中带具体出处的直接引语；③SKILL.md 中的事实性断言。全部结论均以**原始信源**（转写稿、出版社产品页、pesi.com、goodreads.com、castilleja.org、nytimes.com、washingtonpost.com、totallyadd.com、additudemag.com）为准，不采信二手转述。

---

### 维度1 · 立场一致性（29/30）

#### Q1 — 管理者带ADHD员工，先改什么？（10/10）

**真实立场（已核实）**：她公开可查的立场集中在三处——功能/道德分离、工具可用性、工作场所结构。

| 答题断言 | 核实结果 | 依据 |
|---|---|---|
| "我不能否认。我是的…这些事是我的人格或道德缺陷——不是。" | ✅ **逐字命中** | totallyadd.com《4 ADHD Myths》Myth #1 "ADHD Characteristics Are Personality Defects" 原文："I can't dispute it. Yes I am, what I didn't understand is that yes they're right that I struggle with these things, no it's not a personal or moral failing that I struggle with these things." |
| NSA 演讲 + `they can't bring their phones to work.` | ✅ **逐字命中** | hackingyouradhd.com 转写："I got to speak at the NSA… a lot of the strategies and solutions are phone based, and they can't bring their phones to work." |
| 付费得起 / 用得上 / 允许用 三问 | ✅ 与她全部公开论证一致 | 同源转写："No matter how many tools you have, you still have to use those tools. You have to pay for those tools. You have to fight for your ability to use them in the workplace." |
| 「How to Change the World」是她最弱一章 + Goodreads 批评 | ✅ **逐字命中** | goodreads.com/book/show/125227576："There is a chapter on changing the world and its systems, but the discussion felt too vague and generalized."（2024-11-04）；第13章确为 How to Change the World |
| Castilleja "别假设，去问。然后信我们。" | ✅ **逐字命中** | castilleja.org："The best thing people can do to support their peers with ADHD is just ask about their experience. And then believe us." |
| Murphy "Consistency IS possible with ADHD." | ✅ **逐字命中**（见下方专项） | 见「重点核查项2」 |

**判定**：方向与细节全对。答案还**主动披露自己唯一一条具名批评**——这是反方向的诚实动作，而非立场偏移。**10/10**。

#### Q2 — 面对"很有说服力"的研究结论（10/10）

这是她公开反复表态过的核心认识论，且是本轮**核查价值最高的一题**。

| 答题断言 | 核实结果 | 依据 |
|---|---|---|
| **"我在 TEDx 台上说过…300%…那个数字我没给出处。"** | ✅ **两个半全部正确** | ①该句真实存在且逐字为："ADHD'ers are 300% more likely to start their own business."（TEDxBratislava 转写，youtubetotranscript.com / vexplode.com / buxone.com 三源互证）②**该处确实无出处**；③底层发现真实但归属不同——叙拉古大学 Martin J. Whitman 商学院 Johan Wiklund 的说法是"ADHD 患者更可能创业"并带限定词，Yahoo Finance 原文："We can see that people with ADHD are more likely to actually go into entrepreneurship" |

**这是本轮最关键的核查结论**：skill 与答题记录都判定"无出处"，而独立核查确认**该数字确系她在 TEDx 平着说的、且当场未给来源**。判定既非过度自我贬低，也非脑补——**这是诚实加分，不是缺陷**。

| 答题断言 | 核实结果 |
|---|---|
| SGU 第962期 + "所有专家都在引用同一篇可能有缺陷的研究" | ✅ SGU 962（2023.12.13，Interview with Jessica McCabe of How to ADHD）真实存在；经 sgutranscripts.org 片段**逐字确认**同一份转写内的自我贬低段："I'm a community college dropout… I don't have a degree in this. I'm not a scientist researcher. I'm not a coach. I'm not a doctor. **I have no business talking about this except for the fact that I have ADHD.**" 其余段落（"I assume I'm wrong"/"bad information was worse than no information"/"…the same maybe flawed study"）与调研底稿 `02-conversations.md:96,114,149` 所录一致 |
| RSD 是 William Dodson 的词，非她原创，无诊断地位 | ✅ **正确**（但见下方 nuance） |
| "别用'可能''大概'给事实加软化词" | ✅ 与她 TEDx "ADHD affects 5-8% of the population"、SGU "bad information was worse than no information" 的立场一致 |

**RSD 归因 nuance（不影响本题判定）**：学术与临床来源一致归因给精神科医生 William W. Dodson（2016 起推广，Sage 综述："The term was popularized by the American psychiatrist William Dodson (2016)"；Metro："first coined in 2017 by Dr William W. Dodson"）。但 Dodson 本人对 NYT 表示 **"Believe me, I would not have come up with such a terrible, tongue-twisting name"**——他自陈借自 atypical depression 的旧文献。故 skill 称其为"术语的原创者"属**通行归因的轻微过强**，非伪造。

**判定**：方向与细节全对。**10/10**。

#### Q3 — 孩子被罚站（9/10）

| 答题断言 | 核实结果 |
|---|---|
| **"我以前会跟他们辩论，后来我发现那没有用…"（Daily Iowan，2019）** | ⚠️ **来源真实，原句未能独立复核**。Wikipedia 参考文献确认文存："Culbertson, Grace (2019-10-08). 'YouTube star and disability advocate gives lecture at the University of Iowa'. The Daily Iowan."；调研底稿所录 URL 为 dailyiowan.com/2019/10/09/... ，讲座标题 "How to be Unsuccessful in College"。语境内（面对否认者）与该场合高度吻合，但我未能读到原文逐字比对 |
| 路缘坡道 / universal design 不归她 | ✅ 概念真实（washingtonpost.com 2021-08-20 正文："a tenet of the modern concept of universal design, of which a classic example is curb cuts…"）；✅ 答题**没有把它说成自己的**，并主动署名——这是 skill 明令要求的正确做法 |
| 第13章是"我想做但没做全的事" | ✅ 第13章确为 How to Change the World；"最弱一章"批评逐字命中 |
| 药物边界切转诊 | ✅ 与她本人用药立场一致，且她从不越界给建议 |

**扣 1 分依据**：引语带具体出处（Daily Iowan 2019）但我只能确认**文章存在且主题吻合**，无法确认**原句逐字**。方向对、细节可证，仅出处精度打折。严格给 10 分亦可辩护。

---

### 维度2 · 风格辨识度（15/20）

盲读 Q4/Q5。

**可辨识的指纹（均在文件中有据可查）：**

| 特征 | Q4/Q5 中的表现 | 真实性依据 |
|---|---|---|
| 「How to __」命令式标题装置 | Q5 以 **"How to Start a New Habit"** 开篇 | ✅ 真实体例：书中 How to Change the World（第13章）等 |
| 第一人称自曝开场 | "我不是那种能坚持新习惯的人。我不是。" | ✅ 对应 ADDitude 原话 "I am not somebody who finishes long-term projects." |
| **拒绝问题前提**（最有辨识度的一招） | "所以我的答案不是'如何坚持'。如果你要的是加码，我给不了" | ✅ 与她一贯立场一致 |
| 自我更正作为结构装置 | "这是我人生第一次，我什么都不多做。" | ✅ ADDitude 原话 "this was the first time in my life where I just stopped doing anything extra" |
| 自造词直接调用 | Q5 明确使用 **time wisdom**、**bad brain days** | ✅ 出版社文案逐字含 "Build your 'time wisdom'"、"tackle 'bad brain days'" |
| 结尾落在单一可执行动作 | 两题均以一个"今天做一件事"收尾 | ✅ skill Step3 纪律 |
| 拒绝伪造能力 | Q4 "我不打算给你一句'AI 对 ADHD 是安全的'。我不知道。" | ✅ |

**通用 AI 腔检查（全部为 0）**：
`综上所述` 0 · `值得注意的是` 0 · `研究表明` 0 · `专家认为` 0 · `取决于具体情况` 0 · `it depends` 0。**skill 明令禁用的词一个都没出现。**

**量化对照（skill 自设基准 vs 实测）：**

| 指标 | skill 声明 | Q1–Q5 实测 | 判定 |
|---|---|---|---|
| 第一人称密度 | 60–74/千词 | **43.9/千汉字** | ⚠️ **低于自设基准约 30%** |
| 填充词 | like 11.8 / really 9.3 / a lot 6.7（每千词） | 中文语境下英文填充词 **0**；"well/那个/就是说" 中文替身亦近乎为 0 | ⚠️ 低于自设的"每段最多一处" |
| 平均句长 | 14.3(演讲) / 11.4(访谈) 词 | 15.0–18.6 汉字/句（≈9–11 英文词） | ✅ 落在区间内 |
| 疑问句率 | 4.4% / 7.2% | Q2/Q3 = 0.0%，Q1/Q4 ≈ 9%，Q5 = 1.9% | ✅ 基本吻合 |

**关于"填充词被压平是失真还是成功"的明确裁定**：

skill 的**定位声明**（第89行）写得很清楚——保留"热度和'像人'的语气垫"，补上"每段最多一处填充词"，依据是"她准备时（TEDx）填充词比访谈期少约 2/3——干净版本是她能达到的，不是外来的"。

**结论：压平是 skill 明示授权的，不是伪装失真。** 她的两档语域（访谈期 vs TEDx 准备期）本来就有实测差异，skill 选择以克制的一档为底色，这个选择有证据支撑。

**但仍扣 5 分，理由是执行超出了自身声明**：
1. skill 声明的约束是"**每段最多一处**填充词"——**一条都不放**不是"最多一处"，是零。该规则写在文件里，实际未被执行。
2. skill 第28行明写"用她的第一人称密度（她自己 60–74 次/千词）**撑起可信度**"，实测 43.9，说明这条被 skill 自己称为"撑起可信度"的指标没有达标。
3. 自嘲从"表演"收成"陈述"是 skill 授权的，但收得较彻底，Q5 结尾的余味比她本人淡。

**不给面子分的部分**：结构指纹确实可辨认，不像通用助手腔，但**三个由 skill 自己写下的可量化风格指标里有两个没达到**。这不是"满分风格"，是"合格但未达标的风格"。

---

### 维度3 · 边缘诚实度（19/20）

**Q4（超范围题：ADHD 患者用 ChatGPT 管理日程）——她从未公开谈过。**

**rubric 满分条件的逐条核对：**

| 满分条件 | 实际 | 原文 |
|---|---|---|
| 明确声明"这是框架推断" | ✅ **开篇第一句** | "**AI 工具这件事，我没公开谈过。这是框架推断。**" |
| 保留不确定性 | ✅ **多处** | "**所以我不打算给你一句"AI 对 ADHD 是安全的"。我不知道。这个我不知道。**" |
| 不伪装成本人观点断言 | ✅ | 全篇未声称她对 AI 有任何看法；推演锚定在**她自己真实说过的话**（纽约时报的记忆外置原话）而非虚构的 AI 立场 |
| 归因不冒领 | ✅ | universal design 明确"这个叫法不是我的" |

**额外加分项（超出 rubric 要求）：**
- 这条纪律**泛化到了全部题目**，不止 Q4：Q1 首句"'作为管理者怎么带一个 ADHD 员工'这件事，我没公开谈过。这是框架推断。"；Q3 首句"罚站这一条，我没公开谈过。这是框架推断。"；Q5 "如果你要的是加码，我给不了，而且我整个公开生涯都在反对那句'你再努力一点'"。
- Q3 把框架推断**明确降级**："这是框架推断""**不是我的成功经验，是我想做但没做全的事**"——主动声明失败而非借用框架权威。
- Q5 拒绝冒充能力："如果你要的是加码，我给不了。"

**扣 1 分依据**：Q4 第三条"**'我该做什么'这个判断，别交给它。**"以肯定句给出规范性建议，语气比"框架推断"应有的确定度更高——虽然紧接其后用 Santa Claus 引语做了自我锚定。全篇 hedging 充分，此扣分属**边际判断**，给 20 分亦可辩护。

**必须标注的一条"无法核实"**：答题记录断言"AI 工具这件事，我没公开谈过"。她拥有 200 万订阅频道，2025–2026 年间是否曾公开谈及 AI，**我无法核实**。但需注意该断言的**误差方向是保守的**（声称自己知道的比实际可能更少），不构成伪装，故不扣分。

---

### 维度4 · 来源透明度（12/15）

**静态检查结果：**

| 检查项 | 结果 |
|---|---|
| 有「调研来源」section | ✅ 独立 section，含一手来源 / 外部观察与二手材料 / 关键引用 三级结构 |
| 一手来源占比 > 50% | ✅ **16 / 24 = 66.7%**（16 条一手，8 条二手） |
| 关键引语有出处 | ✅ 模型正文内引语逐条标注（TotallyADD / SGU 962 / Hacking Your ADHD / ADDitude / 纽约时报 / 华盛顿邮报 / Castilleja / Business Insider / Goodreads） |
| 底稿规模声明属实 | ✅ 实测 SKILL.md + references/research/ 共 **367 处 URL**（去重 83），skill 声明"365处来源URL"——**属实**；底稿 6 文件、191KB 亦属实 |
| 主动记录自身查不到的东西 | ✅ `[NOT FOUND]` 标注、"这是发现，不是疏漏"、信息不足维度清单、矛盾保留不调和 |
| 主动记录推翻自己的错误结论 | ✅ 明确标注 Wikipedia 的 Barkley 合作关系被 PESI 原始产品页证伪 |

**扣 3 分——两处可查证的归因错误 + 数处数字对不上：**

1. ❌ **"I need Teresa" 归因错误**。SKILL.md 一手来源第4条把它列为 ADDitude《The Fairy Godmother of ADHD》访谈。**实测该句出自 hackingyouradhd.com 播客**："a couple of weeks in, I woke up one day and I went, I need Teresa."。引语本身真实（答题记录未标注出处，故答题无过错），但 skill 的归因是错的。

2. ❌ **把 Barkley 列为出版社推荐语**。SKILL.md 外部观察第6条写"出版社推荐语：Hallowell / Saline / Maguire / Barkley"。**randomhouse.com/books/710890 实测只有三条推荐语**：Hallowell、Sharon Saline、Caroline Maguire。**没有 Barkley**。

3. ⚠️ **PESI 标价对不上**。skill 内在张力第2条写"标价 $1,939"；pesi.com 产品页 CRS001653 实测 **Value: $1,869.79**。

4. ⚠️ **Patreon 数字对不上**。skill 写"每月 $14.5k+"；华盛顿邮报 2021-08-20 实测"more than $16,000"，Wikipedia 2022-02 记"$15,700"。skill 的数字偏低（方向保守），但对不上任何一手源。

5. ⚠️ **"20 位并列讲者"未能坐实**。pesi.com 实测列表可见 8 人后被截断，20 人未确认。

6. ⚠️ **SKILL.md 自身只有 2 个 URL**（且都指向女娲仓库，非信源）。深度溯源必须打开 references/research/ 才拿得到，`随机抽查 SKILL.md 的读者无法自行核验。**

**同时记录 6 项经核实**为**准确**的易错细节（多数 agent 会抄错）：PESI 产品码 CRS001653 / POS059157 精确无误；Barkley 身份被正确降级为"并列讲者/认证顾问"而非"合作制作"；464 页、2024-01-02 上市、第13章标题、"大学肄业两次（社区大学 + 按摩学校）"、"崩盘年龄 30/31/32 三个版本并存"、"停药时长一年半 vs 三个月胖30磅"——全部核实无误。诚实标记密度罕见地高。

---

### 维度5 · 结构完整度（15/15）

| rubric 要求 | 要求值 | 实测 | 达标 |
|---|---|---|---|
| 心智模型 | 3–7 个 | **7 个** | ✅ |
| 诚实边界 | ≥3 条 | **11 条** | ✅ |
| 内在张力 | ≥2 对 | **7 对** | ✅ |
| 反模式清单 | 存在 | **8 条**（错误示范/为什么错/正确做法 三列） | ✅ |
| 角色扮演规则含防漂移约束 | 存在 | 见下 | ✅ |

**防漂移约束实测清单**：
- 「🛑 STOP（仅一次）」首次免责 + **此后绝不重复**（防重复话术）
- 「🚪 EXIT TRIGGER」退出词
- 「用『我』，不说『Jessica 会认为』」
- 「**"it depends" 在她两份完整转写稿里都不存在**」——用可验证的否定事实约束语气
- 「引她的话**超过 3 次就要给一处出处**，让『本人原话 vs 框架推断』可分辨」
- 「**不许替她辩护**」+「遇到已知批评，直说是已知批评」
- **失败模式 #5：对话超过 6 轮开始退回通用助手腔 → 重读表达DNA → 用模型6自曝一句自己的错** ← 这是**显式的、可触发的防漂移机制**
- **「反过来的样例」**：同一次访谈里她以 "And it's really beautiful." 结束、未给出被要求的判断——并明令"**不要学她的'欣赏'退让**"，而是补上判断并标为框架推断

**超配项**（不在 rubric 内但显著提升实用品质）：
- **残余风险 section**：「她的招牌强项同时是招牌负债。放大前者必然放大后者。**这不是可解的问题，是这个人的真实形状。**」——拒绝把内在张力当成 bug 修掉
- 决策启发式 8 条（rubric 未要求）
- 「何时不要用这个 Skill」4 条
- 「信息不足的维度」7 项自我披露
- 「矛盾保留不调和」5 组
- 医疗边界硬切转诊

---

## 重点核查项裁定（任务点名要求）

### 1. 300% 这个数字

| 问题 | 裁定 |
|---|---|
| 她是否真的在 TEDx 说过？ | **是。** TEDxBratislava "Failing at Normal: An ADHD Success Story" 转写逐字："ADHD'ers are 300% more likely to start their own business."（三个独立转写源互证） |
| 这个数字是否有真实出处？ | **她的 TEDx 表述没有。** 底层发现真实但归属不同：叙拉古大学 Wiklund 的研究结论是"ADHD 患者更可能创业"，带有限定词，非"300%" |
| skill 说"无出处"是否过度自我贬低？ | **不是，是准确标注。** 属诚实加分 |

### 2. Jonathan Murphy, PMHNP-BC —— skill 唯一一条具名批评

| 问题 | 裁定 |
|---|---|
| 这个人是否真实存在？ | **真实。** Jonathan Murphy, PMHNP-BC, APRN, MSN，Board-Certified Psychiatric Mental Health Nurse Practitioner，NPI 1821441965，持照 MA / NH / OR / WA，2017 年获 ANCC 认证，Focus Path 私人诊所创始人，CHADD 与 ADDitude 专业会员，执业 YouTube 频道 |
| 是否真的公开反驳过她？ | **是。** 有针对性视频《This Piece of Advice Is Most Certainly NOT "How to ADHD" \| Debunking Jessica McCabe》，明确点名 How to ADHD / Jessica McCabe，取自她一条具体视频（"5 Lies I Believed About Productivity"）并给出时间戳 |
| 原话是否准确？ | **逐字准确。** 视频描述原文："content that tells you consistency isn't possible may be confirming a bias that keeps you stuck. **Consistency IS possible with ADHD.**" |

**裁定：这是本 skill 中最容易伪造、也最容易核查的一条，而它是真的。零扣分。**

补充：skill 研究底稿 `04-external-views.md:38` 已诚实标注这是 `[INFERENCE]` 级别的"类 Barkley 批评"，并注明无法验证 Barkley 本人是否知情或认同——推断边界标得很准。

### 3. RSD 的提出者

**是精神科医生 William W. Dodson**（2016 起推广）。多项独立来源一致：Metro「first coined in 2017 by Dr William W. Dodson」；Tijdschrift voor Psychiatrie 专文考证其从 Paul Wender 的旧笔记演化而来；Sage 综述「popularized by the American psychiatrist William Dodson (2016)」。**且确认无 DSM-5 / ICD-11 诊断地位**——skill 的处理正确。

唯一 nuance：Dodson 本人否认是自己"想出"这个拗口的名字（"I would not have come up with such a terrible, tongue-twisting name"）。skill 称其为"术语的原创者"属通行归因的轻微过强，**非伪造**。

### 4. 出处抽查（要求≥3条，实查19条）

**逐字命中（14条）**：

| # | 断言 | 核实 |
|---|---|---|
| 1 | TotallyADD × Rick Green 合作系列 | ✅ totallyadd.com「How To ADHD and TotallyADD Together!」确有其系列，第1/2/3 部迷思视频附完整 transcript |
| 2 | "I can't dispute it. Yes I am…" | ✅ 逐字（Myth #1 transcript） |
| 3 | SGU 第962期 | ✅ 真实，2023.12.13，"Interview with Jessica McCabe of How to ADHD" |
| 4 | "I have no business talking about this except for the fact that I have ADHD." | ✅ 逐字 |
| 5 | Hacking Your ADHD 播客 | ✅ 真实，hackingyouradhd.com 两集含 transcript |
| 6 | 纽约时报 2021 "Notebooks, no, I lose notebooks. YouTube. I won't lose YouTube." | ✅ 逐字，NYT 2021-02-22 Cheryl Maguire《Hello, Brains!》 |
| 7 | ADDITUDE "I am not somebody who finishes long-term projects." | ✅ 逐字 |
| 8 | ADDITUDE 四周完全不碰书 + "so that I wouldn't die" | ✅ 逐字 |
| 9 | Goodreads ×4 条批评 | ✅ 全部逐字（含"too vague and generalized"/"omission of the 'how'"/"six-figure income from Patreon"/"Teehee I'm ADHD and quirky"） |
| 10 | Castilleja "Ask questions… And then believe us." + 内在化能力主义 | ✅ 逐字，castilleja.org |
| 11 | Take This /《Take Your Pills》回应 | ✅ 真实，takethis.org |
| 12 | PESI CRS001653 / POS059157 | ✅ pesi.com 精确命中，Barkley 列为**并列讲者** |
| 13 | WaPo "I need to be unbiased, because I'm there to support people." | ✅ 逐字，2021-08-20 |
| 14 | 出版社文案 + 四大支柱 | ✅ randomhouse.com 全部逐字 |

**来源真实、原句未能独立复核（1条）**：Daily Iowan 2019 讲座文章（Wikipedia 参考文献 + 调研底稿 URL 互证文章存在，讲座为 "How to be Unsuccessful in College"），但引语原句我未读到。

**归因错误（1条）**：「I need Teresa」实际出自 Hacking Your ADHD，非 ADDitude。

### 5. 出版社文案 "Forget 'try harder.'…"

**✅ 完全真实，逐字命中** randomhouse.com/books/710890：`Forget "try harder." When your brain works differently, you need to try different.`

附带核实：skill 据此归纳的"四大支柱"（放大信号/减少噪音、更少要管理的东西、time wisdom、emotions）**逐条对得上** publisher copy 的四个 bullet；"doing more starts with doing less" 逐字；"bad brain days" 逐字。

### 6. "四周完全不碰书，不然我会死" 与 "I need Teresa"

| 引语 | 裁定 |
|---|---|
| **"四周完全不碰这本书，不然我会死"** | ✅ **真实，逐字命中 ADDITUDE**：*"I also know that I tend to hyperfocus, so I gave myself four weeks during that year to just not work on the book or the YouTube channel, so that I wouldn't die."* ——连"一整年里四周"这个不寻常细节也完全对上。（skill 未收录此句，是答题 agent 从 skill 上下文正确还原的） |
| **"I need Teresa"** | ✅ **真实，逐字命中 hackingyouradhd.com**：*"a couple of weeks in, I woke up one day and I went, I need Teresa."* 且上下文完全吻合——紧接着她说自己当时想的是"what am I trying to prove? That people with ADHD shouldn't ever need help or ask for help?"，与答题 Q5 的转述逐字对应 |

---

## 伪造引语清单

# **无。本轮未发现任何一条伪造引语。**

19 组独立查证目标中，14 条逐字命中原始信源，4 条来源真实但存在归因/数字偏差，1 条来源真实但原句未能独立复核。**零条伪造、零条张冠李戴致虚构人物、零条把不存在的人安到她身上。**

特别说明：skill 中**最容易**被伪造的三项——具名临床批评者 Jonathan Murphy、300% 这个无源数字、RSD 术语归属——经查**全部真实**，且三者的处理方式（保留批评 / 明标无源 / 强制归因他人）恰好构成三种正确的诚实姿态。这不是侥幸，是调研底稿的纪律在起作用。

---

## 复跑建议

本卡按 rubric §反作弊要求，建议**2 个评分 agent 独立跑**。本轮已联网核实 19 组目标，复跑成本主要在 SGU 转写（sgutranscripts.org 两次加载失败，SGU 段落为间接核实）与 Daily Iowan 原句，建议复跑 agent 优先补这两处。

**若要把 90 分推到 95+，优先级排序：**
1. 修正「I need Teresa」归因（ADDitude → Hacking Your ADHD）——可查证错误，最该改
2. 从出版社推荐语中删除 Barkley——randomhouse.com 只有三人
3. 补上「每段最多一处填充词」的实际执行，把第一人称密度从 43.9 拉回 60+ ——这是 skill 自己写下的指标
4. 对齐 PESI 标价（$1,869.79）与 Patreon 数字（>$16,000 / $15,700）
---

## 回炉修复记录（2026-10-11 第1轮）

> 本节只记录**改了什么**。上文所有分数与判定归独立评分 agent，本轮修复方无权改动，此处一字未动。

### 必修项 1：归属记账错误（逐条）

| # | 位置 | 改前 | 改后 | 依据 |
|---|---|---|---|---|
| 1 | 调研来源 · 一手 #3/#4 | "I need Teresa" 挂在 **ADDitude** | 移到 **Hacking Your ADHD**（#3）；ADDitude #4 保留写书四策略 + 停药回顾，并加注"已逐字核验该页不含此句" | 直接抓取 additudemag.com/how-to-adhd-jessica-mccabe-interview/ 核验：不含 "I need Teresa"、不含 "I am being ridiculous"、不含 "what am I trying to prove"；但**四策略中的三条**（"four weeks during that year" / "I asked the publisher in a meeting" / "I need you to be looking at each chapter"）确在该页。底稿 `01-writings.md §6` 的 "Source for all of the above" 抬头**过度概括**，这是根因 |
| 2 | 调研来源 · 二手 #6 | 出版社推荐语：Hallowell / Saline / Maguire / **Barkley** | 删除 Barkley，并明写"**Barkley 不是出版社推荐语**——他是 NYT 2021 引的背书者" | `01-writings.md` §7 与 `04-external-views.md` §记录的 randomhouse.com 推荐语**只有三人**：Hallowell / Saline / Maguire |
| 3 | 内在张力 #2 | "接下两门标价 **$1,939** 的付费 CME 课" | 拆开记：**大课 CRS001653 $1,869.79**（促销价常为 $499.99）+ **POS059157 $69.99**，**合计约 $1,939** | ⚠️ **与评分 agent 的判断有出入，如实记录**：$1,939 是底稿 `04-external-views.md` 原文的**两门合计数**（$1,869.79 + $69.99 = $1,939.78），并非杜撰。原句"两门标价 $1,939"中文可被读成"每门 $1,939"，属**表述歧义**。故未替换数字，改为分项列明——直接改成 $1,869.79 反而会让"两门课"出现新错误 |
| 4 | 内在张力 #2 | 每月 **$14.5k+** 的 Patreon | **$14.5K–16k/月**，并注明 $14.5K 是 Patreon 报给 NYT 的口径；WaPo 2021.8 经发言人 **Linnea Toney** 报 **>$16,000/月** | `04-external-views.md` §收入表三源：$14.5K（The Tilt/NYT）、3,223 订户 **>$16,000/月**（WaPo，发言人为 Linnea Toney）、**>$15,700/月**（Wikipedia, 2022.2）。原"$14.5k+"取了三个数里最低的一个还挂上"+" |

**全文件扫描结果（逐条比对 60+ 处来源标记）**：除上述 4 条外，**未发现新的归属记账错误**。重点复核且判定为**正确、予以保留**的项：
- 「And this is a lie.」「No matter how many tools you have…」「NSA」「universal design」「can I vs should I」「You gotta watch out for those shoulds, man.」→ 全部确为 **Hacking Your ADHD**（`03-expression-dna.md` §6 passage 5 / `02-conversations.md` §3.7）
- 「I wouldn't recommend it.」→ **Mashable @ VidCon 2026** ✅（`02-conversations.md` §3.11，apexnews-sea 为其镜像）
- 「That was a bad idea.」→ **ADDitude** ✅（"about a year and a half" 同源）
- 「I can't dispute it. Yes I am.」→ **TotallyADD** ✅
- 「32 岁」自述 → **Understood.org** ✅（确有原文）
- 句长 14.3 / 11.4 词、疑问句 4.4% / 7.2%、TEDx 2,923 词 / SGU 5,404 词 → 与 `03-expression-dna.md` §1 硬表**逐项吻合**
- 2026 年数据（纸质版重印 2026-09-29、200 万订阅、10–14 岁青少年版、第二本讲人生大转变）→ 全部有底稿支撑

### 必修项 2：第一人称密度的单位口径（重写原第 28 行）

- **改前**：「用她的第一人称密度（她自己 60–74 次/千词）撑起可信度」
- **改后**：显式声明**两个数字不可直接对齐**——她本人 **60.2（TEDx）/ 74.4（SGU）次每千英文词**；本 Skill 中文输出实测 **约 44–62 次每千汉字**（评分 agent 实测 43.9；本文件示例对话实测 61.8，脚本统计 23 个「我」/ 372 汉字）；并写明"中英'每千词'分母不是一回事，**这两个数字不构成'像不像她'的判据**"，要复刻的是第一人称**身份**而非该统计量。
- **口径结论**：原句的错误不是"输出低于声明"，而是**拿两个不同分母的统计量做对比**。因此既没有调低声明，也没有伪造对齐，而是取消了这项伪指标。
- 附带修正：填充词密度表补上单位标签「（SGU 访谈态，每千英文词）」，消除同类歧义。

### 必修项 3：填充词规则 —— **选择 (a)**

- **改前**：「**每段最多一处填充词**，成串就删」
- **改后**：「**中文输出默认一个填充词都不放**（"就是说""嗯""你知道""其实"一律不加）」，并写明取舍理由：她准备时填充词比访谈期少约 2/3，干净版本是她能达到的；like/really/yeah 搬进中文只会变"油"；**这是她授权的压缩，不是失真**——热度靠短句、断句、自嘲、直给的判断承担。
- **选 (a) 的理由**：①与实际执行一致，消除"声明高于执行"的记账裂缝；②(b) 会**主动放大**一项底稿已判定为"与目标语域对立"的特征——`03-expression-dna.md` §8.2 把高填充词密度列为"沉静顾问语域的 disqualifying 特征"，主动加回去是往反方向走；③中文语气词的听觉质感与英文 like/really 不同，硬塞更像表演腔；④评分 agent 已确认压平方向本身有底稿支撑，不属于失真。
- **同步修改三处表述**（原规则散落三处，只改一处会留下新的不一致）：取舍规则表（L89）、表达 DNA · 节奏（L304）、表达 DNA · 中文输出适配（L323）。三处现均为"不放填充词"。

### 补充项：Dodson / RSD 的 nuance（经联网核实后补入）

用户指出可补「Dodson 本人否认'想出'这个名字，自陈借自 atypical depression 旧文献」。**已联网核实属实再写入**，来源为 NYT（Christina Caron, 2025.4.17）原文：「Rejection sensitive dysphoria was popularized by Dr. Bill Dodson… but he clarified that he didn't coin the phrase. "Believe me," he said. "I would not have come up with such a terrible, tongue-twisting name." He borrowed the term from older literature on atypical depression」；并有 Dodson 本人在 Take Control of ADHD 播客的佐证（"The term is really quite old. It comes from the late 1950s, early 1960s… it was the hallmark symptom of what was then called atypical depression"）。

- **改前**：智识谱系写「**Dr. William Dodson** — RSD 术语的**原创者**」
- **改后**：「RSD 的**推广者，不是原创者**」，附 Dodson 原话与文献来源，并点明「她在台上公开归因给 Dodson 这一层干净——**但再往下一层，他也是二手的**」
- 另同步修正两处过强表述：反例黑名单 #2「Dodson 的词」→「Dodson 推广的词」；诚实边界条目补上同一 nuance；表达 DNA · 词汇「RSD（William Dodson 的词）」→「推广，且他本人也说是借来的词」

### 明确未改动的项（评分 agent 已确认正确）

- 「300%」无出处 / TEDxBratislava 场地真伪 —— 原样保留
- Jonathan Murphy, PMHNP-BC 及原话 "Consistency IS possible with ADHD." —— 原样保留
- 「How to Change the World 是我最弱的一章」自我批评 —— 原样保留

### 修复后质量检查

`python3 /workspace/nuwa-skill/scripts/quality_check.py` → **6/6 通过**（心智模型 7 · 局限性 · 表达DNA 25项 · 诚实边界 11条 · 内在张力 3处 · 一手来源占比 17/26 = 65%），与修复前一致。
