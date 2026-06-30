# 面试总览

更新日期：2026-06-30

这份文档作为当前唯一入口。日常先看这里；排期看 [interview-plan.md](interview-plan.md)，打电话和记录进展时再打开 [contact-tracking.md](contact-tracking.md)。

补充：2026-06-24 已有三批新增简历并入当前筛选口径。前两批中李昊泽、方浩、廖月华、王悦、朱坤、冯慧、李家璇、刘锐、李鑫、周升、刘少波、陈学志、赵景博、管瑞阳、胡景晟进入新增补位 / 强初筛；最新一批中曲仁宏、王俊豪、李正筱、王政浩、马克福、邵煜、陈康、徐耀鹏进入强初筛 / 技术一面补位，胡平、马志宇留作低优先初筛，杜浩东、刘盼盼、甄锐暂缓。`HS6...docx` 是问卷，不纳入候选人池。2026-06-30 新增 `实习简历.pdf`（罗政淮），已归入暂缓。排序原则：同档位先女生，其次北京就读候选，再看岗位匹配和到岗条件。

本周结果：2026-06-22 至 2026-06-26 已面试候选人全部未通过。已记录不推进：黄浩男、胡选杰、刘衡、舒泽林、廖月华；李烨保持“确定不来”。下周从未面试 / 未联系的强匹配候选继续推进。

## 1. 面试要求

### 岗位方向

当前岗位重点不是单纯 RAG，而是以下几个方向的组合：

- 浏览器自动运营 Agent：Playwright / Selenium、网页抓取、表单操作、内容生成、自动发布、账号态、Cookie、验证码、反爬、限流、失败重试、人工接管、风控边界。
- 通用 Agent 平台：类 Claw / WorkBuddy / 龙虾平台，重点看 Runtime、Harness、工具注册、上下文工程、checkpoint/resume、权限审批、审计日志、trace、benchmark。
- 工作流平台：Coze / Dify / LangGraph，重点看节点编排、插件/工具接入、状态流、失败重试、兜底、人工确认、流程调试。
- RAG：文档解析、切分、向量化、召回、重排、上下文组装、评测、可观测、幻觉排查。

### 新增验证口径：Agent 思考 / 决策 / 反馈

这是追加在原岗位方向之上的验证维度，不是替代原计划。

- 思考：任务拆解、Plan/ReAct/Plan-Execute、上下文构造、状态维护、长期任务怎么继续。
- 决策：意图路由、工具选择、Judge/Grader、重试/降级/停止条件、人工确认。
- 反馈：trace/eval、失败样例复盘、用户纠正进入记忆、benchmark/RAGAS/LLM-as-Judge 回归。

### 优先级

1. 原计划核心方向仍优先：浏览器自动运营 Agent / 通用 Agent 平台 / Claw 类 Runtime。
2. 在同等岗位匹配度下，上调能讲清 Agent 思考、决策、反馈闭环的人。
3. Coze / Dify / LangGraph 工作流平台作为第二梯队核心补充。
4. RAG 深度和工程化仍有价值，但需要有评测、trace、失败排查闭环。
5. LLM 部署、训练、蒸馏、RL 后训练作为加分项。

### 电话初筛必须确认

- 是否还在看实习机会。
- 最早到岗时间、每周可实习天数、可持续月数。
- 是否可以在技术面展开讲代码、GitHub、demo 或核心文件。
- 简历中的项目哪些是本人独立实现，哪些是团队已有或参考开源。
- 是否能讲清一个 Agent 项目的 plan / route / tool call / observe / evaluate / retry 链路。

### 技术面判断重点

- 不是只听关键词，要追问具体链路、失败场景、取舍和指标来源。
- 对浏览器自动化候选人，重点问登录态、Cookie、验证码、反爬、账号风控、人工接管。
- 对 Agent 平台候选人，重点问 Runtime 主循环、工具 schema、权限、checkpoint/resume、审计日志。
- 对 RAG 候选人，重点问 chunking、召回、重排、评测集、失败样例。
- 对工作流候选人，重点问状态图、节点输入输出、失败重试、兜底和人工确认。
- 对所有推进候选人，都要追问“思考、决策、反馈”：状态怎么流转、为什么调用这个工具、失败反馈如何进入下一轮。

