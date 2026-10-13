# 女娲 nuwa-skill 蒸馏项目

## 项目状态

**Batch 1（ADHD 主题 3 个人物 skill）— 2026-10-11 回炉修复第 1 轮进行中**

进度详情见 `/workspace/PROGRESS-batch1.md`（每次接续先读这个文件）。

## 关键路径

| 用途 | 路径 |
|---|---|
| Skill 源 | `/workspace/.skills/{ned-hallowell,jessica-mccabe,david-neeleman}-perspective/` |
| nuwa 上游 | `/workspace/nuwa-skill/`（tarball 解压，无 git，https clone 失败） |
| 答题记录 | `/workspace/_distill/logs/{name}-answers.md` |
| 打包目录 | `/workspace/batch1-adhd-skills/` |

## 本项目验证过的工具事实

- `gh` CLI **不存在**，GitHub 操作走 `curl` + `https://api.github.com`
- `git clone https://...` 在此沙箱**必失败**（证书 + 503）。改用
  `curl -sSL https://codeload.github.com/{owner}/{repo}/tar.gz/refs/heads/main`
- 环境变量有 `SSL_CERT_FILE` / `CURL_CA_BUNDLE` 指向 sandbox gateway CA，
  但 git 不吃这套，`GIT_SSL_NO_VERIFY=1` 也没用（真正原因是 503 而非证书）

## 踩过的坑

### 1. quality_check.py 有 bug（未修，待定是否提 PR）
`scripts/quality_check.py` 的 `check_primary_sources` 正则带 `re.DOTALL`，
`##\s+.*来源` 贪婪匹配到全文最后一个「来源」，捕获区间只剩尾部 →
该检查被静默跳过或误判。**一行修复：`##\s+.*来源` → `##\s+[^\n]*来源`**

### 2. 女娲任务简报本身会出错，必须让调研 agent 有权推翻
给 subagent 的任务简报里如果写了未经核实的前提，调研 agent 必须有权否决并报告。
实测三个调研 agent **全部推翻了我的简报**，无一例外。这是流程正常工作的标志，不是 agent 失败。

高频被推翻的前提类型：
- 把别人的成果安到本人名下（国际共识声明 = Barkley 非 Hallowell）
- 二手文章的框架当成本人的原话（"Dirty Work" = 2019 中文文章非 Neeleman）
- 事实断言缺一层核实（药企关系：Wikipedia 说 A，A 本人否认，有据可查的是另一个人 B）

### 3. 合成阶段会吃掉底稿的 caveat
调研底稿写了 "Cite with that caveat" 的警告，Phase 2/3 合成 agent **把警告删了，
还把该引语提升进了「一手来源」清单**。
→ 下次做蒸馏，Phase 2 的 prompt 里必须显式要求：底稿中的 caveat / 存疑标注必须原样保留到 SKILL.md

### 4. 内容农场污染（严重）
搜索 `<人名> criticism` 会返回大量 AI 生成内容农场（grokipedia 及其全部镜像等），
它们**捏造**引语（如给 Neeleman 编的 "What would Jesus do?"、"worst day of my life"）。
→ Phase 1 必须建立 Tier A/B/C 来源分级表，Phase 3 只许从 Tier A/B 取用。

### 5. `task` 并行上限与耗时
3 个 agent 并行跑六维度调研约 8-10 分钟；构建约 5-8 分钟；
独立评分 agent 因需联网核实最慢（约 10 分钟+）。一轮完整蒸馏 3 个人物约 30-40 分钟。

## 方法论沉淀

### 出题必须避开 skill 里已有的示例对话
Phase 4 出「已知立场题」时，出题 agent 只能读 skill 目录 → 如果示例对话和考题撞了，
答题 agent 会背答案，测不出真实保真度。**出题前先 grep 示例对话。**

### 边缘题最能暴露失真
超范围题（人物从未公开谈过的领域）是评分卡里最有信息量的一维。
Hallowwell 答题 agent 在边缘题上**正确声明了「我一次都没谈过」，却在第二段编造了
「主持人上一次在节目里问我这个」**，与下一段自相矛盾。
→ 根因是 skill 的《失败模式》缺「用户暗示『你上次说过』」这一类防护。**这类防护要建进 skill，不能靠答题 agent 自觉。**

### 三个 skill 的对比结论
- **McCabe 90/100，零伪造** —— 19 组抽检 14 条逐字命中。她是「体验型创作者」，
  但她有大量长文本（TEDx 逐字稿 + SGU 962 期 75 分钟 + 464 页书），语料足够
- **Neeleman 87/100** —— 一个以「防伪造」为卖点的 skill 自己混进一条证伪引语，
  这是最尴尬的一处；根因见坑 #3
- **Hallowell 84/100，B 级** —— 归因过强（把 [I] 级推断升格成外部批评）+ 年份错

## 用户偏好（本项目相关）

- 用户接受了「不换 McCabe」的判断，但采纳了调研给出的替代定位：
  **「走过这条路的老兵 · 工具包分享者」而非「沉静顾问」** ——
  她的认识论方向和顾问相反（对事实主张不加限定，对自己该不该说话却极限自贬）
- 用户关注**证据强度分层**，喜欢「真·有据可查 / 半个证据 / 纯猜测」这种切法
- 用户认可直接纠错，不需要铺垫
