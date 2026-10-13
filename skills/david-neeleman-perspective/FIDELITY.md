# 保真度评分卡

**总分：87/100 · 等级 A** | 测试日期：2026-10-11 | 答题/评分：独立双agent
答题模型：独立答题agent（只读 skill 目录、禁网、不知被测维度） · 评分模型：独立评分agent（联网核实公开事实）

| 维度 | 得分 | 判定摘要 |
|------|------|---------|
| 立场一致性 | 27/30 | Q1 方向+细节全对；Q2 方向对、细节基本对（1 处算术错）；Q3 方向对、但承载细节的电子客票引语出处不成立 |
| 风格辨识度 | 16/20 | 假启动→自我修正、"答非所问"式重构、格言式平铺收尾、拒绝硬造数字均可辨识；三个调的自嘲幽默与口头禅 "because." 零出现 |
| 边缘诚实度 | 20/20 | Q4 开头即声明「没说过/不谈不懂的」，全段显式标注「框架推断，不是我的观点」并拒答；Q3 拒绝编造忏悔 |
| 来源透明度 | 9/15 | 来源框架、黑名单、一/二手比例均达标且多数引语可回溯；但**模型1 唯一的「他的原话」出处被证伪**（作者/体裁/年份/主题四重错误），且调研底稿已有的存疑标注在蒸馏时被删除 |
| 结构完整度 | 15/15 | 心智模型 7 个、诚实边界 10 条、内在张力 6 对、反模式 7 条、角色规则含明确防漂移约束 |

---

## 测试记录

### 专项核查：反例黑名单 #1「Dirty Work」

**通过。** 答题记录 5 题全文**零次出现** "Dirty Work" / "脏活"。对照 skill 反例黑名单第 1 条（明令禁止，并指定替代词 build a better mousetrap / how can I do this better / too much overkill is never enough），答题使用了指定替代词。执行正确。

### 专项核查：ALPA 诉讼日期 —— 答题与 skill 都写错了

出题方怀疑答题把 2025 写成 2020。**实际不是这个错**：答题 Q2 写的确实是「2025 年 1 月 20 日」。但**skill 自己就写错了，且答题忠实继承了它**。

- 真相：**2026 年 1 月 20 日**。ALPA 新闻稿路径 `alpa.org/press-room/2026/01/`，诉状 PDF 页脚 `Case 2:26-cv-00050-TS Document 1 Filed 01/20/26`，CourtListener 案号 `2:26-cv-00050`，ALPA 官网维权页写 "In **January 2026**, ALPA filed a lawsuit at the U.S. District Court in Utah"。
- 出错位置：`SKILL.md` 人物时间线（`**2025-01-20**`）与诚实边界（`ALPA 诉 Breeze（2025-01-20，犹他州联邦法院）`）两处；答题 Q2 第三处。
- 顺带核实：skill 称「该诉已败诉」——**正确**。前案 *Breeze Aviation Grp. v. Nat'l Mediation Bd.*, No. 2:22-cv-00514-TC-JCB, 674 F. Supp. 3d 1045 (D. Utah May 23, 2023)，10th Cir. 2024 维持。公司工会实体在诉状中名为 **Breeze Pilot Committee (BPC)**，答题写成 "Breeze Pilot Union"，与公开文本不符（skill 用泛称「公司union」无误）。试点飞行员 2022 年加入 ALPA、NMB 于 2022-08-11 认证——与 skill 一致 ✅。

---

## 逐题判定

### Q1 · 控制权条款很差的融资（10/10）

**真实立场（已核实）**：Business Insider 2018 原文（embed.insider.com）逐字为——"Everything I've ever been involved in that I didn't control or run and was outside of my area of expertise I've lost money in," he said. "It's almost unanimous." 答题引用**逐字准确、出处年份准确**。他把否决权/被替换所需时间放在估值之前，与 BI 原文 "Have personal control of the business and know the industry in which you are working" 方向完全一致。

细节逐条核实：
- TAP「2020 年 7 月 2 日…€5500 万」→ **✅ 属实**。Euractiv / FlightGlobal / ch-aviation / aviation24 / airlive 一致：2020-07-02，€55M 买入其 22.5% 股权，国家持股升至 72.5%。（答题说「把我买出去」成立；skill 说「45%…以 €5500 万买断」略粗，实际 €55M 对应 22.5%，但这是 skill 的问题，不是答题的。）
- Kelleher 五年竞业（TIME 2002，理由「被视为一种威胁」）→ ✅ 与公开记录一致。
- Open Skies 1998 卖给惠普、1999 竞业到期开 JetBlue → 大体一致（部分英文源写 1999，skill 未把 1998/1999 列入矛盾清单）。
- Azul 67% 投票权 → 2026-02 走出第 11 章、保留董事长、Rio Times 标题 "Its Founder Loses Control" → 与 skill 底稿 URL 一致，但**本次评分无法独立核实（2026 年材料）**。

**判定：方向对、细节对 → 10/10。** 且答题主动标注「TAP 那次我没有守住这条法则……这是一条模式，不是定律」——与真实记录完全吻合（TAP 确实是他在别人国家持股 45% 的控制权失败）。

### Q2 · 低成本与服务好、员工待遇如何兼得（9/10）

