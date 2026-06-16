# 候选人筛选结果

## 筛选标准

核心要求：

- RAG：是否做过文档入库、切分、向量化、召回、重排、评测、可观测等完整链路。
- 工作流：是否理解 LangGraph、Dify、状态机、任务编排、节点失败重试、checkpoint 等。
- Agent：是否有工具调用、ReAct、多 Agent、MCP、记忆、上下文管理、权限边界等实践。

加分项：

- 了解 LLM 部署：Docker、vLLM、模型服务、GPU/CUDA 环境、线上稳定性。
- 了解训练：SFT、LoRA/QLoRA、数据构建、评测。
- 了解蒸馏：模型蒸馏、Distill 模型、知识蒸馏。
- 了解 RL 后训练：PPO、DPO、GRPO、RLHF、安全对齐。

判断原则：

- 优先看项目深度、难点、指标、设计取舍，而不是只看关键词。
- 简历中只出现“了解/熟悉”但没有项目支撑的，降级处理。
- 所有候选人都需要在面试中验证真实性，尤其是指标、GitHub、个人负责范围。

## 结论

- A 档：优先安排技术一面，核心要求匹配度高。
- B 档：可作为备选，建议先做 20-30 分钟电话初筛或简历追问。
- C 档：暂缓，当前岗位匹配度不足。

## A 档：优先面试

| 候选人 | 简历文件 | 推荐理由 | 面试重点 |
| --- | --- | --- | --- |
| 杨润芝 | `杨润芝-ai agent应用工程师.pdf` | 有 AI Agent 实习，做过金融客服 Agent 工作流、RAG 调优、工业 RAG + GraphRAG、自动化 Web 安全 Agent。加分项包含 QLoRA、vLLM、Docker。 | 追问 GraphRAG 实体关系设计、LangGraph 9 节点导入/6 节点查询工作流、模型微调评测方式。 |
| 肖雨琴 | `28-Agent开发AI应用开发-肖雨琴.pdf` | 北京交通大学硕士，法律 RAG 项目较完整，包含 Milvus、PostgreSQL、Redis、RAGAS、混合检索、RRF、HyDE、可观测 trace。另有面试 Agent 项目。 | 追问法律 RAG 的分块策略、Auto-merging、RAGAS 指标可信度、面试 Agent 的有限状态机和语音链路。 |
| 宋琳琳 | `宋琳琳简历-AI agent.pdf` | AI Agent 项目覆盖私有知识库、长期记忆图谱、MCP、多工具编排、SSE、异步任务。到岗和 6 个月实习时长清晰。 | 重点问 Neo4j 记忆图谱四层溯源、工具白名单、异步任务失败恢复、长期记忆污染治理。 |
| 李明婷 | `李明婷大模型应用算法.pdf` | 北邮硕士，RAG 项目行业性较强，包含 32000+ 页专业文档、多模态抽取、BM25+向量+Rerank、LLM-as-judge。另有电磁信号检测 Agent。 | 追问专业文档 RAG 的数据清洗、图文联合问答、指标定义、检测 Agent 的事件溯源和工具失败自修复。 |
| 王新乐 | `王新乐 大模型应用开发 个人简历.pdf` | 多段大模型应用实习，覆盖 Dify Agent 工作流、RAG、多 Agent、AIOps、Docker、LoRA 微调和训练工程。项目指标较多，业务落地描述完整。 | 重点验证实习中个人实际负责范围、LoRA/Wan2.1 微调细节、AIOps LangGraph 状态机和 MCP 工具接入。 |
| 刘洋 | `刘洋-简历-AI开发实习生.pdf` | 东南大学硕士，Agentic 科研服务平台描述较深，覆盖 LangGraph、RAG Memory、HyDE、Reranker、LLMOps/AgentOps、Judge 重路由。另有金融分析 Agent 项目。 | 深挖三级记忆、AgentOps 链路追踪、Judge node 判定逻辑、工具调用 29-38 次时的稳定性设计。 |
| 李夏洋 | `简历.pdf` | Agent Runtime 和 Agentic RAG 描述完整，包含 Event Stream、State Machine、ReAct Loop、工具/技能调度、Corrective RAG、RAGAS 指标。 | 要求现场画 Agent Runtime 架构，解释状态迁移、上下文压缩、Corrective RAG 触发条件和评测集构建。 |
| 王泽超 | `王泽超_Agent简历.pdf` | 有医疗 AI 实习，独立做过模块化企业知识库 RAG 与评估平台，另有 LangGraph ReAct 旅游智能体。覆盖 RAG、MCP、Ragas、Docker、模型服务部署。 | 验证企业 RAG 平台的 ingestion pipeline、RRF/Rerank、Ragas 指标、医疗实习中的 Agent 接口开发深度。 |
| 王俊伟 | `西北农林科技大学-王俊伟.pdf` | 985/211 人工智能硕士，智能运维 Agent 场景贴近真实业务，覆盖 LangGraph 多 Agent 工作流、MCP 工具、RAG、Prometheus/Loki、Docker Compose。 | 深挖 incident 生命周期、Planner/Executor/Replanner、告警到排障建议的闭环、Docker 多服务拆分。 |
| 吴鹏伟 | `吴鹏伟-agent应用实习(1).pdf` | 覆盖 RAG、Agent、Tool Calling、LangGraph、Docker、Qwen2.5-7B 部署与 LoRA 微调。项目包括多智能体平台和税务金融 Agent 问答。 | 重点验证多 Agent 协作是否真实落地、长期记忆机制、Hybrid Search + Rerank 参数和 LoRA 训练细节。 |
| 孙奇 | `孙奇_AI_Agent开发实习6个月以上.pdf` | 明确 6 个月实习，Agent 落地意识强，项目包括 QQ Agentic 助手、工作流调度、长期记忆、40+ 工具、安全边界和代码工具链。 | 验证聊天场景中的工具权限、消息通道可靠性、工作流调度状态、长期记忆隔离和代码工具安全。 |

