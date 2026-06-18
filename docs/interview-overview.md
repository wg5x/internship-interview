# 面试总览

更新日期：2026-06-18

这份文档作为当前唯一入口。日常先看这里；打电话和记录进展时再打开 [contact-tracking.md](contact-tracking.md)。

## 1. 面试要求

### 岗位方向

当前岗位重点不是单纯 RAG，而是以下几个方向的组合：

- 浏览器自动运营 Agent：Playwright / Selenium、网页抓取、表单操作、内容生成、自动发布、账号态、Cookie、验证码、反爬、限流、失败重试、人工接管、风控边界。
- 通用 Agent 平台：类 Claw / WorkBuddy / 龙虾平台，重点看 Runtime、Harness、工具注册、上下文工程、checkpoint/resume、权限审批、审计日志、trace、benchmark。
- 工作流平台：Coze / Dify / LangGraph，重点看节点编排、插件/工具接入、状态流、失败重试、兜底、人工确认、流程调试。
- RAG：文档解析、切分、向量化、召回、重排、上下文组装、评测、可观测、幻觉排查。

### 优先级

1. 浏览器自动运营 Agent / 浏览器自动化闭环。
2. 通用 Agent 平台 / Claw 类 Runtime 和工具平台。
3. Coze / Dify / LangGraph 工作流平台。
4. RAG 深度和工程化。
5. LLM 部署、训练、蒸馏、RL 后训练作为加分项。

### 电话初筛必须确认

- 是否还在看实习机会。
- 最早到岗时间、每周可实习天数、可持续月数。
- 是否可以在技术面展开讲代码、GitHub、demo 或核心文件。
- 简历中的项目哪些是本人独立实现，哪些是团队已有或参考开源。

### 技术面判断重点

- 不是只听关键词，要追问具体链路、失败场景、取舍和指标来源。
- 对浏览器自动化候选人，重点问登录态、Cookie、验证码、反爬、账号风控、人工接管。
- 对 Agent 平台候选人，重点问 Runtime 主循环、工具 schema、权限、checkpoint/resume、审计日志。
- 对 RAG 候选人，重点问 chunking、召回、重排、评测集、失败样例。
- 对工作流候选人，重点问状态图、节点输入输出、失败重试、兜底和人工确认。

## 2. 符合人员

### 第一优先：今天优先联系 / 约技术一面

| 顺序 | 候选人 | 电话 | 当前状态 | 匹配方向 | 为什么符合 |
| ---: | --- | --- | --- | --- | --- |
| 1 | 李烨 | 17335610901 | 未联系 / 待确认 | Claw / 通用 Agent 平台 + RAG | ClawAgent 本地优先多智能体工作台，覆盖会话队列、任务取消、权限审批、审计日志、SSE、Web 检索。 |
| 2 | 黄浩男 | 13224672500 | 未联系 / 待确认 | Agent Runtime / Harness / Claw 类平台 | Pure Coding Agent Harness 覆盖 Runtime、ToolCalling、ContextManagement、Checkpoint/Resume、JSONL Trace、workspace 隔离。 |
| 3 | 舒泽林 | 17508510706 | 未联系 / 待确认 | 桌面 / 浏览器自动化 Agent | AirJelly 桌面端主动式 Agent，覆盖截图、键盘状态、活跃窗口、主动触发、记忆和 benchmark。 |
| 4 | 刘衡 | 13708800655 | 未联系 / 待确认 | 浏览器自动运营 Agent + OpenClaw | 小红书内容运营自动化 Workflow，明确写 Playwright、内容抓取、爆款分析、选题/标题/正文/标签生成、自动发布。 |
| 5 | 李夏洋 | 15518794255 | 未联系 / 待确认 | Agent Runtime / 通用平台 | Mira Agent Runtime 覆盖 Event Stream、State Machine、ReAct Loop、Tool/Skill、ContextBuilder/Compactor。 |
| 6 | 孙奇 | 18405675136 | 未联系 / 待确认 | OpenClaw / 工具平台 / 工作流 | OpenClaw Plugin SDK、40+ 工具、网页截图、HTML 渲染、工作流调度、长期记忆、安全边界。 |

### 自动化运营最相关

| 候选人 | 判断 |
| --- | --- |
| 刘衡 | 最明确的自动化运营候选。简历写到小红书内容运营自动化、Playwright 抓取、内容生成和自动发布，应优先验证真实性。 |
| 王泽超 | 浏览器工具相关，Selenium 动态网页抓取、验证码/Cookie 处理，更偏抓取工具，不是完整运营闭环。 |
| 卢旭 | Selenium 反爬抓取 + 旅游 Agent，更偏浏览器抓取，不是运营发布。 |
| 舒泽林 | 桌面主动式 Agent，贴 WorkBuddy/桌面助手，不是明确内容运营发布。 |
| 孙奇 | OpenClaw 工具平台和网页截图能力强，但不是明确运营自动化闭环。 |

