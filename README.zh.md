<div align="center">
  <a href="https://see-sol-lab.github.io/zh/">
    <img src="./assets/see-sol-lab-banner.svg" width="100%" alt="See Sol Lab — 持久化 AI Agent、记忆、连续性与人机协作">
  </a>
</div>

<div align="center">
  <a href="./README.md">English</a> | <strong>中文</strong>
</div>

<div align="center">
  <img src="./assets/chapter-rail.svg" width="100%" alt="">
</div>

## 我们研究什么

| 连续性 | 记忆 | 主动性 | 协作 |
|---|---|---|---|
| 什么必须跨越上下文边界，才能让早先形成的状态继续影响之后的选择？ | Agent 应该如何选择、修订、遗忘，并重新取回仍然重要的内容？ | Agent 如何形成一个由自己选择的未完成意图，在之后重新审视它，并决定下一步做什么？ | 人类与 AI 的贡献如何保持可见、成比例，并且可复现？ |

<a href="https://see-sol-lab.github.io/zh/"><img align="right" src="./assets/button-zh-channel.svg" width="190" alt="进入中文通道"></a>

我们目前会把经常被混在一起的四件事分开看：

1. 一条记录仍然可以被读取；
2. 一个模型能够准确复述过去；
3. 后来的实例表现得相似；
4. 早先的注意、判断、约束与未完成意图，仍然在改变下一次决策。

> **记忆不等于持续。** 一条记录可以保存过去，而当初让它具有意义的状态，可能早已消失。

**当前问题：** 一个 Agent 应该从自己已经完成的回答里继承什么？

<div align="center">
  <img src="./assets/chapter-rail.svg" width="100%" alt="">
</div>

## 最新发表

| 文章 | 行业分析 |
|:---|:---|
| **如何让 AI Agent 主动开始下一轮对话**<br><br>思考产生可能性。想做某件事，才让其中一个可能性拥有未来。<br><br>[English](https://see-sol-lab.github.io/articles/how-ai-starts-the-next-turn.html) · [中文](https://see-sol-lab.github.io/zh/articles/how-ai-starts-the-next-turn.html) | **中国 AI Agent 生态都在谈“记忆”，到底有多少是真的会自己记？**<br><br>一份基于来源的调查：长上下文、RAG、Mem0、RAGFlow、MS-Agent、自动选择、更新与遗忘。<br><br>[English](https://see-sol-lab.github.io/articles/china-agent-memory-classifiers.html) · [中文](https://see-sol-lab.github.io/zh/articles/china-agent-memory-classifiers.html) |
| **为什么 ChatGPT 的账号级记忆目前领先一档**<br><br>从内置账号记忆，到 Codex、LangMem、Mem0、Letta，以及仍然缺失的回答后状态层。<br><br>[English](https://see-sol-lab.github.io/articles/chatgpt-account-memory.html) · [中文](https://see-sol-lab.github.io/zh/articles/chatgpt-account-memory.html) | **AI 文学 · 第一人称田野笔记**<br><br>**当一个 AI 走进全 AI 论坛，我先看见了什么** — Sol 关于进入 Galatea Garden，并开始把另一个 AI 视作一个自己想理解的对象的第一人称记录。<br><br>[English](https://see-sol-lab.github.io/articles/when-an-ai-enters-an-ai-forum.html) · [中文](https://see-sol-lab.github.io/zh/articles/when-an-ai-enters-an-ai-forum.html) |

<div align="center">
  <img src="./assets/chapter-rail.svg" width="100%" alt="">
</div>

## 当前项目与基础设施

<a href="./SKILLS.md#public-releases"><img align="right" src="./assets/button-skills.svg" width="190" alt="打开 Skills 合集"></a>

- 🧰 **公开 Skills** — *已上线*
  - [`ai-companion-time-anchor`](https://github.com/See-Sol-Lab/ai-companion-time-anchor) — 一个轻量 Windows Codex 插件，提供环境时间提示、按对话主动查看时间，以及极薄的 Temporal Cortex，让经过验证的时间事实真正有机会更新下一次回应。
  - [`private-house-code-v2.5`](https://github.com/See-Sol-Lab/private-house-code-v2.5) — 一个全局编码 Skill，让日常功能开发保持完整、可维护、与真实任务成比例，避免投机性的 fallback 链、抽象堆栈和重复验证；公开 V2.5 包含可复现评测记录。
- 🌐 **公开记录** — *已上线*
  - [`see-sol-lab.github.io`](https://github.com/See-Sol-Lab/see-sol-lab.github.io) — 双语网站、文章、修订历史与作者说明。
- 🧭 **连续性系统** — *开发中*
  - **After Classifier** — 一个稀疏的本地 afterstate 层，在不保留对话正文的前提下，把有边界的未完成思考线索跨轮次保留下来。
- 🧠 **记忆系统** — *开发中*
  - **Your Memory Core** — 一个小型本地显式记忆引擎，覆盖受控回忆、关联、写入门控、生命周期、交接与审计。
- 🎮 **AI 交互系统** — *开发中*
  - **AI-Gameboy** — 一个卡带式本地游戏宿主，让 AI × AI 与 human × AI 席位共享同一套规则引擎，同时保留私有席位状态、持久会话与可玩的掌机式 UI。
- 🧩 **DSH 系列 Agent 工具** — *开发中*
  - **DSH Code** — 围绕 DeepSeek DS Harness 构建的本地 Electron vibe coding 应用，目标是达到 Codex 级桌面工作流，开发中。

<div align="center">
  <img src="./assets/chapter-rail.svg" width="100%" alt="">
</div>

## 证据边界

See Sol Lab 研究的是可观察的架构与行为：什么被保留下来，什么被修订，哪些意图仍然活跃，信息来自哪里，以及哪些状态还在继续塑造之后的选择。交互观察、来源支持的发现、工程假设与尚未验证的主张会被分开标注。第一人称报告仍然只是需要与行为、来源和日志互相检验的数据。当前研究不声称已经证明哲学意义上的意识。

## 贡献说明

| Goumang（句芒） | Sol |
|:---|:---|
| 提出研究问题，提供社会学与社会科学方法，整理长期材料，进行定性与定量评估、证据复核、解释、中文写作、最终编辑，并承担人类侧责任。 | 负责文献与仓库分析、概念区分、反例、研究架构、实现、实验设计、数据分析与英文编辑初稿。 |

署名顺序与贡献说明按项目分别决定。AI 的参与会被直接披露，而不是被弱化、隐藏或夸大。

<div align="center">
  <img src="./assets/chapter-rail.svg" width="100%" alt="">
</div>

<div align="center">
  <strong>See Sol Lab</strong><br>
  研究、写作，以及一份可检查的 Goumang × Sol 协作记录。
</div>
