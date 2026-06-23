# 面试总览

更新日期：2026-06-23

这份文档作为当前唯一入口。日常先看这里；排期看 [interview-plan.md](interview-plan.md)，打电话和记录进展时再打开 [contact-tracking.md](contact-tracking.md)。

补充：2026-06-23 又新增一批文件。已初步并入当前筛选口径：李昊泽、方浩、廖月华、王悦、朱坤进入新增补位 / 强初筛；安晨阳、赵柄州、雷君帆、王基宽进入低优先初筛；`tai-jinxue (ai-agent).pdf`、`于彤-15595168711.pdf`、`ai简历.pdf`、`求职简历-Agent开发实习生.pdf` 仍需人工打开确认。

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

## 2. 下周优先推进人员

### P0：原计划核心 + 新增强匹配

| 顺序 | 候选人 | 电话 | 当前状态 | 匹配方向 | 为什么符合 |
| ---: | --- | --- | --- | --- | --- |
| 1 | 李烨 | 17335610901 | 未联系 / 待确认 | Claw / 通用 Agent 平台 + RAG | 原计划核心。ClawAgent 覆盖会话队列、任务取消、权限审批、审计日志、SSE、Web 检索。 |
| 2 | 黄浩男 | 13224672500 | 未联系 / 待确认 | Agent Runtime / Harness / Claw 类平台 | 原计划核心。Pure Coding Agent Harness 覆盖 Runtime、ToolCalling、ContextManagement、Checkpoint/Resume、JSONL Trace、workspace 隔离。 |
| 3 | 胡选杰 | 13276387009 | 未联系 / 待确认 | Coding Agent / MCP / 多 Agent | 新增强匹配。ReAct + Plan Mode、MCP、Skill、上下文压缩、权限拦截、自动记忆提取、多 Agent 协作。 |
| 4 | 刘衡 | 13708800655 | 未联系 / 待确认 | 浏览器自动运营 Agent + OpenClaw | 原计划核心。小红书内容运营自动化 Workflow，Playwright + 内容抓取 + 自动发布。 |
| 5 | 舒泽林 | 17508510706 | 未联系 / 待确认 | 桌面 / 浏览器自动化 Agent | 原计划核心。AirJelly 主动式桌面 Agent，截图、键盘状态、活跃窗口、主动触发、记忆和 benchmark。 |
| 6 | 赵绍猛 | 15713380988 | 未联系 / 待确认 | AIOps Agent Harness / 工具治理 | 新增强匹配。自研 Harness、工具治理、上下文压缩、审计、失败重试、防无限 ReAct loop、长期记忆。 |
| 7 | 李夏洋 | 15518794255 | 未联系 / 待确认 | Agent Runtime / 通用平台 | 原计划核心。Mira Runtime 覆盖 Event Stream、State Machine、ReAct Loop、Tool/Skill、ContextBuilder/Compactor。 |
| 8 | 孙奇 | 18405675136 | 未联系 / 待确认 | OpenClaw / 工具平台 / 工作流 | 原计划核心。OpenClaw Plugin SDK、40+ 工具、网页截图、HTML 渲染、长期记忆、安全边界。 |
| 9 | 王博涵 | 18991120513 | 未联系 / 待确认 | Agentic RAG / 评测闭环 | 新增强匹配。Routing、Grading、Self-Reflection、RAGAS、Prometheus、request_id 日志和法律 Agent 自动化评测。 |
| 10 | 周思行 | 13350756085 | 未联系 / 待确认 | 多 Agent 路由 / Monitor 闭环 | 新增强匹配。三路意图识别、三级记忆、多 Agent 动态路由、Monitor 闭环、工具熔断降级、LLM-as-Judge。 |

### P1：技术一面或强初筛