## 2. 下周优先推进人员（2026-06-29 至 2026-07-03）

### P0：下周第一轮联系

| 顺序 | 候选人 | 电话 | 当前状态 | 匹配方向 | 为什么符合 |
| ---: | --- | --- | --- | --- | --- |
| 1 | 冯慧 | 15002602703 | 未联系 / 待确认 | AIOps Agent / LangGraph / MCP | 北邮本硕，Plan-Execute-Replan、MCP、RAG、SSE 和重试机制完整，同档位女生候选前置。 |
| 2 | 李家璇 | 15036583295 | 未联系 / 待确认 | Agentic Knowledge Hub / Dify 客服 Agent | RAG 多阶段检索、Agent 任务拆解和 Dify 工作流，适合强初筛。 |
| 3 | 朱坤 | 13862433994 | 未联系 / 待确认 | MCP 网关 / Multi-Agent / RAG | MCP Nexus 协议网关、Supervisor-Worker、TraceID / 指标链路完整。 |
| 4 | 赵绍猛 | 15713380988 | 未联系 / 待确认 | AIOps Agent Harness / 工具治理 | 自研 Harness、工具治理、上下文压缩、审计、失败重试、防无限 ReAct loop、长期记忆。 |
| 5 | 李昊泽 | 18391892833 | 未联系 / 待确认 | Coding Agent / Harness / Runtime | CodeRein 覆盖 Plan Mode、Checkpoint/Resume、执行域隔离、审计和 benchmark。 |
| 6 | 方浩 | 19121759781 | 未联系 / 待确认 | OnCall Agent / Coding Agent / MCP | 多 MCP、自进化记忆、上下文压缩、多 Agent 协作和安全审查。 |
| 7 | 王悦 | 13819100076 | 未联系 / 待确认 | 主动式 Agent / MCP / 记忆系统 | 6 阶段生命周期、5 阶段推送决策、五层记忆、MCP 并行拉取和后台任务框架。 |
| 8 | 李夏洋 | 15518794255 | 未联系 / 待确认 | Agent Runtime / 通用平台 | Mira Runtime 覆盖 Event Stream、State Machine、ReAct Loop、Tool/Skill、ContextBuilder/Compactor。 |
| 9 | 孙奇 | 18405675136 | 未联系 / 待确认 | OpenClaw / 工具平台 / 工作流 | OpenClaw Plugin SDK、40+ 工具、网页截图、HTML 渲染、长期记忆、安全边界。 |
| 10 | 王博涵 | 18991120513 | 未联系 / 待确认 | Agentic RAG / 评测闭环 | Routing、Grading、Self-Reflection、RAGAS、Prometheus、request_id 日志和法律 Agent 自动化评测。 |
| 11 | 周思行 | 13350756085 | 未联系 / 待确认 | 多 Agent 路由 / Monitor 闭环 | 三路意图识别、三级记忆、多 Agent 动态路由、Monitor 闭环、工具熔断降级、LLM-as-Judge。 |
| 12 | 曲仁宏 | 13303505823 | 未联系 / 待确认 | AI Agent / AI Infra | HChat + HRPC 体现分布式 RPC、网关、聊天与状态服务，基础设施味道强。 |

### P1：第二轮补位联系