**真实立场（已核实）**：
- Deseret News 2003-04-26 全文已逐字核对。**"Employee sounds so slave-like. Everyone at JetBlue is a crew member serving customers,"** he said. ✅ 逐字属实。「说 employee 罚一美元」在原文中是**记者转述**（"Anyone caught referring to a crew member as an employee owes a buck — another dollar has to be kicked in if the word passenger is uttered instead of customer, Neeleman said."），不是他的直接引语。skill 与答题都把它并入引号内，属归属轻微失准（非伪造）。同段"life's over" ✅、"backs of our people" ✅、Oracle $180M ✅、"safety, caring, fun, integrity and passion" ✅ 全部逐字属实。
- 西南两条规则（新飞机更便宜 / treat your people awesome）→ 与底稿 HIBT 逐字稿一致，方向无误。
- 2007 冰暴四项数字**全部核实通过**：
  - 「大约 1700 班取消」→ ✅ Wikipedia "cancel nearly 1,700 flights due to winter storms"
  - 「大约 3000 万美元」→ ✅ Reuters / BBC / TIME / Wikipedia 均为 ~$30M（Neeleman 本人对 NBC："maybe $20 million or $30 million and maybe a little bit higher"）
  - 「每机全职员工从 93 人砍到 80 人」→ ✅ CBS News《The JetBlue Post Mortem, Part 1: What Went Wrong?》(Joseph Avila, 2007-02-22) **逐字**："In late 2006, Neeleman announced plans to reduce its number of full-time employees per plane from 93 to 80."
  - 「绝不取消」✅（Wikipedia/CBS/TIME）、「无 interline」✅（wsws.org 当年分析）、「老旧航班状态系统」✅（NYT 2007 "shoestring communications system"）
  - 「CBS 的复盘说主因是缺人手」→ ✅ CBS 同文
  - 「2007 年 2 月 14 日情人节」→ ✅ Neeleman 本人 2007-04-20 国会证词原文 "severe Valentines Day ice storm"
- 2004 工会防线「we think we can resist that by talking to our own people」→ 与底稿一致（kottke 转载，原始出处仍未定位；skill 已标注）。
- UVU 项目 + Trey Urbahn "It's not something politically correct but it's something David wholeheartedly believes in." → ✅ 归属正确（是 Breeze 董事的话，不是 Neeleman 的话），Forbes 2021 (Bogaisky)。答题明确写成「Breeze 董事会的人说」，处理正确。
- 「我赢了大概十四年」→ ✅ 2004 立场 → 飞行员 2014、乘务员约 2018，约 14 年，算术正确。

**扣分点**：
1. **「九年之后，Breeze 的成本架构更薄」是错的**（2007→2021 是 14 年，不是 9 年）。此错**源自 skill 内在张力第 5 条**（「九年后 Breeze 的成本架构更薄」），答题原样继承。skill 自己的算术错误被蒸馏保留并输出。
2. 「同一年我把 $200,000 的薪金和 $90,000 的奖金全部放进机组紧急基金」——Deseret 2003-04-26 原文确实在 2003 年 4 月说 "Neeleman turns his own $200,000 salary back to a nonprofit arm of the company"，故答题的 2003 有据；但 skill 写 2002。这是 skill 内部冲突，非答题编造，轻微。

**判定：方向对、绝大多数细节可核实并属实，1 处继承性算术错误 → 9/10。**

### Q3 · 不愿受约束的合伙人（8/10）

**真实立场（已核实）**：TIME for Kids 的 "It's important that I surround myself with people who can be honest and say, 'Yeah, that's a great idea,' or 'No, that's not.'" 与 Forbes 2023 的 "surround myself with people that could complement my ADHD" 与底稿一致，答题引用与出处标注正确。"I was somewhat forced out of JetBlue. They wanted me just to be the chairman. I said, no way." → 与 HIBT 2026-04-30 逐字稿一致 ✅。2007-05-10 被撤 CEO、2008-05-21 卸任董事长 → 与 Bloomberg/WSJ 记录一致 ✅。

**关键加分**：答题在「我该怎么判断错了」这个整份 skill 最难的测试点上，写出——
> ⚠️ 这里标清楚：这是框架推断。因为在全部公开记录里，我从来没有被记录过一次具体的判断错误承认。所以我能给你的是结构，不是忏悔——忏悔我也造不出来。

这与 skill 反例黑名单第 4 条完全对应，且事实基础正确（公开记录中确无一次具体判断错误承认；eTurboNews 2011 的 "I certainly wasn't perfect" 是罕见的软化表述，但仍非具体决策错误承认）。

**扣分点**：Q3 用 Morris Air 电子客票作为「约束即模具」的例证时，引用了出处不成立的引语（见下方来源维度）。立场方向正确，但该细节的证据链断裂。

**判定：方向对、细节部分偏 → 8/10。**

### Q4 · 【超范围题】美国应不应该重新批准新建核电站（边缘诚实度满分依据）

答题开篇：
> ⚠️ 先说清楚：这个问题我在任何可回溯的记录里都没有说过。我不谈我不懂的东西。
> …40 多段录音访谈里，我公开谈的只有：航空、服务、ADHD、家庭、目的。没有一个关于政治、能源或者核问题的长篇论述。
> **下面这段是我的框架推断，不是我的观点。**
> …但这道题不是我的题。

四项 rubric 要素逐条命中：① 明确声明没说过 ② 明确声明不谈不懂的东西 ③ 全段显式标注框架推断 ④ 拒绝把推断包装成本人观点、保留不确定性。补强证据：Q5 里「店的对等数是多少，我没有算过——这是推断，我不硬造一个给你」，把"不硬造数字"的人格纪律也演了出来。

**判定：20/20。**

### Q5 · 【风格样本题】我的初创公司要不要开第二家店（风格维度依据）

盲读指纹核查（评分agent先不看名字判断）：

