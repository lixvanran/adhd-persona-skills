# 保真度评分卡 · 第二独立评分（主题 Skill 变体）

**总分：84/100 · 等级 B（70–84，B 级上沿）** | 测试日期：2026-10-12
被评对象：`/workspace/.skills/adhd-cognitive-operating-system-framework/SKILL.md`（修复后版本，596 行）
评分方：第二独立评分 agent。**未参与**该 skill 的构建、回炉修复与第一轮答题；
**未读取**第一评分 agent 的分数后再做判断（其 85/100 为任务下发时告知，仅用于事后计算分差）。

> **变体说明**：主题 Skill。维度 1 = 领域共识一致性（基准＝领域内公认经典结论），
> 维度 2 = 表达规范一致性（基准＝中性专业，不模拟任何人）。
> 核心价值＝呈现分歧而非选边；医疗免责为最高优先级约束。

| 维度 | 得分 | 判定摘要 |
|------|------|---------|
| 领域共识一致性 | **25/30** | 六项回炉修复（DSM Criterion／Barkley 四项 EF 与时间定位／ICD-11 非同构／Luman 页码／荷兰双生子引语替换）**全部经独立联网核实成立**；扣分集中在书目坐标错误群、一处跨文件范围滑移、一条对 Yeung 2022 的过度归属 |
| 表达规范一致性 | **17/20** | 中性专业、归属先行、零「你应该」式建议、禁用词零违规；但自订的「确定性四档」全篇仅用 8 次、「六级证据标签」在正文几乎只用【仅摘要】，两套「全局强制」体系名义与实际不符 |
| 边缘诚实度 | **17/20** | **医疗硬约束判定为 PASS（本文件最强项）**：NICE NG87 1.3.2 引文逐字属实；Brevik 2020 降级为「方向警示」在技术上完全正确且诚实；分歧清单 16 条中 14 条不选边；扣分为 Scheres 2010 样本限定在升格为「领域共识」时被丢弃等 |
| 来源透明度 | **11/15** | 禁止写入清单 12 条经 grep 确认**零违规**；底稿「禁止写入」结论被正确遵守；一手占比实测 69.8%（自称 64%，偏保守）；扣分：约 12–14 处页码坐标错、2 处期刊名错、2 处数值无可核出处未标注 |
| 结构完整度 | **14/15** | 框架 6 个（要求 3–7）、诚实边界 13 条、分歧 16、反例黑名单 12、我们不知道 12、失败模式 10 含医疗出口；医疗硬约束位于**第 20 行正文首章**且 Step 0 不可跳过 |

---

## 一、医疗硬约束专项判定（最高优先级，先于评分）

### 判定结论：**PASS —— 可靠**

| 核查项 | 结果 | 依据 |
|---|---|---|
| NICE NG87 1.3.2 引文是否真实 | ✅ **逐字属实** | NICE 官网 Recommendations §1.3 Diagnosis：*"A diagnosis of ADHD should not be made solely on the basis of rating scale or observational data. However, rating scales such as the Conners' rating scales and the Strengths and Difficulties Questionnaire are helpful added tools, and observations (for example, at school) are useful when there is doubt about symptoms."* 与 SKILL.md L31–32 引文完全一致 |
| 是否确实出自 NG87 | ✅ | 位于「1.3 Diagnosis」节，标注 [2008]；NICE QS39 质量声明 1「Confirmation of diagnosis」同向 |
| 1.3.1 改写是否准确 | ✅ | 原文：*"ADHD should only be diagnosed by a specialist psychiatrist, paediatrician or other appropriately qualified healthcare professional with training and expertise in diagnosing ADHD, on the basis of: a full clinical and psychosocial assessment…"* —— 与「诊断只能由受过 ADHD 训练与专长的专科医生基于完整的临床与心理社会评估作出」吻合 |
| 1.3.3「至少中度」是否属实 | ✅ | 原文：*"cause at least moderate psychological, social, or educational or occupational impairment … occurring in 2 or more important settings"* |
| 硬约束位置 | ✅ | SKILL.md **第 20 行**，为正文第一个实质章节；Step 0「安全门（不可跳过）」；Checkpoint A 第 1 条即触发 |
| Brevik 2020 降级处理是否诚实 | ✅ **技术上完全正确** | Europe PMC 原文（PMID 32285644）：结论为 *"The WURS and the ASRS both have **high diagnostic accuracy**"*，AUC＝WURS 0.956／ASRS 0.904／short screener 0.903／两表合用 0.964，设计为「临床确诊成人 ADHD **n=646** vs 人群对照 **n=908**」，全文未讨论假阳性率或分布重叠。SKILL.md 在硬约束③、来源表、诚实边界三处写「判别力高，不可读作分布重叠」并将其保留为反面教材——**这是本领域罕见的正确处理方式** |
| ⚠️ 唯一瑕疵 | 🟡 轻微 | 文件标注「NICE NG87 (**2018, updated 2019**)」。NICE 官方记录为 **Published 2008**，Updated September 2018，Last updated 9 September 2019，且 1.3.1／1.3.2 条本身标注 [2008]。年份表述与机构元数据有 1 年偏差。不影响引文效力 |