| 顺序 | 候选人 | 电话 | 当前状态 | 适合方向 | 建议 |
| ---: | --- | --- | --- | --- | --- |
| 1 | 马克福 | 17690713967 | 未联系 / 待确认 | LangGraph / RAG / 训练 | 重点问闭环 Agent 的落地、训练与推理边界、评测和实际负责部分。 |
| 2 | 李正筱 | 18654558025 | 未联系 / 待确认 | Coding Agent / Harness / Runtime | 重点问 Orchestrator、工具调度、失败回滚、记忆和上下文压缩。 |
| 3 | 王政浩 | 15513950072 | 未联系 / 待确认 | Coding Agent / Context Compression | 重点问 context 压缩、沙箱隔离、读后写锁和断点续跑。 |
| 4 | 王俊豪 | 13586134636 | 未联系 / 待确认 | AgentHarness / Tool-use / HITL | 重点问主循环、人工确认、数据分析链路和指标来源。 |
| 5 | 陈康 | 13237333616 | 未联系 / 待确认 | ReAct / MCP / RAG / Memory | 重点问 Query Loop、Observation 回传、MCP 工具边界和评测闭环。 |
| 6 | 徐耀鹏 | 17302272003 | 未联系 / 待确认 | C++ MCP Server / Infra | 重点问 MCP 协议封装、双传输层、并发连接和 tool/resource/prompt 边界。 |
| 7 | 邵煜 | 18518653323 | 未联系 / 待确认 | 多 Agent RAG / checkpoint | 重点问状态维护、记忆与 checkpoint、评测集构建和失败样例回放。 |
| 8 | 刘锐 | 18214794197 | 未联系 / 待确认 | 多 Agent 审查 / Playwright / RPA | 重点问 Supervisor-Worker、Playwright/RPA 调用边界、ReAct 自纠错和人工审批接管。 |
| 9 | 李鑫 | 19862255726 | 未联系 / 待确认 | Agent Swarm / MCP / RAGAS | 重点问 Agent Loop、Swarm 路由、工具调用限制、记忆压缩和反思节点评测。 |
| 10 | 周升 | 13476527154 | 未联系 / 待确认 | Plan-Execute-Reflection 多 Agent / RAGAS | 重点问反思 Agent 校验、工具 API 超时降级、Memory 复用和 RAGAS 指标。 |

### 自动化运营最相关

说明：本节保留方向匹配分析；刘衡、舒泽林已在 2026-06-26 回填为“面试未通过 / 不推进”，不进入下周约面池。

| 候选人 | 判断 |
| --- | --- |
| 刘衡 | 最明确的自动化运营候选。简历写到小红书内容运营自动化、Playwright 抓取、内容生成和自动发布，应优先验证真实性。 |
| 王泽超 | 浏览器工具相关，Selenium 动态网页抓取、验证码/Cookie 处理，更偏抓取工具，不是完整运营闭环。 |
| 卢旭 | Selenium 反爬抓取 + 旅游 Agent，更偏浏览器抓取，不是运营发布。 |
| 舒泽林 | 桌面主动式 Agent，贴 WorkBuddy/桌面助手，不是明确内容运营发布。 |
| 孙奇 | OpenClaw 工具平台和网页截图能力强，但不是明确运营自动化闭环。 |

### 2026-06-23 新增补位

说明：本节保留新增批次分析；廖月华已在 2026-06-26 回填为“面试未通过 / 不推进”，不再作为补位联系对象。