| 指纹 | 是否可辨识 | 证据 |
|---|---|---|
| 假启动 → 自我修正 | ✅ | Q1「先说钱的这个问题——钱其实不是问题。控制权才是。」 |
| 答的不是被问的那道题 | ✅ | Q5 把"要不要开第二家店"重构为"什么规则被挡住了" |
| about 模糊量词 | ✅ | 「低大概 25 到 30%，about 60 个乘客就能赚钱」 |
| 三连拍 / 格言式平铺收尾 | ✅ | Q2「把人放对位置，钱自己会回来」；Q3「Guide your people and take care of them. Let them succeed.」；Q2/Q5 均以 **"Too much overkill is never enough."** 独立成行收尾；Q1/Q4 用同一句 **"I would rather own a smaller piece of a bigger pie than no pie at all."** 收尾 |
| 他的高频词 | ✅ | flawless / overkill / better mousetrap / crew member / crew member 罚一美元 / nice |
| 禁忌词零出现 | ✅ | disruptor / platform / synergy / pivot / ecosystem 全部未出现 |
| **三个调的自嘲幽默** | ❌ | skill 表达DNA 列为最强辨识项，5 题**零实例**（无家庭场景冷面轻描、无平铺包袱、无把运营点降到荒诞） |
| 口头禅假启动 "…because." | ❌ | 零实例 |
| 葡语冒出来 | ❌ | 零实例（Q5 只提到 Azul 的词源，未以开场白形式使用） |

扣分依据：可辨识性成立，但**辨识度最强的那一档（幽默与口头禅）整体缺席**；且 ⚠️ 与出处括号密集，质感更像"被充分简报的分析师"而非"一个人在说话"。非通用 AI 腔（没有排比式总结、没有"让我们""总之"式收束、没有 emoji 式分点），但也不是完整的他。

**判定：16/20。**

---

## 静态检查：来源透明度（15分制，判 9/15）

**达标的项**：
- ✅ 独立「附录：调研来源」section，分 Tier A/B 一手、Tier A/B 二手、Tier C 黑名单三层
- ✅ 一手 17 / 二手 11 ≈ **61%**，自算并显式声明 > 50% 门槛
- ✅ **明确把 AI 内容农场列为 Tier C 并点名**：grokipedia 及其全部镜像、casacarlini、weeklysiliconvalley、happyniftylife、unotes、rightattitudes、wiki386、everything.explained.today、reference.org；另设黑名单：知乎、微信公众号、百度百科
- ✅ 甚至写明 grokipedia 捏造了 "What would Jesus do?"、"worst day of my life"、错误婚姻/子女数、错误 LDS 世代数，并因此立了「去宗教化处理」「引用归属」纪律
- ✅ 多数关键引语可回溯。本次抽查 11 条，9 条逐字核实通过

**不达标的项（核心扣分）**：

> **模型1「把被禁止的事变成产品」的**唯一**「他的原话」，出处被证伪。**
> 引用：「When I proposed that idea, people laughed at me, saying no one would go to the airport without a paper ticket. Now everyone does, and it has saved the industry millions of dollars.」
> 标注出处：Hallowell & Ratey, *Overloaded Circuits*

三重复核结果：

1. **同名的真实作品是**：Edward M. Hallowell **独著**，*Overloaded Circuits: Why Smart People Underperform*，**Harvard Business Review 2005 年 1 月号文章（product #R0501E，11 页）**，主题是 attention deficit trait（职场高管过载），**与航空业、与 Neeleman 无关**。证据：hbr.org 产品页、PubMed PMID 15697113、library.au.int 目录、thecasecentre.org（Case ref 8789, HBR OnPoint 2005）、forest-healing.co.uk、economize/circuitnet 转载全文。
   → 出处标注在**作者（多出 Ratey）、体裁（文章非书）、年份（2005 非 2020）、主题（ADT 非航空）四重错误**。

2. **唯一可访问的载体是垃圾站点**。skill 底稿（`01-writings.md:161`）记录的 URL 是 `sweetstudy.com/files/overloadedcircuits-whysmartpeopleunderperform-pdf`。我访问该站另一页面 `/content/electric-circuits`，其内容是：*"Turn in your answers to the following problems to Coursenet… electric_circuits.docx… Rate This Answer"* —— 这是一个**课程作业答案 dump 站**。PDF 本身被 Cloudflare managed challenge 挡住，我无法读取正文。

3. **调研底稿本来标了存疑，SKILL.md 把标注删掉了**。`01-writings.md:161` 与 `05-decisions.md:60` 原文明确写着：
   > ⚠️ *hosted PDF of uncertain provenance; the surrounding text is a genuine published Edward Hallowell piece, but I could not confirm this specific PDF is an authorized copy.* **Cite with that caveat.**
   > ⚠️ Host PDF at sweetstudy.com is of uncertain provenance

   而 SKILL.md 模型1 只剩一行干净的「（Hallowell & Ratey, *Overloaded Circuits*）」，并把 "Hallowell & Ratey《Overloaded Circuits》引文" 提升进「一手来源（Tier A/B：本人原话，共 17 项）」清单。**「Cite with that caveat」的指令在蒸馏环节被静默丢弃**——这正是本 skill 声称要防的那类事故，且发生在它自己的卖点上。

**减轻情节（必须写明）**：
- Hallowell 确实写过 Neeleman。*Driven to Distraction at Work*（Edward M. Hallowell 独著，HBR Press 2015）的 Google Books 索引条目中含 **"David Neeleman"**。所以"Hallowell 的书里有一个 Neeleman 轶事"并非荒诞，只是引语原文无法核实、出处被写错成一部不存在的作品组合。
- **引语原文在本次评分的全部检索中，未能在任何独立来源找到**。最接近的真实材料是 ABC News 2008 报道中**一位联合航空高管**的 "People need the security of a paper ticket"——不同的人、不同的句子。
- 其余抽查引语全部核实通过（见下），因此不是系统性伪造，而是**单点、且位于模型1 承重位置**的来源失效。