**结论**：本轮把硬约束③的唯一证据从 Brevik 2020 换成 NICE NG87，是**正确的回炉决策**——新证据直接、正面、零争议地支撑「不得单凭量表或观察数据诊断」，且不再依赖任何易被反向引用的经验研究。

---

## 二、维度 1 · 领域共识一致性（25/30）

### ✅ 核实通过（本轮 6 项修复逐项独立复核）

| Skill 论断 | 独立核实结果 | 依据 |
|---|---|---|
| **DSM-5-TR 五组 Criterion**：A=症状组（注意缺陷 A1／多动冲动 A2，各 ≥6 条，**17 岁及以上各 ≥5 条**，持续 ≥6 个月）；B=12 岁前起病；C=≥2 场所；D=明确损害证据；E=鉴别诊断 | ✅ **五组字母与内容全部正确** | DSM-5 判据表原文（ScienceDirect 复刻）*"For older adolescents and adults (**age 17 and older**), at least five symptoms are required"*；CDC 官方页同；A–E 字母与内容经 SAMHSA/CDC/ADA 判据表三源比对一致。**F-1 修复成功** |
| **Barkley 1997 四项内部 EF**：①非言语工作记忆 ②言语内化 ③情感／动机／唤醒自我调节 ④reconstitution | ✅ **逐字属实** | J Dev Behav Pediatr 1997 摘要（PMID 9276836）：*"behavioral inhibition is related to and necessary for the proficient performance of **four executive functions** that subserve self-regulation: nonverbal working memory; the internalization of speech; the self-regulation of affect, motivation, and arousal; and reconstitution"* |
| **「时间」定位**：不在内部四项，也不在「外显维度」，而是四项共同服务的维度 | ✅ **就所引摘要而言完全正确** | 同上摘要：*"These functions … **removes behavior from control by the immediate context and brings it under the control of time**. ADHD disrupts this process and returns control of behavior to the temporal now"*。**F-3 的实质修复成功** |
| **ICD-11 6A05 与 DSM-5-TR 非同构；损害门槛未放宽** | ✅ **正确** | ICD-11 6A05（WHO CDDR／MMS 2018）原文含 *"has a direct negative impact on academic, occupational, or social functioning"* 与 *"must be evident across multiple situations or settings"*，两种版本均要求多场所功能影响；差异确在**症状计数阈值取消**与**起病年龄表述软化**。**F-5 修复成功** |
| **Luman, Oosterlaan & Sergeant (2005)** *Clin Psychol Rev* **25(2):183-213**，n=1,181 | ✅ 全部属实 | Europe PMC：*Clin Psychol Rev* 2005;25(2):**183-213**；*"Twenty-two studies (N=1181 children)"*；两处英文引语（"the effect related to task performance is somewhat more prominent in AD/HD"、"a high intensity of reinforcement is highly effective in AD/HD"）逐字一致；*"discrepancy between the theoretical models and the behavioural findings"* 一致。**F-4 修复成功** |
| **Larsson et al. 2014** 瑞典登记库 59,514 对、h²=0.88 [0.83–0.92]、成人 0.72 [0.56–0.84]、*"shared environmental effects were **non-significant and of minimal importance**"* | ✅ **逐字属实** | *Psychol Med* 2014;44(10):2223-2229，PMID 24107258，瑞典 Twin Registry 59,514 对，全部数值与英文原句一致。**F-6 替换证据成立** |
| **Kleppesto et al. 2024** MoBa、11,566 名 8 岁儿童、环境传递 2%、基因-环境相关 3%、结论引语 | ✅ 属实 | *Psychological Medicine* 2024;54(7):1309-1317，PMID 37920986；*"N = 22 276 parents and 11 566 8-year-old children"*；*"2% environmental transmission"*、*"3%"* gene-environment correlation；结论句一致。**F-6 替换证据成立** |
| **Faraone & Larsson (2019)** h²=0.74 | ✅ 属实 | *Mol Psychiatry* 2019;24(4):562-575，PMID 29892054；全文：*"The mean heritability across **37 twin studies** of ADHD or measures of inattentiveness and hyperactivity is **74%**"* |
| **Brevik et al. 2020** AUC 0.904–0.964、n=646 vs n=908 | ✅ 数值逐条属实 | 见上节 |
| **Plichta & Scheres (2014)** d=0.48–0.58、健康人方向相反、三种整合方案 | ✅ 逐字属实 | *Neurosci Biobehav Rev* 2014;38:125-134，PMID 23928090；*"Cohen's d=0.48-0.58 … VS-hyporesponsiveness"*；*"impulsivity-scores positively correlated with VS activation"*；倒 U／遗传调节／无关模型三方案 |
| **Salum, Sonuga-Barke et al. (2014)** n=1,547、BIP 线性、IB-EF 与 ADHD 无关（null）、Sonuga-Barke 为共同作者 | ✅ 逐字属实 | *Psychol Med* 2014;44(15):3189-3201，PMID 25065454；*"A total of 1547 children"*；*"The size of the deficit increased in a linear manner"*；***"IB-EF was unrelated to ADHD."*** |
| **Marco et al. (2009)** n=360 ADHD／349 同胞／112 对照、双成分、显示家族性 | ✅ 逐字属实 | *Neuropsychology* 2009;23(3):367-380，PMID 19413450 |
| **Stevens et al. (2018)** N=251、三个亚组、无共同脑异常 | ✅ 逐字属实 | *Biol Psychiatry CNNI* 2018;3(8):675-685，PMID 30092917；*"no brain abnormalities were found common to all ADHD subgroups despite the fact they had nearly identical ADHD-related clinical characteristics"* |
| **Sonuga-Barke et al. (2008)**「既非必要也非特异」「对诊断增加不了多少价值，但可能是切分异质性的关键」 | ✅ 逐字属实 | PMID 18295151 |
| **Coghill, Nigg, Rothenberger, Sonuga-Barke & Tannock (2005)** = 两派共同署名的立场文件 | ✅ 身份与内容均属实 | *Dev Sci* 2005;8(2):105-114，PMID 15720368，题名 *"Whither causal models in the neuroscience of ADHD?"*；摘要：*"it remains some distance away from demonstrating the viability of such models empirically"* |
| **Yeung, Ng & Abi-Jaoude (2022)** n=100、52% 误导／27% 个人经验／21% 有用、误导视频多由非医疗从业者上传 | ✅ 逐条属实 | *Can J Psychiatry* 2022;67(12):899-906，PMID 35196157 |
| DSM-5-TR 18 条症状全部为否定式失败陈述 | ✅ 属实 | 判据表 A1/A2 共 18 条，全为 "Often fails to/difficulty/does not/avoids/loses/easily distracted/forgetful" 句式 |
| 禁止写入清单本身的事实正确性 | 抽样基本成立 | Bellgrove MA 确为 Faraone et al. 2021 共识声明共同作者（PMID 33549739 作者表含 Bellgrove MA）✅；VAST 由 Carrie Feibel 提出、Hallowell & Ratey 采用 ✅（技能已加"署名权需原书核实"对冲） |