| 候选人 | 简历文件 | 方向 | 为什么关注 | 面试重点 |
| --- | --- | --- | --- | --- |
| 李昊泽 | `李昊泽-AI Agent开发工程师.pdf` | Coding Agent / Harness / Runtime | CodeRein 覆盖 Plan Mode、Todo Ledger、Checkpoint/Resume、执行域隔离、审计和 benchmark，和当前 Agent 运行时口径很贴。 | 追问 Runtime 主循环、ToolExecutor 域隔离、workspace 漂移恢复和 224 个 pytest。 |
| 方浩 | `方浩_Agent 应用开发实习_中南大学硕士_简历.pdf` | OnCall Agent / Coding Agent / MCP | Oncall Agent + Minicode 同时覆盖多 MCP、自进化记忆、上下文压缩、多 Agent 协作和安全审查。 | 追问 Query Loop、自进化记忆闭环、多 Agent 权限边界和人工确认链路。 |
| 廖月华 | `agent开发简历-廖月华.pdf` | ChatBI 多 Agent / MCP / ReAct 重试 | 路由 Agent、查询 Agent、RAG 咨询 Agent、MCP Server 封装和自动重试闭环都比较完整。 | 追问结构化路由输出、MCP Server 接入、SQL 自动修正和评测集构成。 |
| 王悦 | `王悦_agent_1.pdf` | 主动式 Agent / MCP / 记忆系统 | 6 阶段生命周期、5 阶段推送决策、五层记忆、MCP 并行拉取和后台任务框架比较完整。 | 追问主动推送策略、去重机制、记忆审计任务和热点监控闭环。 |
| 朱坤 | `简历_朱坤.pdf` | MCP 网关 / Multi-Agent / RAG | MCP Nexus 协议网关 + Web3 Multi-Agent，覆盖多协议工具包装、限流熔断、TraceID、Supervisor-Worker 和 RAG 双通道。 | 追问 MCP 网关抽象层、熔断与校验、状态一致性和观测链路。 |
| 安晨阳 | `安晨阳 13721337093 Agent应用开发.pdf` | 多 Agent 深度研究 / GraphRAG | 云问 Agent 实习 + DeepFlow 多 Agent 研究平台，LangGraph/StateGraph、GraphRAG、RAGAS、Coze/Dify 都覆盖。 | 追问实习职责、主从 Agent 架构、路由与评测闭环是否真实。 |
| 赵柄州 | `agent实习简历-赵柄州.pdf` | 多 Agent 菜谱客服 / GraphRAG | Router + 多下游 Agent、GraphRAG/Text2Cypher/Text2SQL 和工作流设计都比较清楚。 | 追问 Router 准确率、条件边、GraphRAG 落地和真实代码。 |
| 雷君帆 | `Ageng应用开发.pdf` | 扫地机器人客服 / ReAct + 三层记忆 | 扫地机器人客服覆盖 ReAct、自主工具调用、三层记忆、混合检索和 RAG 全链路评测。 | 追问三层记忆、工具路由、TTL/importance 衰减和 RAGAS 指标来源。 |
| 王基宽 | `电子科技大学-王基宽.pdf` | 心理健康多 Agent / SSE / Docker | Supervisor 协作、双层记忆、Function Calling、SSE 和 Docker 都有，工程链路较完整。 | 追问 RiskGuardian 触发逻辑、长期档案更新和风险预警工具链。 |
| 刘亚津 | `吉林大学_刘亚津个人简历.pdf` | ReAct Agent + RAG | 本地知识库 ReAct Agent + RAG 项目较完整，但更偏单 Agent 应用。 | 追问 Evidence 引用、search_local_kb 工具、ReAct 决策和 LoRA 实操。 |
| 赵浩博 | `北京交通大学赵浩博.pdf` | RAG Agent + 动态 Prompt | 扫地机器人 RAG Agent 覆盖工具调用日志、动态 Prompt 切换和场景切换。 | 追问工具调用日志、中间件动态 Prompt 和报告生成链路。 |
| 韦沐池 | `韦沐池个人简历.pdf` | AIOps 调研 / 故障诊断 RAG | AIOps 调研和日志故障诊断 RAG，偏运维 / RAG 方向，有 LoRA 实操。 | 追问日志解析、诊断生成链路、LoRA 细节和是否有 Agent 决策闭环。 |
| 苏伊童 | `附件简历-苏伊童-26年应届生.pdf` | 训练 / 后训练 | 训练 / 后训练能力较强，但 Agent / 工作流 / RAG 主线证据弱。 | 仅在需要训练加分项时补聊，不进当前主岗优先面试。 |

### 2026-06-23 追加批次强初筛