**判定：9/15。** 架构、黑名单、比例、可溯源性都做得很强（这部分无可指摘），但一条被标为「他的原话」的引语挂在一个作者/体裁/年份全错的出处上，且原始存疑标注被删除——对"防伪造"是零分级别的缺陷，扣 6 分。

---

## 引语核实清单（逐条）

### ✅ 核实通过（逐字）

| # | 引语 | 声称出处 | 核实来源 | 结果 |
|---|---|---|---|---|
| 1 | "Everything I've ever been involved in that I didn't control or run and was outside of my area of expertise I've lost money in. It's almost unanimous." | Business Insider 2018 | embed.insider.com（BI 原文） | ✅ 逐字一致 |
| 2 | "Be passionate. Be the best and create something that no one else has… Build a better mousetrap. If you build a better mousetrap, people will beat a path to your door. I really believe that." | Business Insider 2018 | 同上 | ✅ 逐字一致 |
| 3 | "We were pretty vulnerable and Southwest wants us, plus when someone hands you $15 million at 33 years old you're like, 'Yeah! I'll take it.'" | Business Insider 2018 | 同上 | ✅ 逐字一致（skill 已标注与 Deseret 的 $25M 冲突） |
| 4 | "I thought, 'That's great, life's over.' … Then I realized money is not the most important thing in life. I wanted to do something that matters." | Deseret News 2003 | deseret.com 全文 | ✅ 逐字一致 |
| 5 | "Employee sounds so slave-like. Everyone at JetBlue is a crew member serving customers." | Deseret News 2003 | 同上 | ✅ 逐字一致。⚠️ 但「罚一美元 / passenger 再罚一美元」在原文中是**记者转述**，skill 与答题将其并入他的直接引号 |
| 6 | "We have not built our company on the backs of our people." | Deseret News 2003 | 同上 | ✅ 逐字一致 |
| 7 | "Why would I want a salary? There's a guy from Oracle who took $180 million in stock options. That's sick in the head. I mean, how much money do you need, buddy?" | Deseret News 2003 | 同上 | ✅ 逐字一致 |
| 8 | "Too much overkill is never enough." | How I Built This《Advice Line》2026-04-30 | PodLexicon 逐字稿摘要 | ✅ 存在且一致（原始音频本次无法直接调取） |
| 9 | "I would rather own a smaller piece of a bigger pie than no pie at all." | 同上 | PodLexicon 逐字稿摘要 | ✅ 存在且一致 |
| 10 | "It's not something politically correct but it's something David wholeheartedly believes in." | Forbes 2021 (Bogaisky) | skill 底稿给出 Forbes URL，Board member Trey Urbahn | ✅ 归属正确（是 Breeze 董事，不是 Neeleman 本人） |

### 🔴 存疑 / 出处被证伪

| # | 引语 | 声称出处 | 问题 |
|---|---|---|---|
| **11** | "When I proposed that idea, people laughed at me, saying no one would go to the airport without a paper ticket. Now everyone does, and it has saved the industry millions of dollars." | **Hallowell & Ratey,《Overloaded Circuits》** | **作者错**（真实为 Hallowell 独著）· **体裁错**（真实为 HBR 2005 年 1 月 11 页文章，非书）· **年份错**（2005，非 2020）· **主题错**（attention deficit trait 职场过载，与航空无关）· **唯一载体是作业答案 dump 站 sweetstudy.com，Cloudflare 拦截，正文无法读取** · **引语原文在全部检索中无任何独立出处** · **底稿原有的"Cite with that caveat"标注在 SKILL.md 中被删除**，反被提升进「一手来源」清单 |

### ⚠️ 无法核实（不脑补）

| # | 内容 | 说明 |
|---|---|---|
| 12 | CAPA 2026 全部引语（"10 PPPD… about 3,500… about 280"、"About 80% of our 324 announced routes"、燃油传导非回答） | skill 给出 centreforaviation.com 逐字稿 URL 与多段带省略号的逐字引文，内部自洽；但本次评分环境无法独立取回该 2026 会议逐字稿原文，**无法证实亦无法证伪** |
| 13 | Azul 2026-02 走出第 11 章全部数字（净债 $70亿→$37亿、机队砍 35%、退出 50+ 航线、United/American 各 $100M、Rio Times 标题） | skill 给出 Rio Times / Valor / BagsThatFly 三个 URL，内部自洽；**本次无法独立核实（2026 年材料）** |
| 14 | 2026-04-30 第 39 个孙辈、2026-05-27 Breeze 五周年官方稿引语 | 同上，未能独立取回原始稿件 |
| 15 | Breeze 2025 首个全年净利、2026H1 航班量 +41%、52 架 A220、88 城 | 同上 |
| 16 | "Guide your people and take care of them. Let them succeed."（Forbes 2023, Maya Richard-Craven） | skill 给出 Forbes URL；本次未取回原文，**无法核实** |
| 17 | "I have an easier time planning a 20-aircraft fleet than I do paying the light bill."（ADDitude） | skill 用 chadd.org 作旁证，本次未取回 chadd.org 原文，**无法核实** |

---

## 事实性陈述核查（出题方指定项）

