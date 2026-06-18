# 候选人筛选结果

## 筛选标准

核心要求：

- 浏览器自动运营 Agent：是否做过 Playwright/Selenium/网页抓取/自动发布/表单操作/账号态维护，是否理解反爬、验证码、Cookie、限流、失败重试、人工接管和风控边界。
- RAG：是否做过文档入库、切分、向量化、召回、重排、评测、可观测等完整链路。
- 通用 Agent 平台：是否理解 Claw/WorkBuddy/龙虾类平台形态，是否做过 Runtime、Harness、工具注册、上下文工程、checkpoint/resume、权限审批、审计日志和评测闭环。
- 工作流平台：是否理解 Coze、Dify、LangGraph、状态机、任务编排、节点失败重试、checkpoint、插件/工具接入和流程调试。
- Agent：是否有工具调用、ReAct、多 Agent、MCP、记忆、上下文管理、权限边界等实践。

加分项：

- 了解 LLM 部署：Docker、vLLM、模型服务、GPU/CUDA 环境、线上稳定性。
- 了解训练：SFT、LoRA/QLoRA、数据构建、评测。
- 了解蒸馏：模型蒸馏、Distill 模型、知识蒸馏。
- 了解 RL 后训练：PPO、DPO、GRPO、RLHF、安全对齐。

判断原则：

- 新岗位优先级：浏览器/运营自动化和通用 Agent 平台经验 > 复杂工作流平台经验 > RAG 深度；纯 RAG 候选人仍可作为方向补充。
- 优先看项目深度、难点、指标、设计取舍，而不是只看关键词。
- 简历中只出现“了解/熟悉”但没有项目支撑的，降级处理。
- 所有候选人都需要在面试中验证真实性，尤其是指标、GitHub、个人负责范围。

## 结论

- A 档：优先安排技术一面，核心要求匹配度高。
- B 档：可作为备选，建议先做 20-30 分钟电话初筛或简历追问。
- C 档：暂缓，当前岗位匹配度不足。

## 已面试历史（`～～` 前缀，保留参考）

| 候选人 | 简历文件 | 推荐理由 | 面试重点 |
| --- | --- | --- | --- |
| 杨润芝 | `～～AI-杨润芝.pdf` | 有 AI Agent 实习，做过金融客服 Agent 工作流、RAG 调优、工业 RAG + GraphRAG、自动化 Web 安全 Agent。加分项包含 QLoRA、vLLM、Docker。 | 追问 GraphRAG 实体关系设计、LangGraph 9 节点导入/6 节点查询工作流、模型微调评测方式。 |
| 肖雨琴 | `～～AI-肖雨琴.pdf` | 北京交通大学硕士，法律 RAG 项目较完整，包含 Milvus、PostgreSQL、Redis、RAGAS、混合检索、RRF、HyDE、可观测 trace。另有面试 Agent 项目。 | 追问法律 RAG 的分块策略、Auto-merging、RAGAS 指标可信度、面试 Agent 的有限状态机和语音链路。 |
| 宋琳琳 | `～～AI-宋琳琳.pdf` | AI Agent 项目覆盖私有知识库、长期记忆图谱、MCP、多工具编排、SSE、异步任务。到岗和 6 个月实习时长清晰。 | 重点问 Neo4j 记忆图谱四层溯源、工具白名单、异步任务失败恢复、长期记忆污染治理。 |
| 李明婷 | `～～AI-李明婷.pdf` | 北邮硕士，RAG 项目行业性较强，包含 32000+ 页专业文档、多模态抽取、BM25+向量+Rerank、LLM-as-judge。另有电磁信号检测 Agent。 | 追问专业文档 RAG 的数据清洗、图文联合问答、指标定义、检测 Agent 的事件溯源和工具失败自修复。 |

## A 档：当前优先面试（未面试待推进）