| 候选人 | 简历文件 | 方向 | 为什么关注 | 面试重点 |
| --- | --- | --- | --- | --- |
| 冯慧 | `冯慧_简历 (11).pdf` | AIOps Agent / LangGraph / MCP | 北邮本硕，智能运维知识库 Agent 平台覆盖 Plan-Execute-Replan、MCP、RAG、SSE 和重试机制。 | 追问 AIOps 状态机、MCP 工具封装、重试停止条件和个人代码范围。 |
| 李家璇 | `李家璇简历.pdf` | Agentic Knowledge Hub / Dify 客服 Agent | Agentic Knowledge Hub 与 AgentFlow 客服平台覆盖 RAG 多阶段检索、Agent 任务拆解和 Dify 工作流。 | 追问混合召回、Agent 任务拆解、Dify 与自研后端边界。 |
| 刘锐 | `agent简历.pdf` | 多 Agent 审查 / Playwright / RPA | 供应商资质联合审查覆盖 LangGraph 多 Agent、OCR/RAG/Text-to-SQL、Playwright 信用调查和 RPA 自动填报。 | 追问 Supervisor-Worker、Playwright/RPA 调用边界、ReAct 自纠错和人工审批接管。 |
| 李鑫 | `李鑫_19862255726.pdf` | Agent Swarm / MCP / RAGAS | 医疗问答 Skills-Agent 双层架构、ReAct、Swarm、双层记忆；教学系统覆盖 LangGraph、MCP、RAGAS、LangFuse。 | 追问 Agent Loop、Swarm 路由、工具调用限制、记忆压缩和反思节点评测。 |
| 周升 | `周升__大模型应用开发_2027届.pdf` | Plan-Execute-Reflection 多 Agent / RAGAS | 气象 SkyNexus 多 Agent 系统覆盖三层协作、ReAct、多轮反思、Memory 和标准化工具 API。 | 追问反思 Agent 校验、工具 API 超时降级、Memory 复用和 RAGAS 指标。 |
| 刘少波 | `刘少波-简历.pdf` | 农业多 Agent / KG + RAG / QLoRA | 智能果园辅助决策覆盖 StateGraph、条件边、checkpoint、IoT 数据注入、KG + RAG 和 QLoRA。 | 追问四类 Agent 路由、Checkpoint 恢复、IoT 数据如何影响决策和 Cypher 查询。 |
| 陈学志 | `简历_副本2.pdf` | Windows 操控 Agent / VLM / RAG | RAG + VLM + Win32 API / UI Automation 的 Windows 图形界面操控 Agent，适合自动化补位。 | 追问屏幕理解、UI 元素库、执行失败反馈和安全边界。 |
| 赵景博 | `赵景博-Java全栈开发工程师-27年应届生.pdf` | DAG Runtime / GraphRAG / Harness | AGI Assistant 覆盖 DAG Agent Workflow Runtime、三层记忆、GraphRAG、Harness 容错和 RAGAS benchmark。 | 追问 DAG runtime、拓扑调度、Tool Isolation、记忆去重演化和 benchmark。 |
| 管瑞阳 | `简历 (1).pdf` | DeepAgents / 企业 RAG / LangGraph | 企业 RAG 与 DeepAgents 深度搜索项目覆盖 LangGraph、RAGFlow、FastAPI、WebSocket 和 ContextVar 隔离。 | 追问 DeepAgents 链路、上下文隔离、异步任务推送和报告生成。 |
| 胡景晟 | `resume.pdf` | 轻量 Agent 编排 / Tool / Memory | 独立开发 AgentOrchestrator，写到 Planning -> Tool Use -> Memory -> Output、asyncio、Pydantic 校验和 SSE。 | 追问 GitHub 代码、自研边界、Memory 设计和工具错误拦截。 |

### 2026-06-24 追加批次强初筛