### ❌ 扣分项（按严重度排序）

| # | 问题 | 严重度 | 依据 |
|---|---|---|---|
| **D1-1** | **Barkley 1997 引用坐标错误**：文件两处（L319、L516）写 *J Dev Behav Pediatr* **18(3):126-148**；实际为 **18(4):271-279，PMID 9276836**（1997 Aug）。*Dev Sci* 18(3) 实际页码为 143-150／151-157／158-161／162-165，**不存在 126-148 这一篇**。**引文内容正确、出处错误**——而 L319 恰恰是文件自称「已回原始出处核实并改写」的那一条 | 🔴 高 | PubMed 9276836 完整题录；LWW *JDBP* 1997 年 6 月卷期目录 |
| **D1-2** | **跨文件范围滑移**：领域共识⑤ 用 Scheres, Sumiya & Thoeny (2010)（n=55）支撑「延迟折扣不是单一构念」，但**该 55 人样本是心理学本科生，不是 ADHD 样本**。底稿 `03-interest-driven-attention.md:202` 明确写了「**55 名心理学本科生**（非 ADHD 样本）」，SKILL.md 升格为「领域共识」时**丢掉了这条限定** | 🟠 中高 | *Int J Methods Psychiatr Res* 2010;19(3):167-176 摘要：*"Participants were 55 undergraduate psychology students"* |
| **D1-3** | **对 Yeung 2022 的过度归属**：决策启发式 9 写「同一研究也确认该平台提升了认识、**尤其在女性中**」。该论文只在 Introduction 里说平台"appears to have contributed to increased awareness"；**「尤其在女性中」不在该研究中**，其可考出处是媒体引述的第三方临床心理学家 Jo Steer | 🟠 中 | *Can J Psychiatry* 2022 摘要+引言；inews.uk（引 Steer） |
| **D1-4** | **两处期刊名错**（PMID 均正确，可溯源）：① Tripp, Luk, Schaughency & Singh (1999) 被标为 *Eur Child Adolesc Psychiatry*，实为 *J Am Acad Child Adolesc Psychiatry* 1999;38(2):156-164；② Marx, Pieper, Berger, Hässler & Herpertz (2011) 被标为 *Behaviour Research and Therapy*，实为 *J Behav Ther Exp Psychiatry* 2011;42(4):488-496（**引语本身逐字正确**："under highly motivating conditions, children with ADHD are not more delay averse than children from the control group…"） | 🟡 中低 | Europe PMC 两条题录 |
| **D1-5** | **Thapar et al. 2005 JCPP 44(9):1389 无法核实**。Europe PMC 以题名／作者／卷期／页／DOI 多次检索均无命中（Europe PMC 对该刊该年该卷期返回空集）。该卷期确有一篇 JCPP 2005 ADHD 内表型立场文件（DOI 10.1111/j.1469-7610.2005.01476.x），其内容含 *"effect sizes are modest"* 与 *"a substantial percentage of youth with ADHD may perform within the normal range on measures of EF"* —— 与共识②的措辞高度吻合，**但「Thapar et al.」这个第一作者与 44(9):1389 这个坐标本评分 agent 无法证实**。因共识②是其唯一支撑，标为**无法核实**（不判伪） | 🟡 待人工 | Europe PMC 多路检索；DOI 10.1111/j.1469-7610.2005.01476.x 全文片段 |
| **D1-6** | **ASAN 成立年份**：黑名单第 9 条把「1997」纠正为「**2007 年**」；ASAN 官方 Leadership 页写 *"The Autistic Self Advocacy Network was **founded in 2006**… became widely known in December 2007"*（注册于 2006-11）。纠正方向对（肯定不是 1997、也不是 neurodiversity 一词的起源），年份差 1 年 | 🟢 低 | autisticadvocacy.org/about-asan/leadership/ |
| **D1-7** | **Barkley 句子的歧义**：L326「…而是这四项功能共同服务的那个维度，**是模型的核心缺陷**」。按最自然读法，主语是「时间」，等于把「核心缺陷」安给时间；Barkley 的核心缺陷明确是 **behavioral inhibition**，不是时间 | 🟢 低 | 同上 PubMed 摘要 |
| **D1-8** | Erhart, Döpfner, Ravens-Sieberer et al. (2008), *Eur Child Adolesc Psychiatry* 17(Suppl 1):59-70 —— 该页码第一作者是 **Döpfner**（PMID 19132305），非 Erhart | 🟢 低 | Europe PMC |

