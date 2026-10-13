# ADHD Persona Skills · 女娲蒸馏集

用 [女娲 · Skill造人术](https://github.com/alchaincyf/nuwa-skill) 流程蒸馏的 ADHD 认知模型 Skill 集。

**3 个人物视角 + 3 个主题框架。每一份都带独立 agent 的保真度评分卡。**

---

## ⚠️ 使用前必读：这是健康领域

本仓库收录的 skill **不做诊断**，不评估任何人是否符合 ADHD（**包括说话者自己**），
不涉及药物、剂量、停药、加药的任何建议，一律转向专业医生。

`adhd-work-and-environment-fit` 与 `adhd-women-and-gender-gap` 另有更严格的约束：
**不做个人职业推荐**（前者）、**不提供量表判读路径**（两者）。
这些不是免责声明文字，而是写进了 Skill 的 `Step 0 安全门` 和 `CHECKPOINT`，会实际触发拦截。

---

## 收录清单

### 人物视角（3）

| Skill | 人物 | 定位 | 保真度 |
|---|---|---|---|
| `ned-hallowell-perspective` | Ned Hallowell | 精神科医生 · 临床框架层 | 84/100 · B |
| `jessica-mccabe-perspective` | Jessica McCabe | How to ADHD 创始人 · 个体实操层 | **90/100 · A** |
| `david-neeleman-perspective` | David Neeleman | 捷蓝创始人 · 组织配置层 | 87/100 · A |

三人的选法不是按名气，是按**层级**——临床框架 / 个体实操 / 组织配置，互不重叠。

### 主题框架（3）

| Skill | 回答的问题 | 保真度 |
|---|---|---|
| `adhd-cognitive-operating-system-framework` | 注意力到底怎么运作？各学派分歧在哪？ | 85/A · 84/B（双独立评分，分差 1） |
| `adhd-women-and-gender-gap` | 为什么女性被系统性漏诊？ | 82/100 · B |
| `adhd-work-and-environment-fit` | 什么环境能让人发挥？「我有 ADHD 所以适合 X」成立吗？ | **85/100 · A** |

---

## 安装

每个 skill 目录**自包含**，复制后即可独立使用，不依赖本仓库外部文件。

```bash
# Claude Code
git clone https://github.com/lixvanran/adhd-persona-skills.git
cp -r adhd-persona-skills/skills/* ~/.claude/skills/

# Codex / Cursor / 其他兼容 runtime
cp -r adhd-persona-skills/skills/* <your-runtime>/skills/
```

然后在对话里说「用 McCabe 的视角看看」「用 Hallowell 怎么理解」即可激活。

---

## 这个仓库的立场

**我们收录的不是「ADHD 名人名单」，而是可运行、可追溯、可证伪的思维框架。**

所以每一份 skill 里都有三样东西：

1. **心智模型 + 决策启发式** —— 可运行的认知操作系统
2. **诚实边界 + 内在张力** —— 明确写清它做不到什么、哪里还在吵
3. **调研底稿 + 保真度评分卡** —— 全部来源可回溯，分数由**独立于构建者的 agent** 打出

---

## 蒸馏过程中被推翻的内容

这个仓库最有价值的部分可能不是 skill 本身，而是**它们记录了哪些流行说法经不起查证**。

调研与修复阶段累计推翻或更正了 **19+ 条**前提，其中相当一部分是 ADHD 领域里被广泛转引的：

| 内容 | 结论 |
|---|---|
| Wilmot et al. 2011, *Nature Neuroscience* | **五库检索全 0 命中**；DOI `10.1038/nn.2798` 实为一篇视网膜神经发生论文 |
| 「Bellvue et al. 2021」 | 四库无法确证，疑误认 Mark A. Bellgrove |
| 「Deficiency-Deficit Framework」 | PubMed 全库 0 命中 |
| 「VAST 由 Barkley 共同提出」 | VAST 由 Carrie Feibel 提出，被 Hallowell & Ratey 采用，**Barkley 是公开批评者** |
| 「jagged cognitive profile」 | 四条检索路径零命中，无同行评议版本；Wilson 2023（1800+ 人）结论方向相反 |
| ADHD 十点量表「5-8 分为甜蜜点」 | **零验证** —— 无信度、无效度、无常模、无独立重复验证 |
| Frances「最小的孩子几乎是两倍」 | NEJM n=407,846 实测 **1.34 倍** |
| 「Kazda 2021 无性别分层数据」 | 该文 Q1 下有 Sex 子类 25 项 —— 但那是**诊断率不是漏诊率** |
| Rothenberger 是 Sonuga-Barke 的批评者 | 长期**合著者**，PubMed 共同署名 58 篇 |
| ASAN 成立于 1997 年 | 成立于 **2006 年** |

完整清单见 [`docs-batch3.md`](docs-batch3.md) 与各 skill 的《反例黑名单》章节。

---

## 方法论

本仓库的蒸馏流程与踩坑记录见 [`METHODOLOGY.md`](METHODOLOGY.md)，包括：

- 合成阶段会吃掉调研底稿的限定词（出现 4 次）
- 引语坐标全量核对比抽查多发现 50% 以上的错误
- 修复 agent 自身会引入新错误
- 搜索「人名 criticism」会返回 AI 内容农场捏造引语

---

## 致谢

- [女娲 · Skill造人术](https://github.com/alchaincyf/nuwa-skill) — 蒸馏流程与保真度评分卡
- 各 skill 调研涉及的全部被访谈者与文献作者

## License

MIT