| 候选人 | 简历文件 | 推荐理由 | 面试重点 |
| --- | --- | --- | --- |
| 王新乐 | `王新乐 大模型应用开发 个人简历.pdf` | 多段大模型应用实习，覆盖 Dify Agent 工作流、RAG、多 Agent、AIOps、Docker、LoRA 微调和训练工程。项目指标较多，业务落地描述完整。 | 重点验证实习中个人实际负责范围、LoRA/Wan2.1 微调细节、AIOps LangGraph 状态机和 MCP 工具接入。 |
| 刘洋 | `刘洋-简历-AI开发实习生.pdf` | 东南大学硕士，Agentic 科研服务平台描述较深，覆盖 LangGraph、RAG Memory、HyDE、Reranker、LLMOps/AgentOps、Judge 重路由。另有金融分析 Agent 项目。 | 深挖三级记忆、AgentOps 链路追踪、Judge node 判定逻辑、工具调用 29-38 次时的稳定性设计。 |
| 李夏洋 | `简历.pdf` | Agent Runtime 和 Agentic RAG 描述完整，包含 Event Stream、State Machine、ReAct Loop、工具/技能调度、Corrective RAG、RAGAS 指标。 | 要求现场画 Agent Runtime 架构，解释状态迁移、上下文压缩、Corrective RAG 触发条件和评测集构建。 |
| 王泽超 | `王泽超_Agent简历.pdf` | 有医疗 AI 实习，独立做过模块化企业知识库 RAG 与评估平台，另有 LangGraph ReAct 旅游智能体。覆盖 RAG、MCP、Ragas、Docker、模型服务部署。 | 验证企业 RAG 平台的 ingestion pipeline、RRF/Rerank、Ragas 指标、医疗实习中的 Agent 接口开发深度。 |
| 王俊伟 | `西北农林科技大学-王俊伟.pdf` | 985/211 人工智能硕士，智能运维 Agent 场景贴近真实业务，覆盖 LangGraph 多 Agent 工作流、MCP 工具、RAG、Prometheus/Loki、Docker Compose。 | 深挖 incident 生命周期、Planner/Executor/Replanner、告警到排障建议的闭环、Docker 多服务拆分。 |
| 吴鹏伟 | `吴鹏伟-agent应用实习(1).pdf` | 覆盖 RAG、Agent、Tool Calling、LangGraph、Docker、Qwen2.5-7B 部署与 LoRA 微调。项目包括多智能体平台和税务金融 Agent 问答。 | 重点验证多 Agent 协作是否真实落地、长期记忆机制、Hybrid Search + Rerank 参数和 LoRA 训练细节。 |
| 孙奇 | `孙奇_AI_Agent开发实习6个月以上.pdf` | 明确 6 个月实习，Agent 落地意识强，项目包括 QQ Agentic 助手、工作流调度、长期记忆、40+ 工具、安全边界和代码工具链。 | 验证聊天场景中的工具权限、消息通道可靠性、工作流调度状态、长期记忆隔离和代码工具安全。 |

## 新岗位优先面试（2026-06-17）

新口径更强调浏览器自动运营 Agent、通用 Agent 平台、Coze/Claw 类平台能力。若今天只约 4 人，先约李烨、黄浩男、舒泽林、刘衡；若约 6 人，再加李夏洋、孙奇。