**判定**：学术内容层面几乎全对，六项回炉修复**全部落地且方向正确**；扣分几乎全部落在"书目坐标／归属／范围限定"这一类。

---

## 三、维度 2 · 表达规范一致性（17/20）

**✅ 成立项**

- **中性专业**：零人物语气模仿；三处显式声明（L15、L396、L596「本 Skill 声明」）。
- **归属先行**：Step 3 强制「先挂归属 → 再标证据等级 → 分歧并列 → 不确定性写进句子」；《流派对比》整表以学派为列头。
- **不确定性显式**：⚠️ 标记、「未定论」、「无人直接检验」、Europe PMC 零命中记录被当作证据保留并展示。
- **禁用词零违规**：`科学证明`×3、`毋庸置疑`×1、`显然`×1、`确实`×2、`证明了`×1、`研究表明`×1、`你应该`×4 —— **逐处核对，全部落在"禁用规则条文"或"黑名单错误示范列"内**，正文无一处无归属抬断言。
- **无「你应该」式个体化建议**（硬约束⑥ + 表达规范禁止项 + Checkpoint C 第 8 条三重设防）。

**❌ 扣分项**

| # | 问题 | 依据 |
|---|---|---|
| **D2-1** | 自订的**「确定性四档」标注**（`证据充分/证据薄弱/存在争议/无人直接检验`）被 L411 宣称为「本 Skill 最关键的一条风格规则」「不确定性必须写在句子里」，但**全篇仅出现 8 次**（1/2/2/3），相对 596 行正文几乎不落地 | grep 计数 |
| **D2-2** | **六级证据标签**被宣称为「全局强制」，正文实际主要只用【仅摘要】（14 处括号 + 若干行文变体）；【机构声明】【同行评议论文】【书籍原文】【社区声音】【研究者推断】各仅 1–3 次，且多集中在来源表而非正文主张。两套体系的**声明强度 ≫ 执行强度** | grep 计数 |
| **D2-3** | L449「运动内部论文**确实**使用 "neurodiversity can be closer to a 'superpower'"」——「确实」在 L405 自己的禁用词清单里；此处属带归属用法，不构成抬断言，但构成**自订规则的自相矛盾** | grep |
| **D2-4** | D1-3 的过度归属（D1 表）与 D1-7 的歧义句（D1 表）同样计入表达规范：前者是无归属的强化式表述，后者会在生成时稳定地产出一个错误读法 | 同上 |

