# 任彦舟 · Yanzhou Ren

**AI Agent · RAG · AI Backend**

你好，我是任彦舟，目前在电子科技大学攻读软件工程硕士。我关注 Agent 如何可靠地执行长任务、如何组织上下文，以及如何把检索到的资料变成可追溯的知识。

写一点想法，做一些有意思的工具。这里收集了我的开源作品，也记录了从问题到实现的过程。

[个人网站](https://ren-yanzhou.pages.dev) · [简历 PDF](https://ren-yanzhou.pages.dev/assets/resume.pdf) · [邮件联系](mailto:2675528281@qq.com)

## 正在构建

### [Roc](https://github.com/ryzqi/Roc) · 科研工作台与 Agent 运行时

让长任务记住进展，接着往前。围绕科研场景，把文献、研究助手、知识库和写作放在同一个工作台中。

- 基于 LangGraph / deepagents 组织规划、工具执行与子 Agent 协作，通过检查点和操作回执支持暂停与恢复。
- 分层整理上下文，保留约束、待办与证据位置；结合全局和项目级记忆，支持按需回读。
- 接入 MCP、Skills 与文件、命令、检索工具，关注工具授权、执行边界和回归评测。

`TypeScript` `LangGraph` `deepagents` `SQLite` `Electron` `React`

### [CogniWeb](https://github.com/ryzqi/RAG-Research-Workbench) · 多知识库问答与 Deep Research

让线索相连，让知识可循。从一个问题出发，把检索、核验与写作组织成带引用的研究报告。

- 多知识库隔离与联合检索，结合父子分块、Dense + BM25、RRF 融合与可选 Rerank。
- 使用 LangGraph 编排查询改写、问题拆解与反思补检；通过 deepagents 协作完成检索、主张核验和章节写作。
- 使用 FastAPI + Celery 执行异步任务，通过 SSE 展示进度，保存计划、证据清单与报告，支持回溯和导出。

`Python` `FastAPI` `Celery` `LangGraph` `Milvus` `PostgreSQL` `Redis`

## 边做，边写，边理解

### [learn-agent](https://github.com/ryzqi/learn-agent) · 20 章中文 Agent 架构实战

从一个最小的 Agent Loop 开始，逐章加入工具、权限、上下文、记忆与多 Agent 协作，最后组合成完整的 Harness。每章配有可一起阅读和运行的 TypeScript 代码。

| 阶段 | 主题 |
| --- | --- |
| 01–04 · 执行基础 | Agent Loop、工具与文件、权限、Hook |
| 05–10 · 上下文与知识 | 计划、子 Agent、Skills、上下文压缩、记忆 |
| 11–14 · 可靠执行 | API 恢复、任务 DAG、后台任务、Cron |
| 15–18 · 协作与隔离 | Mailbox、协作协议、SQLite 认领、Worktree |
| 19–20 · 扩展与总装 | MCP 工具池、完整 Harness |

[阅读文章与源码](https://github.com/ryzqi/learn-agent#20-章地图) · [在个人网站浏览目录](https://ren-yanzhou.pages.dev/#writing)

## 常用工具

- **语言：** Python、TypeScript
- **Agent 与后端：** LangGraph、deepagents、MCP、Skills、FastAPI、Celery
- **数据与检索：** PostgreSQL、Redis、SQLite、Milvus、BM25、RRF
- **关注方向：** Agent 编排与恢复、上下文与记忆、Agentic RAG、证据引用、执行安全与评测

## 一点背景

- **电子科技大学 · 软件工程**：硕士在读（2026–2029，预计）；本科（2022–2026），GPA 3.93/4.0。
- **知道创宇 · AI 研发实习生**（2025.08–2026.01）：参与多模态安全研发，负责模型服务化、LoRA SFT、评测与安全检测流程。
- **2025 中国大学生计算机设计大赛 · 国家一等奖**。

欢迎交流 Agent、RAG、开源，或一个值得琢磨的问题：**[2675528281@qq.com](mailto:2675528281@qq.com)**。

保持好奇，继续构建。
