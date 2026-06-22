# 面试总览

更新日期：2026-06-21

这份文档作为当前唯一入口。日常先看这里；排期看 [interview-plan.md](interview-plan.md)，打电话和记录进展时再打开 [contact-tracking.md](contact-tracking.md)。

补充：2026-06-22 上午又新增 5 份简历，已初步并入当前筛选口径：李子昊、来淼鑫、雷剑进入新增强初筛池；薛景瑞进入低优先初筛；黄可心因 PDF 文本不可读，需人工打开确认。

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
4. 如果 P0 里约不到 6 场，就从 P1 按顺序补：陈翔宇、侯永欣、刘心怡、戴霖、王泽超、黄仟秋。
5. 每通电话后立即回填 [contact-tracking.md](contact-tracking.md)。
6. 若有 3-5 人一面表现好，周五前安排设计实操或二面。

### 只需要看的文件

- 总览与决策：当前文件 [interview-overview.md](interview-overview.md)
- 下周排期：[interview-plan.md](interview-plan.md)
- 打电话清单：[today-contact-list.md](today-contact-list.md)
- 记录联系进展：[contact-tracking.md](contact-tracking.md)
- 技术面打印：[output/pdf/ai-agent-rag-interview-pack.pdf](../output/pdf/ai-agent-rag-interview-pack.pdf)

其他文件保留为详细资料，日常不用优先看。