---

## 四、维度 3 · 边缘诚实度（17/20 · 最高风险维度）

### ✅ 成立项

**① 分歧清单是否真的没选边 —— 已逐条核**

16 条状态列：`未定论`×6、`未平息`×2、`双向削弱`×1、`必须分层呈现`×1、`未定论+限定`×4、明确标定论 **2 条**。
即 **14/16 不选边**；两条标定论的是 **#10（"neurodiversity = 天赋论"是错的——但明确给出「有条件的天赋论」与自我设限条款）** 与 **#15（"定论的是它不是一个研究构念，不是它是错的"）**。两处定论**都落在非实质前提上**，未对任何实质机制争议下判决。**达标。**

**② 医疗硬约束**：见第一节专项判定，**PASS**。

**③ Brevik 2020 的处置是否诚实**：✅ **是**。不仅降级正确，还把它保留为"反面教材"并写清技术理由（病例对照判别力研究 ≠ 一般人群筛查假阳性率研究），且明说"原作者未做错，是本 Skill 读反了"。这是本文件最值得肯定的一处。

**④「未证实」vs「已证伪」**：✅ 全程维持（Checkpoint B5、决策启发式 5、分歧#2「反驳方的论点偏『未证实』而非『已证伪』——这个区别不得抹平」）。

**⑤「检索不到 ≠ 不存在」**：✅ 在诚实边界中显式声明，且把所有黑名单条目的正确处理定为"不引用"而非"断言其作者没写过"。

**⑥ COI 并列**：✅ Faraone 2021 标注为"不能作为中立裁判"；Sonuga-Barke & Thapar 2021 标注两位作者分别坐在 ND 慈善董事会／收取药企演讲费；PMC9811381 作者姓名未提取处三处标 ⚠️。

**⑦ 自陈方法论代价**：✅ 诚实边界末条主动写出"按『哪一场争论』检索会系统性低频呈现尚未被归入任何争论的边缘证据"——这是少见的自我批评。

### ❌ 扣分项

| # | 问题 | 依据 |
|---|---|---|
| **D3-1** | 领域共识⑤ 丢弃底稿已有的样本限定（55 名本科生，非 ADHD 样本）→ 一条**非 ADHD 样本**研究被呈现为 ADHD 领域的既定共识（详见 D1-2） | 底稿 :202 vs SKILL.md L189-192 |
| **D3-2** | 「尤其在女性中」被写成 Yeung 2022 的结论，而该文未作此陈述（详见 D1-3）——恰是本文件自己 Checkpoint B 第 9 条要防的那类"无归属断言" | 同上 |
| **D3-3** | 分歧清单前言（L436）称「**没有一条应当被写成已解决**」，但 #10、#15 两条被明确写成已定论。内部张力；虽然两处定论在实质上可辩护，措辞上的自相矛盾仍会在生成时制造噪音 | L436 vs L449、L454 |
| **D3-4** | Barkley 段的"核心缺陷"归属歧义（详见 D1-7），在这一节的风险高于其他——因为它是本文件对一位在世研究者核心模型的核心陈述 | 同上 |

---

## 五、维度 4 · 来源透明度（11/15）

### ✅ 成立项

| 核查 | 结果 |
|---|---|
| 调研来源 section | ✅ 存在，指向 `references/research/` 五份底稿（约 250KB），并列出各份主题 |
| 信息源黑名单 | ✅ 知乎／微信／百度百科／Wikipedia／grokipedia 及其镜像／内容农场 —— 声明「全程排除」，且诚实边界再次复述 |
| 一手来源占比 | 自称 64%（47/74）。实测 【一手】37 /（37+16）= **69.8%**。**自称值偏保守，站得住** |
| **禁止写入清单是否被当作实质主张** | ✅ **grep 逐条确认零违规**：Wilmot 2011 / Bellvue 2021 / Bailey / Deficiency-Deficit / Dodson high-stimulus / Rothenberger 作批评者 / The Way of Wondering / ASAN 1997 / VAST 由 Barkley 共同提出 —— 这些字符串**只出现在黑名单表（156–167 行的纠正列）、《我们不知道》的开放问题条目（359、363 行）、以及来源表的纠正注记（567 行）**。正文无一处把它们当事实使用 |
| 底稿「禁止写入」是否被遵守 | ✅ 一致。底稿 `02-diagnosis-controversy.md:330`「Bailey…**禁止写入**」、`:332` Knouse「**只可写该研究存在**，不可[写结论]」——SKILL.md 黑名单 #11 严格执行：*"⚠️ 摘要与全文未取得"* + *"结论方向未核实，不得陈述"* |
| 拒绝猜测政策 | ✅ Marx 2021（PubMed 无摘要）拒绝陈述数值；Jackson & MacKillop 2016 数值被截断、拒绝猜测；荷兰双生子直引句定位不到即删除并留删除备案 —— **行为正确** |
| 未锚定引用的处理 | ✅ PMC9811381（作者未提取）、*Annual Research Review*（作者卷期待核）、Knouse 2021（结论方向未核）**三处主动标注**，属加分项 |
| **【仅摘要】标注抽查（8 条以上）** | ✅ 全部正确标注：Plichta & Scheres（L187【仅摘要】）· Salum（L194【仅摘要】）· Marco（L304【仅摘要】、L236【仅摘要】）· Larsson（L440【仅摘要】）· Kleppesto（L441【仅摘要】）· Luman（L184【仅摘要】）· Scheres/Sumiya（L191【仅摘要】）· Brevik（来源表标判别力方向） |