| 候选人 | 简历文件 | 匹配方向 | 推荐理由 | 面试重点 |
| --- | --- | --- | --- | --- |
| 李烨 | `李烨-简历.pdf` | Claw/通用 Agent 平台 + RAG | ClawAgent 本地优先多智能体工作台非常贴近通用平台方向，覆盖会话级消息队列、busy/follow-up 排队、任务取消、工具权限审批、审计日志、SSE 和 Web 检索；另有 SmartRecruit RAG 推荐系统。 | 深挖 Agent 执行链路、会话并发控制、任务取消、工具权限、审计日志字段、Web 检索工具边界和代码真实性。 |
| 黄浩男 | `黄浩男-Agent开发_AI应用开发 (2).pdf` | Agent Runtime / Harness / Claw 类平台 | Pure Coding Agent Harness 贴合 Claw 类平台，覆盖 AgentRuntime、ToolCalling、ContextManagement、Checkpoint/Resume、JSONL Trace、workspace 隔离、高风险审批和 benchmark。 | 强验证 GitHub：Runtime 主循环、工具解析、路径边界、只读模式、checkpoint 校验、benchmark 生成和测试覆盖。 |
| 舒泽林 | `舒泽林的简历 (1).pdf` | 桌面/浏览器自动化 Agent | AirJelly 是 Electron + TypeScript 桌面端主动式 Agent，利用屏幕截图、键盘状态、活跃窗口感知上下文，做主动触发、任务归属、记忆抽取和 Benchmark，贴近 WorkBuddy/桌面助手方向。 | 追问截图理解、Task 归属、debounce/cooldown、锁屏/活跃窗口上下文、Episodic/Semantic 记忆、Langfuse trace 和真实截图 benchmark。 |
| 刘衡 | `刘衡aiAgent开发简历.pdf` | 浏览器自动运营 Agent + OpenClaw | 小红书内容运营自动化 Workflow 明确使用 Playwright 做内容抓取、爆款规律分析、选题/标题/正文/标签生成和自动发布；还写到 Agent Runtime、OpenClaw Skills 和 Harness Engineering。 | 重点验证 Playwright 脚本、登录态/Cookie、反爬/验证码、自动发布边界、内容生成工作流、OpenClaw Skills 和时间线真实性。 |
| 李夏洋 | `简历.pdf` | Agent Runtime / 通用平台 | Mira Interview Agent 覆盖 Event Stream + State Machine + ReAct Loop、Tool/Skill 调度、ContextBuilder/Compactor、Memory Store、多模型路由和降级，适合通用 Agent 平台方向。 | 要求画 Runtime 架构，解释状态迁移、工具 schema 注入、技能按需加载、上下文压缩、会话恢复和可观测 trace。 |
| 孙奇 | `孙奇_AI_Agent开发实习6个月以上.pdf` | OpenClaw / 工具平台 / 工作流 | QQ Agentic 助手覆盖 OpenClaw Plugin SDK、40+ 工具、HTML 渲染、网页截图、文档读写/转换、工作流调度、长期记忆和安全边界。 | 追问 OpenClaw 插件开发、工具 schema、网页截图/HTML 渲染链路、QQ 消息通道可靠性、40+ 工具权限和长期记忆隔离。 |

## 方向补充候选（2026-06-17）

| 候选人 | 简历文件 | 适合方向 | 判断 | 建议动作 |
| --- | --- | --- | --- | --- |
| 刘心怡 | `刘心怡_武汉大学硕士_大模型应用开发616.pdf` | RAG + 多 Agent 工作流 | Agentic RAG 调研和 CareerPilot 多 Agent 很稳，适合作为 RAG/工作流方向强候选，但浏览器运营和 Claw 平台证据少。 | 保留技术面，重点考 LangGraph 反思补检、MCP Tool Manager 和评测闭环。 |
| 戴霖 | `应聘Agent应用开发实习生—27年应届生北科大戴霖简历.pdf` | AIOps Agent + RAG | OnCall AIOps Agent 工程化好，适合运维 Agent/RAG 方向，和浏览器运营方向不是最贴。 | 作为工程化强候选，问 MCP 监控/日志工具、Golden Set 和 Redis 锁。 |
| 王泽超 | `王泽超_Agent简历.pdf` | Selenium 浏览器工具 + RAG | 旅游智能体里使用 Selenium 做动态网页抓取、验证码/Cookie 处理，并接入高德 MCP，兼具 RAG 评估平台。 | 可上调为浏览器工具补充候选，重点问 Selenium、验证码、Cookie 复用和网页抓取稳定性。 |
| 卢旭 | `卢旭-Agent开发-简历.pdf` | Selenium + 旅游 Agent | 旅游 Agent 集成 Selenium 反爬抓取、高德地图 API、DuckDuckGo 搜索和 Checkpoint。 | 电话初筛即可，确认 Selenium 实现深度和是否有真实浏览器自动化代码。 |
| 黄仟秋 | `黄仟秋.pdf` | Agent 评测 + RAG 后端 | DataAgent-Bench 做 LangGraph Agent、工具边界、benchmark、trace/metrics；ShopGuide 做 RAG 导购 Agent，评测意识强。 | 新增备选，适合评测和 RAG 后端；问 benchmark、工具隔离、SSE 契约和失败兜底。 |
| 田宏越 | `简历1.pdf` | Agent Harness + 工作流平台 | 简历驱动 AI 面试官系统使用 Agent Harness、PLAN-EXECUTE-VERIFY、四层记忆、ContextAssembler 和 311 个 pytest。 | 新增备选，验证 Agent Harness 是否自研、测试覆盖和状态机边界。 |
| 刘逍龙 | `刘逍龙18940802759 agent应用开发工程师.pdf` | Coze 工作流 + 后端 Agent | 明确熟练掌握 Coze 工作流，后端工程经验较多；但平台深度需要核实。 | 初筛问 Coze 节点编排、插件接入、和自研 Agent 的差别。 |
| 高敬杰 | `高敬杰河北工程大学.pdf` | Go/Eino Agent 后端 | 智能运维 Agent 覆盖 Eino、Gemini Function Calling、MCP、Milvus/MySQL 分层记忆和多源告警证据融合，适合后端 Agent 补充。 | 初筛问 Eino 编排、MCP 工具边界、RAG 分片策略和 Go 后端个人职责。 |
| 邓靖俊 | `邓靖俊--AI应用实习--.pdf` | RAG + LangGraph Agent | 扫地机器人客服、网安论文 RAG + QLoRA、Personal Chef LangGraph 都有完整链路和 GitHub，但更偏 RAG/应用 Agent。 | 初筛问工具调用上限、动态 Prompt、QLoRA 数据构造、checkpoint 和 GitHub 代码。 |