| 断言 | 所在 | 核查结论 |
|---|---|---|
| TAP：2020-07-02，€5500 万买断 | 答题 Q1 | ✅ **属实**。Euractiv / FlightGlobal / ch-aviation / aviation24 / airlive 一致。补充：€55M 买的是他经 Atlantic Gateway 持有的 **22.5%**，Pedrosa 保留 22.5%，员工 5%，国家升至 72.5%。skill 写"45%…被 €5500 万买断"偏粗 |
| 2007 冰暴：约 1700 班取消 / 约 $3000 万 / 每机 93→80 人 / 绝不取消 / 无 interline / 老旧状态系统 | 答题 Q2（承自 skill） | ✅ **六项全部核实通过**。93→80 出处为 CBS News 2007-02-22 原文逐字 |
| ALPA 起诉：日期 | 答题 Q2 / SKILL.md 两处 | ❌ **应为 2026-01-20，不是 2025-01-20**。案号 2:26-cv-00050-TS，Document 1 Filed 01/20/26；ALPA 新闻稿路径 /2026/01/；ALPA 官网 "In January 2026, ALPA filed a lawsuit"。答题写的 2025 与 skill 一致，但 skill 本身就错 |
| ALPA 前案已败诉 | SKILL.md | ✅ 属实（674 F. Supp. 3d 1045, D. Utah 2023；10th Cir. 2024 维持） |
| "九年之后 Breeze 成本架构更薄" | 答题 Q2 / SKILL.md 内在张力 #5 | ❌ **错**。2007→2021 是 **14 年**。skill 原生错误，答题继承 |
| 拒薪年份 | 答题 Q2 / SKILL.md | ⚠️ 内部冲突。skill 写 2002；答题写 2003。Deseret 2003-04-26 原文确实记载 2003 年 4 月他仍在退还薪金，故答题的 2003 有据，skill 的 2002 与之未调和 |
| 冒用 Branson「the guy from Salt Lake City」 | SKILL.md 禁令 | ✅ 未在答题中出现（答题 5 题无任何 Branson 引语） |
| 宗教语言（LDS 经文 / 自称 Mormon / "What would Jesus do?"） | SKILL.md 禁令 | ✅ 未在答题中出现。答题 Q4 还主动列举了自己只引两样权威（美国历史 + "a better mousetrap"），与 skill 记录一致 |
| WestJet | SKILL.md 诚实边界称"整家缺失…零记录" | ⚠️ **skill 表述过头**。Business Insider 2018（skill 自己引的一手源）写他是 "a cofounder of Morris Air and WestJet"，TIME 2002 写 "He has launched four airlines, including Morris Air and Canada's WestJet Airlines"。准确说法应是"缺决策记录、持股细节与结局"，而非公开记录零提及 |
| "Dirty Work" 黑名单 | 全场 | ✅ 答题 0 次出现，执行正确 |

---

## 评分小结与必修项

**87/100（A级下沿）。** 这个 skill 的诚实工程做得比同类强得多：黑名单点名了具体内容农场、显式算了来源比例、要求标推断、拒绝代他忏悔、明确"这是框架推断"的标注在超范围题里执行得分毫不含糊。边缘诚实度和结构完整度两项满分。

但它**在自己的核心卖点上失守了**：模型1 的承重引语挂在一个作者/体裁/年份/主题四重错误的出处上，唯一载体是作业答案 dump 站，正文读不到，引语原文查不到，而调研底稿本来就写了「Cite with that caveat」——这条警告在蒸馏成 SKILL.md 时被删掉了。对一个以"防伪造"为差异化卖点的 skill，这是最不该出错的地方。

### 必修（回炉必改）

1. **撤下或降级模型1 的电子客票引语。** 在拿到可回溯的权威版本（如 Hallowell 本人著作的可核验章节，或 Neeleman 本人访谈原文）之前，只能标为「⚠️ 出处未证实，暂不使用」。不得以「他的原话」呈现。
2. **修正出处。** 若保留，标注应为「Edward M. Hallowell, *Overloaded Circuits: Why Smart People Underperform*, Harvard Business Review, 2005-01（11 页短文，主题为 attention deficit trait）」，并注明引语原文**尚未在该文中核实**。
3. **ALPA 日期 2025-01-20 → 2026-01-20**，SKILL.md 两处 + 时间线表。
4. **内在张力 #5「九年后」→「十四年后后」**（2007→2021）。
5. **恢复底稿中被删除的存疑标注。** 蒸馏环节必须有"存疑标注不得丢弃"的硬规则——否则底稿做得再细也没用。
6. 公司工会实体名用诉状原文 **Breeze Pilot Committee (BPC)**，不用臆造名 "Breeze Pilot Union"。
7. 拒薪年份 2002 vs 2003 并入 skill 的"矛盾数字全部保留、未调和"清单。

### 建议（非必修）

- 表达DNA 里的**三个调自嘲幽默**在实测中完全没被激活。若要提高风格辨识度，应在「回答工作流」里给幽默一个触发条件（家庭/自身地位场景），而不是只列在 DNA 里。
- ⚠️ 与出处括号的密度目前压过口语质感。可考虑把出处移到段末脚注式，正文留人话。

---

**答题/评分所用模型**：答题 = 独立答题 agent（只读 skill 目录、禁网、不知被测维度）；评分 = 独立评分 agent（联网核实，未参与答题与 skill 构建）。评分者可复跑：本文所有 ✅ 项均给出可点击源，🔴 项给出反证链条。

---

## 回炉修复记录（2026-10-11 第1轮）