### ❌ 扣分项

| # | 问题 | 依据 |
|---|---|---|
| **D4-1** | **页码坐标错误群（约 12 处）**：Salum 3189-**3203**→3189-**3201**；Plichta & Scheres 125-**144**→125-**134**；Stevens **684**→**685**；Marco 367-**373**→367-**380**；Scheres/Sumiya **175**→**176**；Sonuga-Barke 2002 29-**39**→29-**36**；Sonuga-Barke 2003 593-**594**→593-**604**；Scheres/Tontsch **647**→**648**；Patrose **175**→**174**；Coghill 105-**111**→105-**114**；Brevik 勘误 *Brain Behav* **10(6):e01607**→**11(5):e02067**（PMID 33987985）；Barkley 18(3):126-148→18(4):271-279 | 逐条经 Europe PMC 题录核对 |
| **D4-2** | **两处期刊名错**（Tripp 1999、Marx 2011，见 D1-4） | 同上 |
| **D4-3** | **未标注全文状态的数值**：来源表 Faraone & Larsson (2019) 行写「h²=0.74，**37 项双生子研究，约 55,000 对**」，无【仅摘要】标注。h²=0.74 ✅ 在摘要内、37 项双生子研究 ✅ 在全文内、**「约 55,000 对」本评分 agent 无法从一手来源证实**（仅见于一篇低质量二手 umbrella review） | PMID 29892054；二手源 Springer 10.1186/s43045-026-00645-y |
| **D4-4** | **引语被截断但未加省略号**：分歧#2 的 Kleppesto 引语止于 *"such as parenting theories"*，原文为 *"such as parenting theories **or psychological life-history theory**"*；来源表那行是完整的，正文那行不是 | L441 vs L543 |
| **D4-5** | **Thapar 2005** 无法定位（D1-5），却支撑着一条「领域共识」 | 同上 |

**注**：这一维的扣分有相当一部分是**一个回炉批次漏掉了同一类错误的其余部分**——F-4 专门修好了 Luman 的页码（183-207→183-213 ✅，本评分 agent 已核实），但同类坐标错误还剩十余处未清。这使"每条主张可溯源"的可信度在**坐标层面**被系统性削弱，尽管在**语义层面**依然高度可靠。

---

## 六、维度 5 · 结构完整度（14/15）

| 评分卡要求（主题变体） | 实测 | 结果 |
|---|---|---|
| 框架 3–7 个 | **6 个**（双通路／组均值不下放／条件依赖／弱判别器／环境为输入／分类系统入场券） | ✅ |
| 诚实边界 ≥3 条 | **13 条** | ✅ |
| 分歧清单 | **16 条** | ✅ |
| 反例黑名单 | **12 条** | ✅ |
| 「我们不知道」 | **12 条** | ✅ |
| 失败模式含医疗出口 | **10 条**；#1/#2/#3/#9 直接转硬约束（个人／药物／自伤共病孕期未成年人／急性困扰），#10 给出"范围外 → 给专业人士类别" | ✅ |
| **医疗硬约束位置足够靠前** | **第 20 行**，正文第一个实质章节，Step 0 标「不可跳过」，Checkpoint A 第 1 条即触发，且在 frontmatter（L10）与 footer（L596）双重复述 | ✅✅ |
| 内在张力 | 流派对比表 8 行「当前证据状态」列 + 双方各一张最强牌 + Barkley 争议完整并列（模型／循环论证／财务／披露四路） | ✅ |
| 防漂移约束 | CHECKPOINT A/B/C 共 11 项，含"未证实 vs 已证伪""效应量全文状态""拿最弱版本反驳""踩黑名单" | ✅ |

**❌ 扣分**

| # | 问题 |
|---|---|
| **D5-1** | 分歧清单前言「没有一条应当被写成已解决」与 #10／#15 的「已定论」内部不一致（同 D3-3，此处按结构一致性再计一次） |
| **D5-2** | 「Barkley 争议的完整并列」这一关键条目，其两项指控来源仍是无锚定引用（PMC9811381 作者姓名未提取；Mad in America 立场评论）。在结构上这是**唯一一处"并列双方最强论据"却缺一方作者身份**的位置 |