## B 档：备选或初筛确认

| 候选人 | 简历文件 | 判断 | 建议动作 |
| --- | --- | --- | --- |
| 边轩凯 | `边轩凯17773923713.pdf` | Java/LangChain4j 方向，Agent + RAG 项目描述完整，有难点和解决方案；本科在读，需确认深度。 | 20-30 分钟初筛，重点查 LangChain4j、Rerank 微调、低配部署调优。 |
| 徐泉鑫 | `徐泉鑫的简历.pdf` | Agent、MCP、Coding Agent 原型和 RLHF/DPO/LoRA 知识覆盖不错；当前教育时间显示 2026.09 开始硕士，需确认实习时间。 | 初筛确认可到岗时间，技术面问 Coding Agent 工具权限和上下文压缩。 |
| 卢旭 | `卢旭-Agent开发-简历.pdf` | UCAS 软件所硕士，RAG+Agent 电商客服和 LangGraph 旅游机器人覆盖核心要求，但项目相对常规。 | 初筛后可面，重点查独立实现程度和高级 RAG 细节。 |
| 管翔 | `管翔 个人简历.pdf` | Coding Agent Harness 描述很深，覆盖上下文、记忆、checkpoint、安全和评测；但项目需要重点验证真实性。 | 要求展示代码或现场讲 benchmark，避免只停留在概念描述。 |
| 贾永星 | `贾永星-硕士-后端、agent开发 (1).pdf` | 与管翔简历中的 Harness 项目高度相似，另有 AI 应用后端实习和 RAG 问答链路。 | 先查是否团队项目、个人职责和代码证据，再决定是否进入技术面。 |
| 王伟 | `Wang_Wei.pdf` | 本科在读，但 RAGent 项目覆盖 Agentic RAG、LangGraph、混合检索、可观测和大量测试；工程化意识强。 | 初筛验证项目真实性、1200+ 测试用例、RAG 指标来源。 |
| 肖华宇 | `Go实习开发简历.pdf` | Go 后端工程强，AI 面试引擎覆盖 RAG、SSE、MCP、pgvector、Docker。Agent 深度略弱于 A 档。 | 如果需要 Go/后端方向，可安排备选技术面。 |
| 高乐 | `个人简历(2)(3)(1)_20260604211843.pdf` | 项目覆盖 ReAct Agent、Subagent、MCP、RAG 混合检索、多智能体客服；背景跨度较大，需要核实。 | 初筛问项目代码、个人职责、为什么从原专业转 AI 应用。 |
| 熊友文 | `熊友文的简历.pdf` | 有扫地机器人客服 Agent、知识库语义搜索、MCP 工具封装，内容较实用但深度一般。 | 可作为备选，重点查 RAG 召回质量和 MCP 工具实现。 |
| 黄仁力 | `黄仁力工作简历.pdf` | Multi-Agent 编排、RAG/MCP、VibeCoding 贴合要求；本科阶段，项目指标需核实。 | 初筛确认项目代码和工程深度。 |
| 赵岩 | `赵岩 暑期实习(4).pdf` | 情感咨询 AI 助手覆盖 Agent + RAG + Redis 记忆 + 工程落地，但整体更偏应用 Demo。 | 可作为低优先级备选，问真实用户/数据和幻觉治理。 |
| 李真 | `附件简历-李真-Python-27年应届生.pdf` | RAG 和本地部署、训练数据处理较强，但工作流/Agent 深度不足。 | 如果需要 RAG/模型应用基础，可约初筛。 |
| 杜伟悦 | `杜伟悦-北京航空航天大学28届硕士.pdf` | LLM 训练、SFT、LoRA、GRPO、安全对齐很强；但不符合当前 RAG/工作流/Agent 主线。 | 作为训练/后训练加分方向候选，不作为主岗优先。 |
| 林振鑫 | `林振鑫简历.pdf` | DeepResearch Agent 覆盖 LangGraph、异步并发、RAG 优化，但项目数量和工程细节偏少。 | 暂作备选，适合轻量初筛。 |

## C 档：暂缓

| 候选人 | 简历文件 | 原因 |
| --- | --- | --- |
| 刘兴瑞 | `2_实习简历_AI.pdf` | 交通建模、多 Agent 仿真和强化学习较强，但不是 LLM Agent/RAG 应用方向。 |
| kyan | `kyan简历.pdf` | 机器学习/RAG 研究描述较少，缺少 Agent、工作流和工程落地证据。 |
| 张皓 | `北京工业大学-计算机科学与技术-张皓.pdf` | 主要是 AI 平台前端开发，和 RAG/Agent/工作流核心要求不匹配。 |

## 面试验证风险点

- 多份简历存在相似的 Coding Agent Harness 表述，需要查代码、提交记录和个人职责。
- 很多简历写了较高指标，需要问指标定义、数据集规模、baseline、评测脚本和失败样例。
- 对“熟悉 LangGraph/LangChain”的候选人，必须让其画出状态图、节点输入输出、失败重试和 checkpoint 机制。
- 对“RAG 优化”的候选人，必须追问 chunking、召回、重排、上下文组装、评测和线上排障，避免只会调用框架。
- 对“训练/微调/RL 后训练”的候选人，必须追问数据构建、训练配置、显存、loss 曲线、评测指标和安全边界。