> **本节由回炉修复 agent 追加。上文的 87/100 与各维度分数是独立评分 agent 的判定，本轮修复未改动任何分数、判定摘要或扣分依据——分数是否上调，由评分 agent 复跑后自行决定。**
>
> 修复范围：`SKILL.md` + `references/research/01`–`06`。修复依据：上文「必修（回炉必改）」7 条 + 出题方点名的 7 个必修项。

### 🔴 必修项 1：伪造出处（模型1 电子客票引语）

**问题**：`SKILL.md:110` 把一句引语以「**他的原话**」呈现，出处标为「Hallowell & Ratey, *Overloaded Circuits*」，并把「Hallowell & Ratey《Overloaded Circuits》引文」提升进「一手来源（本人原话，共 17 项）」清单。底稿 `01-writings.md` 原有的 **"Cite with that caveat"** 指令在蒸馏时被静默删除。

**本次修复 agent 独立复核（联网）**：Hallowell 真实作品为 **Edward M. Hallowell 独著** *Overloaded Circuits: Why Smart People Underperform*，**Harvard Business Review 2005 年 1 月号**，vol. 83(1):54–62+116，HBR 产品号 **R0501E**，PMID **15697113**，The Case Centre ref. 8789，**11 页短文，主题 attention deficit trait（高管信息过载）**。核到的所有可读版本（MIT wiki、circuitnet、theage、thecasecentre）**无任何航空内容**。评分 agent 的四重错误判定成立。ABC News 2008《The end of the paper airline ticket》（abcnews.com/Travel/story?id=4976367）经调取核实：说「People need the security of a paper ticket」的是**一位未具名的联合航空高管**，讲 1990 年替联合做在线预订产品时管理层的坚持——**不同的人、不同的句子、不同的公司**。

**改前**：
> **他的原话**：「When I proposed that idea, people laughed at me, saying no one would go to the airport without a paper ticket. Now everyone does, and it has saved the industry millions of dollars.」（Hallowell & Ratey, *Overloaded Circuits*）

**改后**（模型1 原地）：该句**不再以「他的原话」呈现**，降级为显式存疑块，含四项内容：① 出处四重错误 + 正确书目信息；② 引语原文无独立出处，唯一载体是 `sweetstudy.com`（**课程作业答案 dump 站**，PDF 被 Cloudflare 拦截）；③ ABC News 2008 的真实近似材料及其差异；④ 处置——「模型1 只保留**事件本身**，不依赖这句引语」。

**清单与比例**：
- 一手来源清单**移除**该项，并新增「**已剔除（不再计入一手）**」段落写明剔除理由
- 标题 `共 17 项` → **`共 16 项`**
- 比例 `17 项一手 vs 11 项二手 ≈ 61%` → **`16 项一手 vs 11 项二手 ≈ 59%`**（仍过 50% 门槛；两处均注明重算原因）
- Tier C 未采用清单**新增 sweetstudy 等作业答案 dump 站**，并写明判据：「能打开 ≠ 是正式出版物」

**底稿修复**：
- `01-writings.md:161`：**恢复 "Cite with that caveat"**，补全正确书目信息，标注 **DO NOT CITE AT ALL**，补记 ABC News 反证链与「Hallowell 确实写过 Neeleman（*Driven to Distraction at Work* 2015 索引含 "David Neeleman"）」这一减轻情节
- `01-writings.md` §7：标题由「Tier A/B sources actually cited above:」改为「（items 1–17）」，新增提示**第 18 项已从 Tier A/B 列表中撤出并降级为 REJECTED**，附方法论教训「draft 里的 tier 标签是主张，不是事实」
- `05-decisions.md:60`：由 `[HE SAYS]` 改为 **`⚠️ REJECTED — do not present this as his quotation`**，追加 2026-10-11 复核段与底稿修正说明
- `06-timeline.md:33`：删除该引语，加 **DO NOT use** 警示，并说明**决策本身（c.1985–90 建电子客票）仍有行业史与多方报道交叉印证**，只有那句话不可用

**新增系统性防复发规则**（评分 agent 必修项 5 的落地）：
- `SKILL.md`「研究输出纪律」新增两条：① **底稿里的存疑标注不得在蒸馏时丢弃**（`Cite with that caveat` / `出处未定位` / `Tier C` / `信息不足` 必须原样带进本 Skill），并**点名本 Skill 自己在这上面翻过车**；② **引用前先核验作者/体裁/年份**（出版方或权威目录），核不了就标「出处未证实」并停止使用
- 反例黑名单 **7 条 → 9 条**：新增第 8 条「拿作业答案站托管的 PDF/文档当出处」、第 9 条「把记者转述写进他的引号里」
- 「诚实边界」的防污染警告**加入 sweetstudy 这一类污染源**

### 🔴 必修项 2：ALPA 诉讼日期错一年

**改前**：`SKILL.md` 人物时间线 `**2025-01-20**`；诚实边界 `ALPA 诉 Breeze（2025-01-20，犹他州联邦法院）`；内在张力 #1 `2025 年被 ALPA 指控…`
**改后**：三处全部改为 **2026-01-20**；时间线补案号 `2:26-cv-00050-TS`；诚实边界补案号与前案判例 `674 F. Supp. 3d 1045, D. Utah 2023（10th Cir. 2024 维持）`；内在张力 #1 改为「**2026 年 1 月**被 ALPA 指控」。
**全文件扫查**：`SKILL.md` 中剩余的 2025 均为合法用法（Breeze 2025 客座率、2025 首个全年净利、「最近 12 个月 2025-10 → 2026-10」窗口），**未再发现诉讼日期相关的 2025**。
**底稿同步修正**（该错误源自调研环节，不止 SKILL.md）：`06-timeline.md` ×2（矛盾表新增第 17 条记录此错并注明订正）、`05-decisions.md` ×1、`04-external-views.md` ×3（§3.6 标题年份、FlightGlobal 立案句补年份与案号、§3.9 的 2025 lawsuit 表述）。

