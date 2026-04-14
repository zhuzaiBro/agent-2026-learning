# 2026 AI Agent 开发学习路线图

---

## 🗺️ 总览

```
阶段一 ➜ 阶段二 ➜ 阶段三 ➜ 阶段四 ➜ 阶段五 ➜ 阶段六 ➜ 阶段七
Python   LLM基础   Prompt    RAG      Agent    MCP/    项目实战
基础     & 生态     Engineering 知识增强   智能体    工程化   & 面试
(2周)    (3周)      (2周)      (3周)     (4周)    (2周)    (持续)
```

---

## 阶段一：Python 编程基础（约 2 周）

> 目标：能读懂和编写基础 Python 程序，为后续 AI 开发打底。

| 主题 | 要点 |
|------|------|
| Python 基础语法 | 变量、数据类型、控制结构 |
| 数据结构 | 列表、字典、集合、元组 |
| 函数与模块 | 函数定义、模块导入、包管理 |
| 面向对象编程 | 类、继承、多态、封装 |
| 数据处理三件套 | NumPy、Pandas、Matplotlib |

### 免费学习资源

- [Python 官方教程（中文）](https://docs.python.org/zh-cn/3/tutorial/)
- [廖雪峰 Python 教程](https://www.liaoxuefeng.com/wiki/1016959663602400)
- [菜鸟教程 - Python3](https://www.runoob.com/python3/python3-tutorial.html)
- [Kaggle - Python 免费课程](https://www.kaggle.com/learn/python)
- [NumPy 官方入门教程](https://numpy.org/doc/stable/user/quickstart.html)
- [Pandas 官方入门教程](https://pandas.pydata.org/docs/getting_started/intro_tutorials/)
- [Matplotlib 官方教程](https://matplotlib.org/stable/tutorials/index.html)

---

## 阶段二：大语言模型（LLM）基础 & 生态（约 3 周）

> 目标：理解 LLM 的工作原理、Transformer 架构、以及开源生态全貌。

### 2.1 AI & 深度学习核心概念

| 主题 | 要点 |
|------|------|
| 机器学习基础 | 有监督/无监督/强化学习、特征工程 |
| 神经网络 | 前向传播、反向传播、梯度下降、损失函数 |
| CNN & RNN | 卷积网络、循环网络、LSTM |
| NLP 基础 | 词嵌入 Word2Vec、seq2seq、Attention 机制 |

### 免费学习资源

- [3Blue1Brown 神经网络系列（YouTube/B站）](https://www.youtube.com/playlist?list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi)
- [吴恩达 机器学习课程（Coursera 免费旁听）](https://www.coursera.org/learn/machine-learning)
- [吴恩达 深度学习专项课程（Coursera 免费旁听）](https://www.coursera.org/specializations/deep-learning)
- [李宏毅 机器学习 2023（YouTube/B站）](https://www.youtube.com/playlist?list=PLJV_el3uVTsPy9oCRY30oBPNLCo89yu49)
- [Stanford CS224N NLP 课程](https://web.stanford.edu/class/cs224n/)
- [动手学深度学习（Dive into Deep Learning）](https://zh.d2l.ai/)

### 2.2 Transformer & LLM 原理

| 主题 | 要点 |
|------|------|
| Transformer 架构 | Encoder-Decoder、Self-Attention、多头注意力、位置编码 |
| KV 缓存 | 推理优化核心机制 |
| 预训练 & 微调 | Pre-training、Fine-Tuning、RLHF |
| 大模型技术前景 | Scaling Law、涌现能力 |

### 免费学习资源

- [Attention Is All You Need 原始论文](https://arxiv.org/abs/1706.03762)
- [The Illustrated Transformer（Jay Alammar）](https://jalammar.github.io/illustrated-transformer/)
- [The Illustrated GPT-2](https://jalammar.github.io/illustrated-gpt2/)
- [Andrej Karpathy - Let's build GPT from scratch](https://www.youtube.com/watch?v=kCc8FmEb1nY)
- [Hugging Face NLP 课程（免费）](https://huggingface.co/learn/nlp-course)
- [LLM Visualization（3D 可视化）](https://bbycroft.net/llm)

### 2.3 大模型生态 & 选型

| 主题 | 要点 |
|------|------|
| 开源生态 | 分层架构：模型层→推理层→开发框架层→应用编排层→代理系统层 |
| 主流开源模型 | Qwen、DeepSeek、LLaMA、Mistral、GLM 等 |
| 推理系统 | vLLM、SGLang、Ollama |
| 模型评估 | Multiple Choice、Verifier、Leaderboard、LLM Judge |
| 模型选型 | 选型原则与流程 |

### 免费学习资源

- [Hugging Face 模型库 & 文档](https://huggingface.co/docs)
- [Ollama 官方文档（本地运行开源模型）](https://ollama.com/)
- [vLLM 官方文档](https://docs.vllm.ai/)
- [Open LLM Leaderboard](https://huggingface.co/spaces/open-llm-leaderboard/open_llm_leaderboard)
- [LMSYS Chatbot Arena](https://chat.lmsys.org/)
- [大模型开源生态全景图 - Awesome LLM](https://github.com/Hannibal046/Awesome-LLM)

---

## 阶段三：提示工程 Prompt Engineering（约 2 周）

> 目标：掌握 Prompt 设计方法论，能系统化地与 LLM 交互。

| 主题 | 要点 |
|------|------|
| 提示词核心结构 | 系统提示、角色扮演、上下文提示 |
| 高级推理技术 | CoT 思维链、Self-Consistency、ToT 思维树、ReAct 框架 |
| 输出控制 | 采样参数（Temperature/Top-P）、长度控制、惩罚机制 |
| 工程化实践 | Jinja2 模板、PromptOps 版本管理、自动化评测 |
| C.L.E.A.R 原则 | 提示词层级进化与高级技巧 |

### 免费学习资源

- [OpenAI Prompt Engineering 官方指南](https://platform.openai.com/docs/guides/prompt-engineering)
- [Anthropic Prompt Engineering 指南](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/overview)
- [Google Prompt Engineering 白皮书](https://services.google.com/fh/files/misc/gemini-for-google-workspace-prompting-guide-101.pdf)
- [Prompt Engineering Guide（DAIR.AI）](https://www.promptingguide.ai/zh)
- [Learn Prompting（免费交互式课程）](https://learnprompting.org/docs/intro)
- [LangChain Hub（Prompt 模板库）](https://smith.langchain.com/hub)
- [Jinja2 官方文档](https://jinja.palletsprojects.com/)
- [Chain-of-Thought 论文](https://arxiv.org/abs/2201.11903)
- [Tree of Thoughts 论文](https://arxiv.org/abs/2305.10601)
- [ReAct 论文](https://arxiv.org/abs/2210.03629)

---

## 阶段四：知识增强 RAG（约 3 周）

> 目标：构建端到端 RAG 系统，掌握从文档处理到检索生成的全流程。

### 4.1 RAG 基础

| 主题 | 要点 |
|------|------|
| RAG 概述 | 标准流程、关键技术点、全流程架构 |
| Embedding 向量表示 | 语义向量、维度选择、距离度量 |
| 向量数据库 | Milvus、Chroma、Pinecone、Qdrant、Weaviate 选型 |
| 文档处理 | 分片策略（Chunking）、向量化、索引构建 |

### 免费学习资源

- [RAG 入门指南 - LangChain 官方教程](https://python.langchain.com/docs/tutorials/rag/)
- [LlamaIndex 官方教程](https://docs.llamaindex.ai/en/stable/)
- [Embedding 基础 - OpenAI Cookbook](https://cookbook.openai.com/examples/vector_databases/readme)
- [Chroma 官方文档](https://docs.trychroma.com/)
- [Milvus 官方文档](https://milvus.io/docs)
- [Qdrant 官方文档](https://qdrant.tech/documentation/)
- [Pinecone 学习中心](https://www.pinecone.io/learn/)

### 4.2 RAG 高级技术

| 主题 | 要点 |
|------|------|
| 检索优化 | 混合检索、重排序（Reranking）、知识图谱 |
| 查询优化 | 语义改写、多路召回、Query2Doc、Doc2Query |
| 索引扩展 | Small-to-Big、离散/连续索引扩展 |
| RAG 质量提升 | 数据准备→知识检索→答案生成三阶段方法 |
| RAG 可观测性 | 关键指标、日志、分布式追踪 |
| Agentic RAG | 基于 Agent 的自主检索增强 |
| Graph RAG | 微软 Graph RAG、Neo4j、知识图谱增强 |

### 免费学习资源

- [Advanced RAG Techniques（LangChain 博客）](https://blog.langchain.dev/deconstructing-rag/)
- [RAGFlow 官方文档（企业知识库）](https://ragflow.io/docs/dev/)
- [RAGFlow GitHub](https://github.com/infiniflow/ragflow)
- [Graph RAG 微软开源](https://github.com/microsoft/graphrag)
- [Neo4j Graph RAG 教程](https://neo4j.com/developer/graph-data-science/)
- [Ragas - RAG 评估框架](https://docs.ragas.io/)
- [Jerry Liu - Building Agentic RAG（YouTube）](https://www.youtube.com/watch?v=aQ4yGVKOX4I)
- [混合检索策略详解 - Weaviate Blog](https://weaviate.io/blog/hybrid-search-explained)

### 4.3 框架实践

| 框架 | 用途 |
|------|------|
| LangChain | 链式调用、Agent 工具集成 |
| LlamaIndex | 高效语料索引、文档处理 |
| RAGFlow | 企业级知识库搭建 |

### 免费学习资源

- [LangChain 官方文档](https://python.langchain.com/docs/introduction/)
- [LangChain 中文教程（GitHub）](https://github.com/liaokongVFX/LangChain-Chinese-Getting-Started-Guide)
- [LlamaIndex 官方文档](https://docs.llamaindex.ai/en/stable/)
- [LangChain + LlamaIndex 联合使用教程](https://docs.llamaindex.ai/en/stable/community/integrations/using_with_langchain/)

---

## 阶段五：Agent 智能体开发（约 4 周）⭐ 核心阶段

> 目标：掌握 Agent 核心原理、架构设计、多种框架开发能力。

### 5.1 Agent 核心概念与原理

| 主题 | 要点 |
|------|------|
| 智能体基本组成 | LLM + 工具 + 记忆 + 规划 |
| 三种落地路径 | Workflow、Agent、Multi-Agent |
| 执行流程 | 感知→规划→执行→反馈循环 |
| 通信协议 | MCP 协议、A2A 协议、ANP 协议 |
| 三大经典范式 | ReAct、Plan-and-Solve、Reflection |

### 免费学习资源

- [Anthropic - Building Effective Agents](https://www.anthropic.com/engineering/building-effective-agents)
- [OpenAI Agent 开发指南](https://platform.openai.com/docs/guides/agents)
- [Google - Agent 白皮书](https://arxiv.org/abs/2401.03568)
- [LLM Powered Autonomous Agents（Lilian Weng 博客）](https://lilianweng.github.io/posts/2023-06-23-agent/)
- [ReAct 论文](https://arxiv.org/abs/2210.03629)
- [Plan-and-Solve 论文](https://arxiv.org/abs/2305.04091)
- [Reflexion 论文](https://arxiv.org/abs/2303.11366)
- [Andrew Ng - AI Agentic Workflows（DeepLearning.AI）](https://www.deeplearning.ai/short-courses/ai-agentic-design-patterns-with-autogen/)

### 5.2 Agent 架构与上下文工程

| 主题 | 要点 |
|------|------|
| Agent 架构分层 | 感知层→推理层→执行层→记忆层 |
| 结构化提示词工程 | System Prompt 设计、指令层级 |
| 上下文工程 | Context Engineering、RAG 管道集成 |
| 语义化工具系统 | 工具描述、MCP 协议集成 |
| 规划与协作 | 任务分解、多 Agent 协作模式 |

### 免费学习资源

- [Context Engineering 指南 - LangChain](https://blog.langchain.dev/context-engineering/)
- [Anthropic Tool Use 文档](https://docs.anthropic.com/en/docs/build-with-claude/tool-use/overview)
- [OpenAI Function Calling 文档](https://platform.openai.com/docs/guides/function-calling)
- [Agent 设计模式 - Microsoft AutoGen 文档](https://microsoft.github.io/autogen/)

### 5.3 多智能体协同

| 主题 | 要点 |
|------|------|
| 角色分工模型 | 主控 Agent、执行 Agent、审查 Agent |
| 共识机制 | 仲裁策略、任务合并、冲突解决 |
| 跨 Agent 追踪 | Trace 跟踪模式 |
| 资源管控 | 限额控制、防滥用 |

### 免费学习资源

- [CrewAI 官方文档](https://docs.crewai.com/)
- [AutoGen 官方文档](https://microsoft.github.io/autogen/)
- [LangGraph Multi-Agent 教程](https://langchain-ai.github.io/langgraph/tutorials/multi_agent/multi-agent-collaboration/)
- [MetaGPT 多智能体框架](https://github.com/geekan/MetaGPT)

### 5.4 低代码智能体平台

| 平台 | 特点 |
|------|------|
| Coze（扣子） | 字节跳动、零代码搭建 |
| Dify | 开源 LLMOps 平台 |
| n8n | 开源自动化工作流 |

### 免费学习资源

- [Coze 官方文档](https://www.coze.cn/docs)
- [Dify 官方文档](https://docs.dify.ai/zh-hans)
- [Dify GitHub](https://github.com/langgenius/dify)
- [n8n 官方文档](https://docs.n8n.io/)
- [n8n AI Agent 教程](https://docs.n8n.io/advanced-ai/)

### 5.5 Agent 开发框架实战

| 框架 | 要点 |
|------|------|
| **LangChain** | Create Agent、Models、Tools、MCP 集成、Memory、Streaming |
| **LangGraph** | 状态图、Nodes & Edges、Checkpointers、Human-in-the-Loop |
| **Agno** | 轻量级 Agent 框架 |
| **CrewAI** | 多角色协作框架 |
| **Smolagents** | HuggingFace 极简 Agent |
| **AutoGen** | 微软多 Agent 对话框架 |
| **AgentScope** | 阿里多 Agent 平台 |

### 免费学习资源

- [LangChain 官方文档](https://python.langchain.com/docs/introduction/)
- [LangGraph 官方文档 & 教程](https://langchain-ai.github.io/langgraph/)
- [LangGraph Academy（免费课程）](https://academy.langchain.com/)
- [Agno 官方文档](https://docs.agno.com/)
- [CrewAI 官方文档](https://docs.crewai.com/)
- [Smolagents（HuggingFace）](https://huggingface.co/docs/smolagents)
- [AutoGen 官方文档](https://microsoft.github.io/autogen/)
- [AgentScope GitHub](https://github.com/modelscope/agentscope)
- [DeepLearning.AI - Functions, Tools and Agents with LangChain（免费短课）](https://www.deeplearning.ai/short-courses/functions-tools-agents-langchain/)
- [DeepLearning.AI - LangGraph（免费短课）](https://www.deeplearning.ai/short-courses/ai-agents-in-langgraph/)

### 5.6 Deep Agents & Agent Skills

| 主题 | 要点 |
|------|------|
| Deep Agent | 计划工具、Todo List、文件系统、子代理 |
| Agent Skills | MCP 之后的能力扩展、Skills 创建与使用 |
| Agent Harness | 六大核心组件、三种 Harness 设计范式 |
| Agent 工程化 | 三层复杂度、成长五阶段模型、设计模式 |

### 免费学习资源

- [Anthropic Claude Code Skills 文档](https://docs.anthropic.com/en/docs/claude-code)
- [Agent Engineering - Chip Huyen 博客](https://huyenchip.com/2025/01/07/agents.html)
- [Building Production-Ready AI Agents（LangChain 博客）](https://blog.langchain.dev/)

---

## 阶段六：MCP 开发 & 工程化（约 2 周）

> 目标：掌握 MCP 协议开发、系统可观测性、氛围编程工具。

### 6.1 MCP 开发

| 主题 | 要点 |
|------|------|
| MCP 架构 | JSON-RPC 2.0、传输协议（STDIO/SSE/Streamable HTTP） |
| 客户端/服务端交互 | 交互流程、SDK 开发 |
| FastMCP V2 | 框架开发实战 |
| MCP Sampling | 流程步骤、最佳实践 |
| LangChain 集成 MCP | 集成高德地图等 MCP Server |

### 免费学习资源

- [MCP 官方规范文档](https://modelcontextprotocol.io/)
- [MCP GitHub（Anthropic）](https://github.com/modelcontextprotocol)
- [FastMCP 官方文档](https://gofastmcp.com/)
- [MCP Python SDK](https://github.com/modelcontextprotocol/python-sdk)
- [MCP TypeScript SDK](https://github.com/modelcontextprotocol/typescript-sdk)
- [Awesome MCP Servers（社区合集）](https://github.com/punkpeye/awesome-mcp-servers)

### 6.2 AI 系统观测与评估

| 工具 | 要点 |
|------|------|
| LangSmith | Tracing、Datasets、Evaluators、Experiments、Playground |
| LangFuse | 开源可观测平台、Prompt 管理、评估 |
| DeepEval | LLM 评估框架 |

### 免费学习资源

- [LangSmith 官方文档](https://docs.smith.langchain.com/)
- [LangFuse 官方文档](https://langfuse.com/docs)
- [LangFuse GitHub](https://github.com/langfuse/langfuse)
- [DeepEval 官方文档](https://docs.confident-ai.com/)
- [DeepEval GitHub](https://github.com/confident-ai/deepeval)

### 6.3 氛围编程（Vibe Coding）

| 工具 | 说明 |
|------|------|
| Claude Code | Anthropic CLI 编程助手 |
| OpenCode | 开源终端 AI 编码工具 |

### 免费学习资源

- [Claude Code 官方文档](https://docs.anthropic.com/en/docs/claude-code)
- [OpenCode GitHub](https://github.com/opencode-ai/opencode)
- [Cursor IDE 文档](https://docs.cursor.com/)

---

## 阶段七：项目实战 & 进阶（持续）

> 目标：通过实战项目巩固所学，达到生产级 Agent 开发能力。

### 推荐实战项目路径

| 序号 | 项目 | 涉及技术 | 难度 |
|------|------|----------|------|
| 1 | 从零构建生产级 RAG 系统 | 数据清洗、向量化、LangGraph Pipeline、Ragas 评估 | ⭐⭐⭐ |
| 2 | 基于 LangGraph 构建智能分诊系统 | 状态图对话流程、工具调用、动态路由、查询改写 | ⭐⭐⭐ |
| 3 | 从零构建生产级 AI Agent 服务 | FastAPI + LangGraph ReAct Agent + PostgreSQL + Redis + HITL + MCP | ⭐⭐⭐⭐ |
| 4 | 企业智能招标采购系统 | RAG + 微调 + LlamaIndex + Chroma + LLaMA Factory | ⭐⭐⭐⭐ |
| 5 | 基于 RAG 的法律咨询智能助手 | 模型微调 + RAG + 对比学习 + 多轮对话 | ⭐⭐⭐⭐ |
| 6 | OpenClaw 实战 | 全栈 Agent 系统、工具系统、多智能体协作 | ⭐⭐⭐⭐⭐ |

### 免费学习资源 & 开源项目参考

- [LangChain Templates（项目模板）](https://github.com/langchain-ai/langchain/tree/master/templates)
- [LangGraph Examples](https://github.com/langchain-ai/langgraph/tree/main/examples)
- [Full Stack RAG - LlamaIndex](https://github.com/run-llama/rags)
- [FastAPI 官方文档](https://fastapi.tiangolo.com/zh/)
- [Open Compass 评估平台](https://opencompass.org.cn/)
- [LLaMA Factory（微调工具）](https://github.com/hiyouga/LLaMA-Factory)

---

## 附录：微调知识（选修/按需学习）

> Agent 工程师不强制要求，但了解微调有助于理解模型能力边界。

| 主题 | 要点 |
|------|------|
| PEFT 高效微调 | LoRA、QLoRA、Prefix Tuning、P-Tuning V2 |
| 训练框架 | Unsloth、LLaMA Factory |
| 低精度训练 | FP16、8bit、4bit 量化 |
| 模型部署 | vLLM、SGLang、LMDeploy |

### 免费学习资源

- [Hugging Face PEFT 库](https://huggingface.co/docs/peft)
- [Unsloth（高效微调框架）](https://github.com/unslothai/unsloth)
- [LLaMA Factory GitHub](https://github.com/hiyouga/LLaMA-Factory)
- [DeepLearning.AI - Finetuning Large Language Models（免费短课）](https://www.deeplearning.ai/short-courses/finetuning-large-language-models/)
- [QLoRA 论文](https://arxiv.org/abs/2305.14314)

---

## 附录：面试准备

| 方向 | 高频面试主题 |
|------|-------------|
| LLM | Transformer 原理、Attention 机制、KV Cache、Tokenization |
| Agent | ReAct 流程、工具调用机制、记忆系统、多 Agent 协作 |
| RAG | 向量检索原理、Chunking 策略、Reranking、Graph RAG |
| 微调 | LoRA 原理、RLHF 流程、数据集构建 |
| 工程化 | MCP 协议、系统可观测性、Agent 评估方法 |

### 免费学习资源

- [大模型面试题汇总（GitHub）](https://github.com/wdndev/llm_interview_note)
- [LLM 面试八股文（GitHub）](https://github.com/km1994/LLMs_interview_notes)
- [AI 求职指南 - 台大李宏毅](https://www.youtube.com/watch?v=0R2A2CM2P7s)

---

## 推荐学习顺序 & 每日安排建议

| 时间 | 学习内容 |
|------|---------|
| **第 1-2 周** | Python 基础（有基础可跳过） |
| **第 3-5 周** | LLM 基础理论 + Transformer + 大模型生态 |
| **第 6-7 周** | Prompt Engineering 全技术栈 |
| **第 8-10 周** | RAG 从入门到高级（Agentic RAG + Graph RAG） |
| **第 11-14 周** | Agent 核心开发（LangChain + LangGraph + 多 Agent） |
| **第 15-16 周** | MCP 开发 + 工程化 + 可观测性 |
| **第 17 周起** | 项目实战（边做边学，持续迭代） |

> 💡 建议每天 2-3 小时，约 4 个月可完成主线学习路径。周末可加大实战练习时间。

---

## 持续跟进的社区 & 资讯

- [Hugging Face Blog](https://huggingface.co/blog)
- [LangChain Blog](https://blog.langchain.dev/)
- [Anthropic Research](https://www.anthropic.com/research)
- [OpenAI Blog](https://openai.com/blog)
- [arXiv AI 板块](https://arxiv.org/list/cs.AI/recent)
- [GitHub Trending - AI](https://github.com/trending?since=weekly)
- [AI 工具集导航](https://ai-bot.cn/)

---

*最后更新：2026 年 4 月 14 日*