## 原今日新增优先面试（旧口径，保留参考）

旧口径下，若只能约 4 人，先约刘心怡、戴霖、李烨、施佳俊；若约满 6 人，再加崔灿、黄浩男。

| 候选人 | 简历文件 | 推荐理由 | 面试重点 |
| --- | --- | --- | --- |
| 刘心怡 | `刘心怡_武汉大学硕士_大模型应用开发616.pdf` | 武汉大学硕士，CareerPilot 多 Agent 求职助手和 Agentic RAG 调研系统都贴合岗位，覆盖 LangGraph、FastAPI、Milvus、BM25、Rerank、SSE、Redis 记忆、Prometheus 和 Docker。 | 深挖多 Agent 路由、MCP Tool Manager、反思补检、资料入库元数据、评测集和指标提升是否真实。 |
| 戴霖 | `应聘Agent应用开发实习生—27年应届生北科大戴霖简历.pdf` | 北京科技大学硕士，明确每周 4 天、可 6 个月、一周内到岗。OnCall AIOps Agent 和 EdgeMind 项目覆盖 LangGraph Plan-Execute-Replan、RAG Golden Set、MCP 监控/日志工具、Redis 锁、pytest/CI。 | 重点问 Golden Set 构造、软拒答阈值、MCP 工具 schema、Redis 分布式锁、监控指标和真实到岗安排。 |
| 李烨 | `李烨-简历.pdf` | 电子科技大学硕士，ClawAgent 本地优先多智能体工作台和 SmartRecruit RAG 简历推荐系统都很贴合，覆盖 LangGraph、SSE、会话队列、权限审批、审计日志、SQLite FTS5/向量召回、Milvus 混合检索和离线评测。 | 要求讲清会话级队列、任务取消、工具权限、长期记忆索引、Hybrid Search + CrossEncoder、Recall/MRR/NDCG 评测集。 |
| 施佳俊 | `施佳俊-简历.pdf` | 燕山大学硕士，DeepResearch 多 Agent 和多模态 RAG 描述较完整，包含 6 Agent DAG、Reviewer 反馈路由、ResearchState、工具调用、Redis 状态缓存、SSE、OCR/PPT/视频字幕入库。 | 追问 6 Agent 状态图、Reviewer 如何决定补检/修订、ResearchState 字段、OCR 多模态入库、Recall@10/MRR 指标来源。 |
| 崔灿 | `崔灿Agent (8).pdf` | 河南大学硕士，有 GitHub AgentDesk，企业服务台 Agent 覆盖 Hub & Spoke、多轨道语义路由、HITL interrupt、FAISS RAG、119 个测试用例和 SSE。 | 现场要求打开/讲代码，验证 9 节点工作流、80 条路由评测集、interrupt 状态冻结、119 个测试的覆盖范围。 |
| 黄浩男 | `黄浩男-Agent开发_AI应用开发 (2).pdf` | 天津大学本科，Pure Coding Agent Harness 和 Charon Agentic RAG 诊断系统高度贴合，覆盖 Runtime 主循环、工具治理、上下文压缩、checkpoint/resume、JSONL trace、BM25+Dense+RRF 和 108 条 benchmark。 | 强验证真实性：GitHub 代码结构、workspace 隔离、危险操作拦截、checkpoint 校验、108 条日志 benchmark 和消融实验。 |

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
| 高敬杰 | `高敬杰河北工程大学.pdf` | Go/Eino 智能运维 Agent 覆盖 Gemini API 适配、Function Calling、MCP、Milvus/MySQL 分层记忆、多源告警证据融合；浏览器运营证据不足。 | 作为 Go/Agent 后端备选初筛，重点问 Eino 编排、MCP 工具、thought_signature 多轮透传、RAG 分片和真实代码。 |
| 高乐 | `个人简历(2)(3)(1)_20260604211843.pdf` | 项目覆盖 ReAct Agent、Subagent、MCP、RAG 混合检索、多智能体客服；背景跨度较大，需要核实。 | 初筛问项目代码、个人职责、为什么从原专业转 AI 应用。 |
| 熊友文 | `熊友文的简历.pdf` | 有扫地机器人客服 Agent、知识库语义搜索、MCP 工具封装，内容较实用但深度一般。 | 可作为备选，重点查 RAG 召回质量和 MCP 工具实现。 |
| 邓靖俊 | `邓靖俊--AI应用实习--.pdf` | RAG/Agent 项目完整，包含扫地机器人客服 ReAct Agent、网安论文 RAG + QLoRA、Personal Chef LangGraph；有评估集、日志和 checkpoint。浏览器/Claw 平台证据不强。 | RAG/Agent 备选初筛，重点问 5 次工具上限、动态 prompt、QLoRA 数据、SqliteSaver checkpoint 和 GitHub 真实性。 |
| 黄仁力 | `黄仁力工作简历.pdf` | Multi-Agent 编排、RAG/MCP、VibeCoding 贴合要求；本科阶段，项目指标需核实。 | 初筛确认项目代码和工程深度。 |
| 赵岩 | `赵岩 暑期实习(4).pdf` | 情感咨询 AI 助手覆盖 Agent + RAG + Redis 记忆 + 工程落地，但整体更偏应用 Demo。 | 可作为低优先级备选，问真实用户/数据和幻觉治理。 |
| 李真 | `附件简历-李真-Python-27年应届生.pdf` | RAG 和本地部署、训练数据处理较强，但工作流/Agent 深度不足。 | 如果需要 RAG/模型应用基础，可约初筛。 |
| 杜伟悦 | `杜伟悦-北京航空航天大学28届硕士.pdf` | LLM 训练、SFT、LoRA、GRPO、安全对齐很强；但不符合当前 RAG/工作流/Agent 主线。 | 作为训练/后训练加分方向候选，不作为主岗优先。 |
| 林振鑫 | `林振鑫简历.pdf` | DeepResearch Agent 覆盖 LangGraph、异步并发、RAG 优化，但项目数量和工程细节偏少。 | 暂作备选，适合轻量初筛。 |
| 舒泽林 | `舒泽林的简历 (1).pdf` | 西安电子科技大学，AirJelly 桌面端主动式 Agent 实习经历较实用，覆盖截图理解、任务归属、主动执行、情景/语义记忆、Benchmark 和 Langfuse 链路可视化。 | 作为今日第一替补，重点问主动触发策略、记忆合并、真实截图 benchmark、Prompt 迭代和个人负责代码。 |
| 朱松 | `朱松-简历.pdf` | GraphFlow 和 GraphRAG/RAG 项目覆盖 LangGraph、Neo4j、ChromaDB、LightRAG、HITL、Docker/K8s，技术栈很强，但指标和表述偏满，需要查真伪。 | 备选技术面，必须看 GitHub、让其画 GraphRAG 数据流、解释 LightRAG local/global/hybrid 和 K8s 实际部署。 |
| 彭浚烨 | `彭浚烨简历.pdf` | Plan-Execute Agent 与加权融合 RAG 项目覆盖层次化切分、BM25+向量、RRF、BGE Reranker、interrupt、Command(resume) 和长期记忆；另有同名 `彭浚烨简历.docx`，内容基本重复。 | 备选电话初筛，重点问父子节点存储、AutoMerging 父节点丢失、加权 RRF 参数和 LangGraph 并行 reducer。 |
| 刘耀阳 | `刘耀阳简历.pdf` | 北京工业大学，Agentic RAG 复习助手覆盖 MarkItDown、父子分块、pgvector HNSW、RRF、Cross-Encoder、LangGraph Map-Reduce、RAGBench/RAGAS；简历日期有乱码。 | 初筛先确认项目时间和可实习时间，再问 parent-child chunk、interrupt_before、RAGAS 指标和 Harness 项目真实性。 |
| 王紫航 | `个人简历.pdf` | AI 应用实习经历较贴近，覆盖文档解析、评审 Agent、扫地机器人客服 Hybrid RAG、动态 Web RAG 和 Deep Researcher 多 Agent。 | 备选初筛，重点查文档解析、业务评审 Agent 的真实使用场景、RRF/Rerank 评测和 Web RAG 证据链。 |
| 吴孔利 | `吴孔利-15870846204-ai大模型应用开发-东华理工大学-2027.6.pdf` | 企业知识库 RAG + Agent 和多 Agent 周报系统覆盖核心关键词，也有 GitHub/指标；本科背景，指标较多。 | 先电话核实项目代码和个人职责，重点问 RAG 评测、工具调用、工作流状态和指标计算。 |
| 廖晚迪 | `廖晚迪（同济本清华硕2027届）+个人简历.pdf` | 清华硕士、同济本科，学习能力强；做过 AI CR、智能问答知识库、短期/长期记忆、RAG 召回和城市设计 Agent Harness，但计算机工程深度需确认。 | 备选初筛，重点问 RAG 具体实现、记忆机制、AI CR 评测标准和非 CS 背景下的实际编码比例。 |
| 孟豪 | `孟豪的简历.pdf` | 北邮硕士，AutoResearch 和 Career Copilot 多 Agent 方向较贴合，综合背景不错。 | 初筛问项目代码、Agent 工作流节点、RAG 数据来源和实习时间。 |
| 周安康 | `周安康-北京邮电大学简历.pdf` | 北邮硕士，RAG 和 FaultRecap 多 Agent 覆盖部分核心要求。 | 作为备选，问故障复盘 Agent 的状态流、知识库评测和工具调用边界。 |
| 翟旭强 | `个人简历–翟旭强.pdf` | 西安交大拟入学，Agent/RAG 评测平台和评论 RAG 推荐 Agent 有一定深度；可 7 月 1 日到岗、至少 2 个月。 | 若短期补人可初筛，重点确认只能实习 2 个月是否满足岗位要求。 |
| 刘逍龙 | `刘逍龙18940802759 agent应用开发工程师.pdf` | 有 Agent 开发实习和后端工程经验，覆盖 RAG、LangGraph、MCP、Tool、Skill 和产品推荐/问答系统。 | 初筛验证“一年实习”真实性、产品推荐系统架构、RAG 幻觉抑制指标和个人负责范围。 |
| 侯晓光 | `山东大学侯晓光.pdf` | 山东大学硕士，Agent 学习助手和国家电网风险预警 Agent 有场景，另有 Qwen SFT/LoRA/QLoRA 实践。 | 备选初筛，重点问学科 NPC 配置化、Qdrant 知识库、学习报告/知识图谱和 Qwen 微调细节。 |
| 吕鹏 | `实习简历-吕鹏.pdf` | 北师大硕士，医疗 Agent 与 SFT/DPO 方向较强，加分项好，但岗位主线匹配度略低于今日优先。 | 可作为训练/后训练加分备选，问医疗 Agent 的工具边界、数据安全和 SFT/DPO 实操。 |
| 黄珍珍 | `哈尔滨工程大学-黄珍珍-简历.pdf` | 具备 HITL/OnCall Agent、LoRA/CV 等经历，整体贴近但项目细节弱于今日优先。 | 备选初筛，重点问 HITL 触发条件、OnCall 工具调用和模型训练细节。 |
| 赵杨 | `简历-AI应用.pdf` | GraphRAG 煤矿安全智能体和从零复现类 LLaMA 训练链路有加分项，但主岗工程落地证据一般。 | 适合作为训练/GraphRAG 备选，问 Neo4j 建图、父子块、SFT/DPO 训练配置。 |
| 牛锐搏 | `牛锐搏-.pdf` | 电商语音客服、多 Agent、MCP、RAG-Anything、SFT/DPO 都覆盖，但指标、术语和业务收益堆叠明显，需要强真实性验证。 | 只建议电话初筛，要求提供项目代码/截图/接口，追问 MCP Server、Graph Checkpointer、微调数据和线上 A/B 口径。 |
| 张飞扬 | `AI应用开发.pdf` | Multi-Agent 求职评估和 RAG 系统覆盖核心方向，但简历抽取文字异常、指标较高，可信度需核验。 | 低优先备选，先问项目是否可展示、指标如何计算、客服实习是否真实上线。 |
| 刘衡 | `刘衡aiAgent开发简历.pdf` | 有医疗和 workflow 相关经历，但教育/经历时间线需要确认，核心 Agent/RAG 深度不如今日优先。 | 初筛确认时间线和可实习时间，再决定是否进入技术面。 |
| 梁宇超 | `简历  梁宇超 - 实习.pdf` | 中南大学本科、兰州大学拟录取，PAPERAGENT 有 PDF 解析、RAG、Evidence、多 Agent 和可视化控制台，基础不错。 | 作为低优先备选，问 PaperState、Evidence Pack、RAG 评估和硕士入学后的实习周期。 |