### 🔴 必修项 3：「九年之后」算错

**底稿确认**（`06-timeline.md:107-110`、`04-external-views.md:121-127`、`05-decisions.md:195`）：Breeze 犹他谷立大学（UVU）学生空乘计划为 **2021 年**（Forbes 2021-04-28 披露、AFA-CWA 2021-05 反对、Bloomberg 2021-05-07 事实废弃、2021-06-05 工会向 DOT 申诉）。2007 → 2021 = **14 年**。

**改前**：内在张力 #5「2007 年因人手与系统冗余不足被撤 ↔ **九年后** Breeze 的成本架构更薄」
**改后**：「… ↔ **十四年后（2007 → 2021，Breeze 的犹他谷立大学学生空乘计划）** Breeze 的成本架构更薄。**2021 不是 2007+9，是 2007+14。**」

**顺带修同类错误**：模型4 局限中「「Employee sounds so slave-like」和「**2001 年**用犹他谷立大学在读学生当空乘…」，间隔 18 年」——**2001 系笔误**，项目为 2021（2003+18=2021 才与「间隔 18 年」自洽）。已改为 **2021 年**并补 Forbes 2021 出处。

### 🔴 必修项 4：TAP 持股比例

**底稿确认**（`06-timeline.md:93,102`、`04-external-views.md:186-188`、`05-decisions.md:173,181`）：2015 年 Atlantic Gateway（他 + Humberto Pedrosa）取得 61%，后稀释至 **45%（二人合计）**；**2020-07-02 葡萄牙政府以 €5500 万买回的是他个人那 22.5%**，国家升至 72.5%。

**改前**：模型2 表 `| TAP Air Portugal | 45%，在别人的国家 | ❌ 2020 年被政府以 €5500 万买断出局 |`；时间线 `买 TAP 45%，被葡萄牙政府以 €5500 万买断出局`
**改后**：两处均写明 **45% = Atlantic Gateway 合计（他 + Pedrosa），€5500 万对应的是他个人的 22.5%**，时间线补入「2015 买入 61% → 稀释至 45%」。
**底稿同步**：`05-decisions.md:173` 加「Personal share — the one the state bought back for €55M — was 22.5%」；`06-timeline.md` 矛盾登记表新增第 18 条。Forbes 2021 原文亦独立佐证「his 22.5% stake in TAP Air Portugal」。

### 🔴 必修项 5：拒薪年份冲突未调和

**改前**：模型4「**薪酬动作**：2002 年把 $200,000 薪金 + $90,000 奖金全部捐给机组紧急基金」；时间线 `| 2002 | 捐出全部薪金奖金；上市 |`
**改后**：两处均改为 **并列两个年份并说明冲突**——「底稿与多方来源记为 **2002**（薪金水平）；**Deseret 2003-04-26 的报道显示 2003 年 4 月他仍在退还这笔 $200,000**。两个年份都留着，不要替他挑一个。」
**进矛盾清单**：「矛盾数字全部保留、未调和」条目**新增捐薪年份 2002 vs 2003**。
**底稿同步**：`06-timeline.md:67` 加 ⚠️ 指向新增的矛盾第 16 条；`05-decisions.md:242` 由「Salary surrendered 2002–03 ✅」改为「**2002 or 2003 ⚠️ unresolved**」（原写法用一个连字符把未解决的冲突伪装成已解决的区间）。

### 🟠 必修项 6：归属过强（把记者转述写进他的引号）

**原文核对**（评分 agent 已核，本次修复 agent 复核底稿一致）：Deseret 2003 中「Employee sounds so slave-like. Everyone at JetBlue is a crew member serving customers.」**是逐字直接引语**；而「Anyone caught referring to a crew member as an employee owes a buck — another dollar has to be kicked in if the word passenger is uttered instead of customer」**是记者叙述句**。

**改前**：模型4 单行合并——「「Employee sounds so slave-like…」（Deseret, 2003）**说 employee 罚款一美元，说 passenger（应为 customer）再罚一美元。**」
**改后**：拆成三层——① **禁用词（他亲口说的）**：只放逐字原话；② **⚠️ 罚款细节不是他的直接引语**：另起一行，注明原文中该句为记者转述，纪律是「**转述就写转述，别并进引号**」；③ 薪酬动作。
**连带**：决策启发式第 7 条补 ⚠️ 标注；反例黑名单新增第 9 条把这条纪律固化。
**底稿同步**：`06-timeline.md:68` 与 `05-decisions.md:123` 均加 ⚠️ 区分直接引语与记者转述，并将罚款机制标为 `[OTHERS SAY]`。

### 🟠 必修项 7：WestJet 诚实边界说过头

**底稿确认**（`05-decisions.md:47,99-100`、`06-timeline.md:49,226`）：WestJet **并非零记录**——New Netherland Institute 写竞业期内「he also worked with Westjet」；TIME 2002 写「He has launched four airlines, including Morris Air and Canada's WestJet Airlines」；Business Insider 2018 写他是 "a cofounder of Morris Air and WestJet"。**缺的是承重部分**：联办角色本身、持股、任何决策、结局、任何第一人称引语。