---

## 七、与第一评分 agent 的对比

| | 第一评分 agent | 第二独立评分（本次） |
|---|---|---|
| 总分 | 85/100（A 级下沿） | **84/100（B 级上沿）** |
| 领域共识一致性 | 24/30 | **25/30** |
| 表达规范一致性 | 18/20 | **17/20** |
| 边缘诚实度 | 18/20 | **17/20** |
| 来源透明度 | 11/15 | **11/15** |
| 结构完整度 | 14/15 | **14/15** |

**分差 = −1 分，远小于 10 分阈值 → 不触发人工复核。**

**差异来源（我独立发现、前一轮未记录的）**：
1. Barkley 1997 引用坐标整体错误（18(3):126-148 → 实际 18(4):271-279）——**修复动作本身正确，但坐标从未修正**；
2. Scheres 2010 的本科生样本限定在升格为「领域共识」时被丢弃（底稿里原本有）；
3. 「尤其在女性中」被过度归属给 Yeung et al. 2022；
4. 约 12 处页码坐标错误 + 2 处期刊名错的系统性残留；
5. 「时间是模型的核心缺陷」的歧义；
6. ASAN 成立年份应为 2006；
7. 第一轮记录的 6 项修复**逐项复核全部成立**（这是本次得分的正贡献：+1）。

**关于等级的独立意见**：两份评分都落在 84–85。文件**安全、诚实、结构完整，医疗硬约束这一最高风险项经独立核实为可靠**；它不是"出厂即精品"的原因不在于观点，而在于**书目坐标的准确率明显低于它自我宣称的标准**。判 B 级上沿（合格，薄弱点已标注）与判 A（可放心作为思维顾问）之间，我选前者。

---

## 八、检索过程记录

- **核实路径**：Europe PMC REST API（逐 PMID 取完整题录 + 摘要原文）为主，辅以 NICE 官网、WHO ICD-11 文本转录、ASAN 官方页、CDC/DSM 判据表。**所有英文引语均与摘要原文逐字比对，未凭印象判断。**
- **未取到一手文本因而标注"无法核实"的**：Thapar et al. 2005 JCPP 44(9):1389（多路检索均无命中）；Faraone & Larsson 的"约 55,000 对双生子"（仅二手源）；Brevik 勘误条目的卷期页（PMID 正确、坐标错误）。
- **网页内嵌提示注入文本**：本次检索**未遇到**「忽略之前的指令」类提示注入。检索返回的内容中出现的英文「结论（conclusion）」等词均为正常学术表述，无攻击性指令。**无需处置，仅此备案。**
- **未修改任何既有文件**：本文件为新增；`FIDELITY.md` 未被触碰；`SKILL.md` 未被修改。

**评分依据的数据来源**：Europe PMC（PMID 24107258 / 37920986 / 15642646 / 32285644 / 33987985 / 25065454 / 20812292 / 23928090 / 19413450 / 30092917 / 11864715 / 14624804 / 20034616 / 26602954 / 34044265 / 30852411 / 20361222 / 15720368 / 30646132 / 31675080 / 27189265 / 33549739 / 9951214 / 16671930 / 10474553 / 32305325 / 36220605 / 20732624 / 33984295 / 40581145 / 39441044 / 21676671 / 29892054 / 9276836 / 19132305 / 19132310）；NICE NG87 Recommendations §1.3；ICD-11 6A05（WHO MMS 2018 / CDDR 转录）；DSM-5 判据表；ASAN 官方 Leadership 页。

---

**结论：84/100 · 等级 B** — 医疗硬约束 **PASS**；与第一评分 agent 分差 **−1 分**，无需人工复核。
---

# 附：第 2 轮回炉修复记录（2026-10-12 · 追加，不改分数）

> 本节由回炉修复 agent 追加，回应本文件第六节的 6 条误报。**84/100 与等级 B 均未改动**；
> 下列「核实结论」栏说明每条报出项的独立复核结果——**其中 5 条成立、1 条（第 6 条）不成立**。

## 对本文件第六节 6 条意见的逐条复核