## C 档：暂缓

| 候选人 | 简历文件 | 原因 |
| --- | --- | --- |
| 刘兴瑞 | `2_实习简历_AI.pdf` | 交通建模、多 Agent 仿真和强化学习较强，但不是 LLM Agent/RAG 应用方向。 |
| kyan | `kyan简历.pdf` | 机器学习/RAG 研究描述较少，缺少 Agent、工作流和工程落地证据。 |
| 张皓 | `北京工业大学-计算机科学与技术-张皓.pdf` | 主要是 AI 平台前端开发，和 RAG/Agent/工作流核心要求不匹配。 |
| 纪晓一 | `个人简历(1).pdf` | 主要是金融/业务系统和 AI Advisor，Agent/RAG/工作流证据不足。 |
| 林欣宇 | `个人简历_LXY.pdf` | 只有较简单的本地知识库 AI 助手，深度和工程复杂度不足。 |
| 蒋锦宏 | `蒋锦宏简历.pdf` | 年级较低，Agent 旅行规划项目偏入门，暂不作为今天面试对象。 |
| 魏正沙 | `求职简历1111.pdf` | 当前可抽取信息只有基础个人信息，缺少岗位相关项目和技能证据。 |

## 面试验证风险点

- 多份简历存在相似的 Coding Agent Harness 表述，需要查代码、提交记录和个人职责。
- 很多简历写了较高指标，需要问指标定义、数据集规模、baseline、评测脚本和失败样例。
- 对“熟悉 LangGraph/LangChain”的候选人，必须让其画出状态图、节点输入输出、失败重试和 checkpoint 机制。
- 对“RAG 优化”的候选人，必须追问 chunking、召回、重排、上下文组装、评测和线上排障，避免只会调用框架。
- 对“训练/微调/RL 后训练”的候选人，必须追问数据构建、训练配置、显存、loss 曲线、评测指标和安全边界。