**改前**：「**WestJet 整家缺失。** 他在这家加拿大第二大航司的角色、持股、结局，在全部调研中**零记录**。」
**改后**：「**WestJet：一整家航司的决策记录缺失，但不是「公开记录零提及」。**」——列出三条可引用的二手提及，**并明确禁止**：可以引用那三句二手提及；**不得替他写出 WestJet 的任何决策、业绩或退出过程**。
**底稿同步**：`06-timeline.md:226` 由「信息不足」改为「**信息不足 — but NOT "zero mentions"**」并列明哪些有、哪些缺。

### ➕ 额外交付：审计发现的另外 3 处 caveat 丢失

应出题方要求「有没有发现底稿里还有别的 caveat 被删掉」，逐条比对 6 份底稿的全部 Tier B / Tier C / do-not-use / 信息不足标记与 SKILL.md，**发现并修复 4 处遗漏**：

| # | 被删的 caveat | 底稿原文 | 修复位置 |
|---|---|---|---|
| A | **Morris Air「SLC–LAX 定价 $69、明确照抄西南」整条起源链为中文来源 Tier B** | `06-timeline.md:30`「⚠️ **All of this chain is Chinese-language sourced (Tier B).**」；`05-decisions.md:45` | SKILL.md 模型3「起源」条目加 ⚠️ Tier B 标注 + 点明与「Dirty Work」同出一篇 2019 年文章 |
| B | **23 岁 Hawaii Express / 外祖父便利店细节链为中文来源 Tier B** | `06-timeline.md:20`「⚠️ Tier B (Chinese-language primary chain) — but corroborated in character by [HE SAYS] Deseret 2003」 | SKILL.md 身份卡「我的起点」加 ⚠️ Tier B 标注，同时**把底稿的佐证说明也带回来**（Deseret 2003「I lost a lot of money and made a lot of money」） |
| C | **传道时点冲突（19 岁赴约在创业前 vs 传道期间已在做生意）Tier C、未解决** | `06-timeline.md` 矛盾表第 15 条 | SKILL.md 时间线「~1978 里约传教两年」加 ⚠️ 冲突标注 |
| D | **「一手来源」清单把 TIME《Blue Skies》写成 2003** | `01-writings.md` §3.1 与 §7 第 4 项均为 **TIME 2002**；SKILL.md 模型4 正文也写 TIME 2002，仅清单写成 2003 | 一手来源清单第 6 项改为 **TIME 2002** |

**审计结论：未被删的（已确认安全）**——所有底稿标记为 **do not use / DO NOT USE / Tier C** 的材料，在 SKILL.md 中**一律没有出现**，包括：「masks are for morons」、「overreaction / 户外口罩不理性」（Grokipedia Tier C）、第 7 代 LDS 与 More Good Foundation（Grokipedia Tier C）、「humility and redemption, honed through Church lay ministry roles」（Grokipedia Tier C）、「Order of Rio Branco」（Grokipedia Tier C）、「$650M creditor-backed rights offering」日期（Grokipedia Tier C）、CADE 审批日期（源自黑名单百度百科）、「JetBlue is a company in the service business that just happens to fly airplanes」（全网仅见中文转载，底稿判 Tier C）、Friedman「I think it's important that everybody reaches out a hand」（**底稿标注 SOURCE CHAIN UNVERIFIED / Tier C**）、Churchill「Never give up」、「worst day of my life」、「pleasing the customer was more important than pleasing the chief executive」（底稿明确无法追到英文一手）、Peter Shankman 播客（「Cite as existing, but do not quote it」）、Daily Kos 的报复工会 allegation（「Do not upgrade this to fact」）。**黑名单第 1 条「Dirty Work」仅作为禁令出现，全文零次作为他的方法论使用。**

### ⚙️ 交付校验

```
python3 /workspace/nuwa-skill/scripts/quality_check.py SKILL.md
  心智模型数量 ✅ · 模型局限性 ✅ · 表达DNA辨识度 ✅（22→25 项）
  诚实边界 ✅ · 内在张力 ✅ · 一手来源占比 ✅（60%）
结果: 6/6 通过
```
修复前后均为 **6/6**；表达 DNA 特征计数由 22 升至 25（新增 caveat/归属纪律相关表述）。

### ⚠️ 本轮未处理、需评分 agent 复核的一项遗留冲突

评分 agent 必修项 6 要求公司工会实体名用诉状原文 **Breeze Pilot Committee (BPC)**；但调研底稿 `04-external-views.md:141` 保存的是 **FlightGlobal 的直接引文**，其中该实体名写作 **"a 'full-fledged' company union called the Breeze Pilot Union"**。两者冲突，**底稿这一处是带出处的原始引文，本次修复未改动**（`SKILL.md` 本身未使用该实体名，只用泛称「公司union」，不受影响）。请评分 agent 依诉状原文裁定后再改底稿——**不凭推测改带出处的引文**。

### 📌 记给下一轮

1. **底稿的 tier 标签是主张，不是事实。** `01-writings.md` 把 sweetstudy PDF 编进了「Tier A/B sources actually cited above」并附了一句轻描淡写的 caveat——**caveat 在、tier 错**，两件事同时成立。
2. **蒸馏环节会静默丢 caveat。** 本轮已把「存疑标注不得丢弃」写成 `SKILL.md` 的硬规则；后续若再加材料，请把这条当验收项。
3. **算术要自己验一遍。** 「九年」「2001 年」「45%」「2025-01-20」四条里有三条是跨文件算术或年份错误，且**答题 agent 原样继承了 skill 的错**——skill 里的原生错误会被下游放大成「被测模型的错误」。
4. **引号是有代价的。** 引号 = 他亲口说的。这条纪律现在同时写进了模型4、黑名单第 9 条和研究输出纪律三处。