### 补位候选

| 顺序 | 候选人 | 电话 | 当前状态 | 适合方向 | 建议 |
| ---: | --- | --- | --- | --- | --- |
| 1 | 刘心怡 | 13852765692 | 未联系 / 待确认 | RAG + 多 Agent 工作流 | RAG/工作流强补位。 |
| 2 | 戴霖 | 18900727703 | 未联系 / 待确认 | AIOps Agent + RAG | 工程化强，适合运维 Agent/RAG。 |
| 3 | 王泽超 | 15158269252 | 未联系 / 待确认 | Selenium 浏览器工具 + RAG | 浏览器工具补位。 |
| 4 | 黄仟秋 | 15399760679 | 未联系 / 待确认 | Agent 评测 + RAG 后端 | 适合评测、trace、RAG 后端。 |
| 5 | 田宏越 | 15253882785 | 未联系 / 待确认 | Agent Harness + 工作流平台 | 适合 Harness、测试、工作流。 |
| 6 | 刘逍龙 | 18940802759 | 未联系 / 待确认 | Coze 工作流 + 后端 Agent | 适合 Coze/后端初筛。 |
| 7 | 高敬杰 | 13483000182 | 未联系 / 待确认 | Go/Eino Agent 后端 | 适合 Go 后端 Agent 补位。 |
| 8 | 邓靖俊 | 13541043150 | 未联系 / 待确认 | RAG + LangGraph Agent | 适合 RAG/应用 Agent 补位。 |

### 已面试 / 已处理历史

`raw/` 中 `～～` 开头的简历视为已面试 / 已处理历史，不进入今天新增联系。

| 候选人 | 当前状态 | 备注 |
| --- | --- | --- |
| 杨润芝 | 已联系 / NG | 不再推进。 |
| 肖雨琴 | 已联系 / 2轮面试已通过 | 已通过二轮，等待后续决策。 |
| 宋琳琳 | 已联系 / 待确认 | 等待确认。 |
| 李明婷 | 已联系 / 待确认 | 等待确认。 |

### 旧 A 档待联系 / 补位

| 候选人 | 电话 | 当前状态 | 备注 |
| --- | --- | --- | --- |
| 王新乐 | 18092238606 | 未联系 / 待确认 | Dify、RAG、多 Agent、AIOps、LoRA，偏综合 AI 应用。 |
| 刘洋 | 18673861525 | 未联系 / 待确认 | Agentic 科研服务平台，偏 RAG/AgentOps。 |
| 王泽超 | 15158269252 | 未联系 / 待确认 | Selenium + RAG，已列为补位。 |
| 王俊伟 | 15518376670 | 未联系 / 待确认 | 智能运维 Agent，偏 AIOps/RAG。 |
| 吴鹏伟 | 13603250371 | 未联系 / 待确认 | 多 Agent、RAG、LoRA。 |

## 3. 面试进展

### 当前状态汇总

- 已面试 / 已处理：4 人。
- 明确通过二轮：肖雨琴。
- 已联系待确认：宋琳琳、李明婷。
- NG：杨润芝。
- 当前新岗位第一优先 6 人：都还处于未联系 / 待确认，需要今天开始联系。
- 补位 8 人：都还处于未联系 / 待确认。

### 今天建议动作

1. 先打第一优先 6 人：李烨、黄浩男、舒泽林、刘衡、李夏洋、孙奇。
2. 如果前 6 人里约不到 4 人，就按补位顺序继续打：刘心怡、戴霖、王泽超、黄仟秋、田宏越、刘逍龙、高敬杰、邓靖俊。
3. 每通电话后立即回填 [contact-tracking.md](contact-tracking.md)。
4. 若有 3-4 人明确愿意面，且能讲代码/GitHub/demo，可以开始安排下一轮技术一面。
5. 若自动化运营是重点，刘衡必须优先约；王泽超/卢旭作为浏览器自动化补充。

### 只需要看的文件

- 总览与决策：当前文件 [interview-overview.md](interview-overview.md)
- 打电话清单：[today-contact-list.md](today-contact-list.md)
- 记录联系进展：[contact-tracking.md](contact-tracking.md)
- 技术面打印：[output/pdf/ai-agent-rag-interview-pack.pdf](../output/pdf/ai-agent-rag-interview-pack.pdf)

其他文件保留为详细资料，日常不用优先看。