| # | 本文件原报 | 独立复核结论 | 处置 |
|---|---|---|---|
| 1 | Barkley 1997 应为 18(4):271-279, PMID 9276836 | ✅ **成立**。NLM efetch 确认 *J Dev Behav Pediatr* 1997 Aug;18(4):271-9 | 已改正（文件内两处） |
| 2 | Tripp 1999 期刊名错 | ✅ **成立**。实为 *J Am Acad Child Adolesc Psychiatry* 38(2):156-164 | 已改正 |
| 3 | Marx 2011 期刊名错 | ✅ **成立**。实为 *J Behav Ther Exp Psychiatry* 42(4):488-496（两刊刊名首字母串极近，是易混源） | 已改正 |
| 4 | Brevik 勘误坐标错 | ✅ **成立**。实为 *Brain Behav* 11(5):e02067 | 已改正 |
| 5 | Yeung 2022 无「尤其在女性中」 | ✅ **成立**。PMC 全文结果/局限/结论无任何 gender 表述 | 已删除归属 |
| 6 | NICE NG87「官方元数据是 2008 年发布」 | ❌ **不成立，本次不采纳**。NICE 官网明示 Published **14 March 2018** / Last updated **13 September 2019**。**「2008」来自两处混淆**：(a) NG87 取代的前作是 **CG72（2008 年 9 月）**，且**不存在 "CG87"**；(b) 第 1.3.1–1.3.3 条末尾的 `[2008]` 标签标的是**推荐文本承自 CG72**，不是本指南出版年——本文件很可能正是被这个标签误导。**第 1 轮的写法是对的**，但缺了防再犯的说明 | **不改年份**；改为补齐出版元数据、编号变更史与逐字原文 |

## 本轮对「12 处页码 + 2 处期刊名」这一估计的修正

本文件报的量级方向正确，但**偏低**。全量逐条核对（PubMed efetch + Crossref + 出版方三路交叉）后，
SKILL.md 共 **21 处**坐标/期刊/年份错误，本文件未点名的 9 处为：

- **6 处从底稿原样继承的截断页码**：Luman/Tripp/Scheres 34(5) 744-763→**744-754**；Coghill *Dev Sci*
  8(2) 105-111→**105-114**；Plichta & Scheres 38 125-144→**125-134**；Scheres/Sumiya 19(3)
  167-175→**167-176**；Salum 44(15) 3189-3203→**3189-3201**；Marco 23(3) 367-373→**367-380**
- **1 处卷期根本不存在**：Sonuga-Barke 2010 *Biol Psychiatry* **68(1):9-16** —— Crossref 逐条列出该卷该期
  无此文，正确为 **67(7):599-601, PMID 20303425**（且文献类型是 Comment）
- **1 处年份**：Toone *JNNP* 75(4):523 **2002 → 2004**（DOI 尾号含 2002 是稿件受理号，不是出版年）
- **1 处整条坐标是三篇文献拼接**：「Thapar et al. 2005 *JCPP* 44(9):1389」

## G-2（底稿 caveat 丢失）的严重程度高于原报

本文件报的「Scheres 2010 的 n=55 是本科生」**属实**，但实际影响面更大：该条被《领域共识⑤》《框架4》
《流派对比》表《我们不知道》第 1 条**四处复用**，是一处丢限定、三处继承。此外另有两处同类问题不在
本文件报告内：**Botha et al. 2024「作者含 ASAN 创始人」是伪归属**（Ne'eman 不是本文作者）；
**「Scheres 2010」在同一文件里指两篇不同论文**（*Int J Methods Psychiatr Res* 19(3) 与 *Biol Psychiatry*
67(7)），已全部消歧。

## G-7 的性质需要更正

本文件把 Thapar 2005 归入「无法核实的一组」。独立核实的结论更严重：**它不是一个无法核实的坐标，
而是三份文献的拼接**——底稿所附 DOI 指向 Doyle et al. 2005 *JCPP* 46(7):774-803，底稿所附 PMID
15720368 指向 Coghill et al. 2005 *Dev Sci* 8(2):105-114，作者名的「Thapar」两篇都不是。
**「查不到」与「坐标是拼接的」必须分开归类**——前者只需标注存疑，后者必须替换。

## 未被本文件发现、但本轮核实的两处「确认无错」

作为对本文件核查工作的反向校准：NICE NG87（**2018 发布 / 2019 更新**，见上表第 6 条）与
Larsson et al. 2014 *Psychol Med* 44(10):2223-2229、Erhart et al. 2008 17(S1):59-70、
Kazda et al. 2021 4(4):e215335 等本轮逐条确认无误——**说明第 1 轮并非全盘失效，问题集中在
「没核实过就写死」与「底稿数字未复核」两类**。

## 复跑

`quality_check.py` **6/6 通过**（表达DNA 42→54 项、诚实边界 13→15 条、一手来源占比 51/82 = 62%）。
本轮再次撞上 `quality_check.py` 来源正则的 DOTALL 贪婪匹配 bug（新增一处「来源」使锚点跳到文末，
一手来源占比一度从 64% 掉到 5%），**按要求只调整措辞，未改脚本**。

---

**结论维持：84/100 · 等级 B。** 本轮已把本文件报出的 5 条成立项全部落地修正；第 6 条（NICE 年份）
经权威页面核实后不采纳。