| 候选人 | 简历文件 | 方向 | 为什么关注 | 面试重点 |
| --- | --- | --- | --- | --- |
| 曲仁宏 | `曲.pdf` | AI Agent / AI Infra | HChat + HRPC 体现分布式 RPC、网关、聊天与状态服务，基础设施味道很强。 | 问服务拆分、RPC 注册发现、并发模型和个人负责范围。 |
| 李正筱 | `李正筱求职.pdf` | Coding Agent / Harness / Runtime | 本地代码 Agent Harness 覆盖 Redis TTL、checkpoint / resume、4 模型后端、7 工具。 | 问 Orchestrator、工具调度、失败回滚、记忆和上下文压缩。 |
| 王政浩 | `王政浩简历(2).pdf` | Coding Agent / Context Compression | minicodAI 从零构建 Agent 系统，覆盖 ReAct 循环、流式输出、双后端切换和子 Agent 沙箱。 | 问 context 压缩、沙箱隔离、读后写锁和断点续跑。 |
| 王俊豪 | `最终修改简历！！.pdf` | AgentHarness / Tool-use / HITL | 企业财务与流量数据分析 AgentHarness，强调 Tool-use、SSE、HITL 和闭环分析。 | 问主循环、人工确认、数据分析链路和指标来源。 |
| 陈康 | `陈康-Agent开发岗位.pdf` | ReAct / MCP / RAG / Memory | ReAct、Tool Calling、MCP、RAG、Memory、评测都覆盖，Agent 架构表达完整。 | 问 Query Loop、Observation 回传、MCP 工具边界和评测闭环。 |
| 徐耀鹏 | `C++开发 - 徐耀鹏 - 17302272003 - 中国地质大学（武汉）.pdf` | C++ MCP Server / Infra | C++17 MCP Server，做了 HTTP / stdio 双传输层、工具注册、资源、Prompt 和 Ollama 集成。 | 问 MCP 协议封装、双传输层、并发连接和 tool/resource/prompt 边界。 |
| 邵煜 | `邵煜.pdf` | 多 Agent RAG / checkpoint | 多 Agent RAG 研究链路、SQLite 记忆 / checkpoint、评测集和长期任务思路比较清楚。 | 问状态维护、记忆与 checkpoint、评测集构建和失败样例回放。 |
| 马克福 | `简历_副本4.pdf` | LangGraph / RAG / 训练 | BUPT 硕士，LangGraph / RAG / LoRA / DPO / GRPO 都有，偏模型与 Agent 结合方向。 | 问闭环 Agent 的落地、训练与推理边界、评测和实际负责部分。 |

### 2026-06-24 低优先初筛

| 候选人 | 简历文件 | 判断 | 建议动作 |
| --- | --- | --- | --- |
| 胡平 | `胡平-立刻到岗-可实习六个月.pdf` | JobCopilot 走的是 LLM workflow + 岗位筛选 + 个性化招呼语，更偏自动化投递和 prompt 工程。 | 30 分钟初筛，重点问岗位筛选规则、LLM-as-Judge、异步流程和反爬/节流处理。 |
| 马志宇 | `简历-马志宇.pdf` | 农业 RAG + 文档解析链路较完整，但核心还是检索和领域问答，不是当前主线最强匹配。 | 30 分钟初筛，重点问复杂表格清洗、Query Rewrite / HyDE、评测和幻觉治理。 |

### 已面试 / 已处理历史

`raw/` 中 `～～` 开头的简历视为已面试 / 已处理历史，不进入下周新增联系。

| 候选人 | 当前状态 | 备注 |
| --- | --- | --- |
| 杨润芝 | 已联系 / NG | 不再推进。 |
| 肖雨琴 | 已联系 / 2轮面试已通过 | 已通过二轮，等待后续决策。 |
| 宋琳琳 | 已联系 / 待确认 | 等待确认。 |
| 李明婷 | 已联系 / 待确认 | 等待确认。 |

## 3. 下周建议动作

1. 周一先打 P0 前 12 人；本周未通过候选不再重复约面。
2. 每通电话都确认到岗时间、每周天数、可持续月数、是否能讲代码/GitHub/demo。
3. 技术面统一追加“Agent 思考、决策、反馈”追问，不单独作为一个新岗位。
4. 如果 P0 里约不到 6 场，就从 P1 和新增补位里按顺序补：马克福、李正筱、王政浩、王俊豪、陈康、徐耀鹏、邵煜、刘锐、李鑫、周升、刘少波、陈翔宇、侯永欣。
5. 每通电话后立即回填 [contact-tracking.md](contact-tracking.md)。
6. 若有 3-5 人一面表现好，周五前安排设计实操或二面。

### 只需要看的文件

- 总览与决策：当前文件 [interview-overview.md](interview-overview.md)
- 下周排期：[interview-plan.md](interview-plan.md)
- 打电话清单：[today-contact-list.md](today-contact-list.md)
- 记录联系进展：[contact-tracking.md](contact-tracking.md)
- 技术面打印：[output/pdf/ai-agent-rag-interview-pack.pdf](../output/pdf/ai-agent-rag-interview-pack.pdf)

其他文件保留为详细资料，日常不用优先看。