| 顺序 | 候选人 | 电话 | 当前状态 | 适合方向 | 建议 |
| ---: | --- | --- | --- | --- | --- |
| 1 | 陈翔宇 | 18253832648 | 未联系 / 待确认 | MedAgent / Self-RAG / MCP | 新增强候选，查完整前后端、MCP 和 RAGAS 评估是否真实。 |
| 2 | 侯永欣 | 18238052603 | 未联系 / 待确认 | 客服 Agent / trace eval | 新增强候选，查 JSON 命令、工具确认、trace/eval 数据模型。 |
| 3 | 李子昊 | 18302774840 | 未联系 / 待确认 | Multi-Agent PR Copilot / RAG-MCP | 新增 2026-06-22。更贴“思考/决策/反馈”，重点查 Orchestrator、DAG 规划、失败降级和双评估后端。 |
| 4 | 来淼鑫 | 18335933458 | 未联系 / 待确认 | 医疗多 Agent / LangGraph | 新增 2026-06-22。5-Agent Pipeline、条件路由和共享状态模型较完整。 |
| 5 | 雷剑 | 13203543481 | 未联系 / 待确认 | ReAct 出行 Agent / MCP + RAG | 新增 2026-06-22。FastMCP、stdio/SSE、LangGraph ReAct、多用户上下文隔离和 RAGAS 评估。 |
| 6 | 刘心怡 | 13852765692 | 未联系 / 待确认 | RAG + 多 Agent 工作流 | 原补位，重点考 LangGraph 反思补检、MCP Tool Manager 和评测闭环。 |
| 7 | 戴霖 | 18900727703 | 未联系 / 待确认 | AIOps Agent + RAG | 原补位，工程化强，问 Golden Set、软拒答阈值、MCP 工具和 Redis 锁。 |
| 8 | 王泽超 | 15158269252 | 未联系 / 待确认 | Selenium 浏览器工具 + RAG | 原补位，问 Selenium、验证码/Cookie 和企业 RAG 平台。 |
| 9 | 黄仟秋 | 15399760679 | 未联系 / 待确认 | Agent 评测 + RAG 后端 | 原补位，适合评测、trace、RAG 后端。 |
| 10 | 田宏越 | 15253882785 | 未联系 / 待确认 | Agent Harness + 工作流平台 | 原补位，验证 PLAN-EXECUTE-VERIFY 和 311 个 pytest。 |

### 自动化运营最相关

| 候选人 | 判断 |
| --- | --- |
| 刘衡 | 最明确的自动化运营候选。简历写到小红书内容运营自动化、Playwright 抓取、内容生成和自动发布，应优先验证真实性。 |
| 王泽超 | 浏览器工具相关，Selenium 动态网页抓取、验证码/Cookie 处理，更偏抓取工具，不是完整运营闭环。 |
| 卢旭 | Selenium 反爬抓取 + 旅游 Agent，更偏浏览器抓取，不是运营发布。 |
| 舒泽林 | 桌面主动式 Agent，贴 WorkBuddy/桌面助手，不是明确内容运营发布。 |
| 孙奇 | OpenClaw 工具平台和网页截图能力强，但不是明确运营自动化闭环。 |

### 2026-06-23 新增补位

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

### 已面试 / 已处理历史

`raw/` 中 `～～` 开头的简历视为已面试 / 已处理历史，不进入下周新增联系。

| 候选人 | 当前状态 | 备注 |
| --- | --- | --- |
| 杨润芝 | 已联系 / NG | 不再推进。 |
| 肖雨琴 | 已联系 / 2轮面试已通过 | 已通过二轮，等待后续决策。 |
| 宋琳琳 | 已联系 / 待确认 | 等待确认。 |
| 李明婷 | 已联系 / 待确认 | 等待确认。 |

## 3. 下周建议动作

1. 周一先打 P0 前 10 人；原计划第一优先 6 人不能丢，新增候选作为同池竞争。
2. 每通电话都确认到岗时间、每周天数、可持续月数、是否能讲代码/GitHub/demo。
3. 技术面统一追加“Agent 思考、决策、反馈”追问，不单独作为一个新岗位。
4. 如果 P0 里约不到 6 场，就从 P1 和“2026-06-23 新增补位”里按顺序补：李昊泽、方浩、廖月华、王悦、朱坤、陈翔宇、侯永欣、李子昊、来淼鑫、雷剑。
5. 每通电话后立即回填 [contact-tracking.md](contact-tracking.md)。
6. 若有 3-5 人一面表现好，周五前安排设计实操或二面。

### 只需要看的文件

- 总览与决策：当前文件 [interview-overview.md](interview-overview.md)
- 下周排期：[interview-plan.md](interview-plan.md)
- 打电话清单：[today-contact-list.md](today-contact-list.md)
- 记录联系进展：[contact-tracking.md](contact-tracking.md)
- 技术面打印：[output/pdf/ai-agent-rag-interview-pack.pdf](../output/pdf/ai-agent-rag-interview-pack.pdf)

其他文件保留为详细资料，日常不用优先看。
