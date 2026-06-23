# 下周面试计划

更新日期：2026-06-23

适用周期：2026-06-22（周一）至 2026-06-26（周五）。这份计划是在原 2026-06-17 新岗位计划基础上追加新要求，不替代原来的浏览器自动运营 Agent / 通用 Agent 平台 / 工作流 / RAG 主线。

补充：2026-06-23 已并入两批新增简历。前一批里李昊泽、方浩、廖月华、王悦、朱坤进入新增补位 / 强初筛；最新追加批次里冯慧、李家璇、刘锐、李鑫、周升、刘少波、陈学志、赵景博、管瑞阳、胡景晟进入强初筛 / 技术一面补位。排序原则是岗位匹配优先；同档位、匹配度接近时女生候选尽量前置。

## 1. 本周目标

下周面试同时看两层：

- 原计划主线：浏览器自动运营 Agent、通用 Agent 平台、Claw/WorkBuddy/龙虾类 Runtime、Coze/Dify/LangGraph 工作流、RAG 工程化。
- 新增验证口径：候选人是否真的理解 Agent 的“思考、决策、反馈”闭环。

“Agent 思考/决策/反馈”具体按下面拆：

- 思考：任务拆解、Plan/ReAct/Plan-Execute、上下文构造、长期任务状态维护。
- 决策：意图路由、工具选择、Judge/Grader、重试/降级/停止条件、人工确认。
- 反馈：trace/eval、LLM-as-Judge、RAGAS、失败样例复盘、用户纠正进入记忆、benchmark 回归。

成功标准：

- 先约原计划第一优先 6 人，再补新增强匹配候选。
- 约到 8-10 场技术一面。
- 筛出 3-5 人进入技术二面或设计实操。
- 每个推进候选人都要能讲清代码、状态图、关键文件、评测方式和失败案例。

## 2. 下周排期总览

| 日期 | 上午 | 下午 | 目标产出 |
| --- | --- | --- | --- |
| 2026-06-22 周一 | 批量联系原计划核心：李烨、黄浩男、舒泽林、刘衡、李夏洋、孙奇；同步联系新增强匹配：胡选杰、赵绍猛、王博涵、周思行 | 技术一面优先排：李烨、黄浩男、胡选杰 | 先锁定通用 Agent 平台 / Runtime / Coding Agent 第一梯队 |
| 2026-06-23 周二 | 技术一面：刘衡、舒泽林 | 技术一面：赵绍猛、王博涵 | 同时覆盖浏览器/桌面 Agent 和思考-决策-反馈强候选 |
| 2026-06-24 周三 | 技术一面：李夏洋、孙奇 | 技术一面或强初筛：周思行、陈翔宇、侯永欣 | 补齐 OpenClaw、工具平台、客服 Agent、评测闭环方向 |
| 2026-06-25 周四 | 原补位池初筛：刘心怡、戴霖、王泽超、黄仟秋、田宏越 | 新增补位初筛：李昊泽、方浩、廖月华、王悦、朱坤；如需女生候选补位，优先加冯慧、李家璇 | 形成 A+/A-/候补/NG 初版 |
| 2026-06-26 周五 | 二面/设计实操：周一至周四通过者 | 面试官复盘、最终排序、回填跟进表；如有余量再初筛刘锐、李鑫、周升、刘少波、陈学志、赵景博、管瑞阳、胡景晟 | 输出 offer/候补/淘汰建议 |

建议排期粒度：

- 技术一面：60 分钟。
- 30 分钟初筛：只确认真实性、可实习周期、是否能讲代码。
- 技术二面/设计实操：90 分钟。
- 连续面试中间至少留 15 分钟做记录。

## 3. P0：优先约技术一面

P0 不是只按新增简历排序，而是把原计划核心和新增“思考/决策/反馈”强候选合并后排序。

| 优先级 | 候选人 | 简历文件 | 联系方式 | 主匹配方向 | 为什么优先 | 思考/决策/反馈追问 |
| ---: | --- | --- | --- | --- | --- | --- |
| 1 | 李烨 | `李烨-简历.pdf` | 17335610901 / 17335610901@163.com | Claw / 通用 Agent 平台 + RAG | 原计划核心。ClawAgent 本地优先多智能体工作台，覆盖会话队列、任务取消、权限审批、审计日志、SSE、Web 检索。 | 让他画 Agent 执行链路；追问会话 busy/follow-up 如何决策、任务取消后状态如何恢复、审计日志如何支持失败复盘。 |
| 2 | 黄浩男 | `黄浩男-Agent开发_AI应用开发 (2).pdf` | 13224672500 / hhn13224672500@163.com | Agent Runtime / Harness / Claw 类平台 | 原计划核心。Pure Coding Agent Harness 覆盖 Runtime、ToolCalling、ContextManagement、Checkpoint/Resume、JSONL trace、workspace 隔离。 | 强验证 GitHub；问 Runtime 主循环、工具调用失败如何重试/停止、checkpoint 校验、benchmark 如何驱动迭代。 |
| 3 | 胡选杰 | `我的简历 (1).pdf` | 13276387009 / 755877147@qq.com | Coding Agent / MCP / 多 Agent | 新增简历中最贴新要求。Coding Agent 写到 ReAct + Plan Mode、MCP、Skill、两层上下文压缩、五层权限拦截、自动记忆提取、多 Agent 协作。 | 追问 Plan Mode 与 ReAct 如何切换、工具 schema 延迟加载、用户纠正如何进入记忆、Coordinator Agent 如何汇总反馈。 |
| 4 | 刘衡 | `刘衡aiAgent开发简历.pdf` | 13708800655 / 453093656@qq.com | 浏览器自动运营 Agent + OpenClaw | 原计划核心。小红书内容运营自动化 Workflow 明确写 Playwright、内容抓取、爆款分析、生成、自动发布和 OpenClaw。 | 追问选题-生成-审核-发布-复盘如何决策；登录态/Cookie/验证码失败时如何反馈到流程；自动发布前人工确认怎么做。 |
| 5 | 舒泽林 | `舒泽林的简历 (1).pdf` | 17508510706 / 857824448@qq.com | 桌面 / 浏览器自动化 Agent | 原计划核心。AirJelly 桌面端主动式 Agent，覆盖截图、键盘状态、活跃窗口、主动触发、记忆和 benchmark。 | 追问主动触发的判定规则、截图理解如何归属 Task、用户反馈如何更新 Episodic/Semantic 记忆、benchmark 如何回归。 |
| 6 | 赵绍猛 | `赵绍猛-个人简历.pdf` | 15713380988 / 15713380988@163.com | AIOps Agent Harness / 工具治理 | 新增简历中 Harness 和治理意识强：模型调用、工具执行、上下文压缩、审计、工具权限、失败/超时/重试、防无限 ReAct loop、长期记忆和评测。 | 问 Harness 是否自研；工具治理状态机、重试停止条件、审计字段、长期记忆去重/遗忘、AIOps 真实代码。 |
| 7 | 李夏洋 | `简历.pdf` | 15518794255 / 15518794255@163.com | Agent Runtime / 通用平台 | 原计划核心。Mira Runtime 覆盖 Event Stream、State Machine、ReAct Loop、Tool/Skill、ContextBuilder/Compactor。 | 要求画状态机；追问 ContextBuilder 何时压缩、工具结果如何进入 observe、失败后如何 resume。 |
| 8 | 孙奇 | `孙奇_AI_Agent开发实习6个月以上.pdf` | 18405675136 / 1446437177@qq.com | OpenClaw / 工具平台 / 工作流 | 原计划核心。OpenClaw Plugin SDK、40+ 工具、网页截图、HTML 渲染、工作流调度、长期记忆和安全边界。 | 问插件 schema、40+ 工具如何权限分级、网页截图结果如何反馈给工作流、长期记忆如何做用户隔离。 |
| 9 | 王博涵 | `王博涵_杭电27届硕.pdf` | 18991120513 / 1433340920@qq.com | Agentic RAG / 评测闭环 | 新增强候选。Agentic RAG 明确包含 Routing、Grading、Self-Reflection 节点，另有 RAGAS、Prometheus、request_id 日志、法律 Agent 自动化评测。 | 追问 Grading/Self-Reflection 触发条件、30 条黄金集是否够、Tool Calling Success Rate 如何测、Dify 与自研 LangGraph 边界。 |
| 10 | 周思行 | `后端&Agent实习-周思行-13350756085.pdf` | 13350756085 | 多 Agent 路由 / Monitor 闭环 | 新增强候选。DealFlow AI 写到三路意图识别、三级记忆、多 Agent 动态路由、Monitor 闭环、工具熔断降级、LLM-as-Judge。 | 问 Monitor 如何把成功率/延迟转成路由惩罚因子、LLM-as-Judge 一致性、工具熔断阈值、复合问题并行协作边界。 |

## 4. P1：约技术一面或强初筛

| 候选人 | 简历文件 | 联系方式 | 判断 | 建议动作 |
| --- | --- | --- | --- | --- |
| 陈翔宇 | `陈翔宇-简历.pdf` | 18253832648 / 18253832648@163.com | MedAgent 覆盖 ReAct Agent、MCP、Function Calling、Adaptive RAG + Self-RAG、RAGAS 异步评估、云端失败回退本地模型。 | 周三技术一面或强初筛，重点查是否真有完整前后端和 MCP 代码。 |
| 侯永欣 | `侯永欣-个人简历-井盖+智能客服.pdf` | 18238052603 / 2376687078@qq.com | LangGraph 智能客服 RAG Agent 写到路由决策、JSON 命令、工具 schema、发票确认、agent_trace/retrieval_trace/tool_trace/eval_record。 | 周三技术一面或强初筛，重点看 trace/eval 数据模型和工具确认机制。 |
| 李子昊 | `附件简历-李子昊-后端开发-29年应届生.pdf` | 18302774840 / liziar7@gmail.com | 新增 2026-06-22。Agent Loop、MCP、四层上下文压缩、Orchestrator、多 Agent 协作、RAG-MCP、PR Copilot 两层 DAG 规划，贴“思考/决策/反馈”口径。 | 周四强初筛；重点问 Orchestrator、两层 DAG 规划、maxRetries=2、失败降级、Golden Test Set 与 RAGAS。 |
| 来淼鑫 | `来淼鑫简历.pdf` | 18335933458 / 1307837569@qq.com | 新增 2026-06-22。多 Agent 医疗临床辅助决策系统写到 5-Agent Pipeline、条件路由、共享状态模型。 | 周四强初筛；问条件路由、ClinicalState、信息不足回退、ICD-10 接口和 100+ 用例测试。 |
| 雷剑 | `雷剑-实习简历-27应届生.pdf` | 13203543481 / leijian0905@163.com | 新增 2026-06-22。LangGraph + FastMCP 出行 ReAct Agent、stdio/SSE、多用户上下文隔离、RAGAS 评估。 | 周四强初筛；问 FastMCP、会话隔离、工具接入效率 90% 口径、RAGAS 和全链路异步。 |
| 刘心怡 | `刘心怡_武汉大学硕士_大模型应用开发616.pdf` | 13852765692 / liuxy66880@163.com | 原计划补位。CareerPilot 多 Agent 和 Agentic RAG 稳，适合 RAG/工作流强补位。 | 周四初筛；重点问反思补检、MCP Tool Manager 和评测闭环。 |
| 戴霖 | `应聘Agent应用开发实习生—27年应届生北科大戴霖简历.pdf` | 18900727703 / 18900727703@163.com | 原计划补位。OnCall AIOps Agent 工程化好，适合运维 Agent/RAG。 | 周四初筛；问 Golden Set、软拒答阈值、MCP 工具和 Redis 锁。 |
| 王泽超 | `王泽超_Agent简历.pdf` | 15158269252 / wzc294621327@gmail.com | 原计划补位。Selenium 动态网页抓取、验证码/Cookie，兼具 RAG 评估平台。 | 周四初筛；问 Selenium 稳定性、验证码/Cookie 复用和网页抓取失败反馈。 |
| 黄仟秋 | `黄仟秋.pdf` | 15399760679 / huangqianqiu7@qq.com | 原计划补位。DataAgent-Bench、trace/metrics、工具边界和 RAG 后端。 | 周四初筛；问 benchmark、工具隔离、SSE 契约和失败兜底。 |
| 田宏越 | `简历1.pdf` | 15253882785 / 15253882785@163.com | 原计划补位。Agent Harness、PLAN-EXECUTE-VERIFY、四层记忆、311 个 pytest。 | 周四初筛；问 Harness 自研程度、VERIFY 阶段怎么判定、测试覆盖。 |
| 刘逍龙 | `刘逍龙18940802759 agent应用开发工程师.pdf` | 18940802759 / changqingbest@163.com | 原计划补位。Coze 工作流 + 后端 Agent。 | 如果 P0/P1 约不满再补；问 Coze 节点编排、插件接入、自研 Agent 差异。 |
| 高敬杰 | `高敬杰河北工程大学.pdf` | 13483000182 / 3077618869@qq.com | 原计划补位。Go/Eino Agent 后端，MCP、Milvus/MySQL 分层记忆。 | 如果需要 Go 后端 Agent 补位再约；问 Eino 编排和 MCP 工具边界。 |
| 邓靖俊 | `邓靖俊--AI应用实习--.pdf` | 13541043150 / jingjun_deng@qq.com | 原计划补位。RAG + LangGraph Agent + QLoRA。 | 如果需要 RAG/应用 Agent 补位再约；问工具调用上限、动态 Prompt、checkpoint。 |

## 5. 2026-06-23 追加批次：强初筛 / 技术一面补位

这一批不替代 P0，但可作为本周约面不足、或希望增加女生候选时的直接补位池。

| 候选人 | 简历文件 | 联系方式 | 判断 | 建议动作 |
| --- | --- | --- | --- | --- |
| 冯慧 | `冯慧_简历 (11).pdf` | 15002602703 / fenghui@bupt.edu.cn | 北邮本硕，AIOps Agent 平台覆盖 LangGraph、Plan-Execute-Replan、MCP、RAG、SSE 和重试机制。 | 周四/周五强初筛或技术一面；重点问 AIOps 状态机、MCP 工具、重试停止条件和个人代码。 |
| 李家璇 | `李家璇简历.pdf` | 15036583295 / Lijiaxuan@henu.edu.cn | Agentic Knowledge Hub 与 AgentFlow 客服平台覆盖 RAG 多阶段检索、Agent 任务拆解和 Dify 工作流。 | 强初筛；重点问混合召回、Agent 任务拆解、Dify 与自研后端边界。 |
| 刘锐 | `agent简历.pdf` | 18214794197 / 2196290715@qq.com | 供应商资质联合审查覆盖 LangGraph 多 Agent、OCR/RAG/Text-to-SQL、Playwright 信用调查和 RPA 自动填报。 | 技术一面补位；重点问 Supervisor-Worker、Playwright/RPA 调用边界、ReAct 自纠错和人工审批。 |
| 李鑫 | `李鑫_19862255726.pdf` | 19862255726 / znnn2004@163.com | 医疗问答 Skills-Agent 双层架构、ReAct、Agent Swarm、双层记忆；教学系统有 LangGraph、MCP、RAGAS、LangFuse。 | 技术一面补位；重点问 Agent Loop、Swarm 路由、工具调用限制、记忆压缩和反思节点评测。 |
| 周升 | `周升__大模型应用开发_2027届.pdf` | 13476527154 / 13476527154@163.com | 气象 SkyNexus 多 Agent 系统覆盖 Plan-Execute-Reflection、ReAct、多轮反思、Memory、标准化工具 API 和 RAGAS。 | 强初筛；重点问反思 Agent 校验标准、气象工具超时降级和 RAGAS 指标来源。 |
| 刘少波 | `刘少波-简历.pdf` | 18826340457 / 2505632210@qq.com | 智能果园多 Agent 调度体系，覆盖 StateGraph、条件边、checkpoint、IoT 数据注入、KG + RAG、QLoRA。 | 强初筛；重点问四类 Agent 路由、Checkpoint 恢复、IoT 数据影响决策和 Cypher 查询。 |
| 陈学志 | `简历_副本2.pdf` | 15338571351 / a35661353@163.com | Windows 操控 Agent 覆盖 RAG、VLM、Win32 API / UI Automation、意图澄清和记忆，适合自动化方向补位。 | 强初筛；重点问屏幕理解、UI 元素库、执行失败反馈和安全边界。 |
| 赵景博 | `赵景博-Java全栈开发工程师-27年应届生.pdf` | 15703278840 / 3323076514@qq.com | AGI Assistant 覆盖 DAG Agent Workflow Runtime、GraphRAG、三层记忆、Harness 容错和 RAGAS benchmark。 | 强初筛；重点问 DAG 拆分、拓扑调度、Tool Isolation、记忆演化和 benchmark。 |
| 管瑞阳 | `简历 (1).pdf` | 18535918722 / 3219402441@qq.com | 企业 RAG 与 DeepAgents 深度搜索项目覆盖 LangGraph、RAGFlow、FastAPI、WebSocket 和 ContextVar 隔离。 | 强初筛或补位；重点问 DeepAgents 链路、上下文隔离、异步推送和报告生成。 |
| 胡景晟 | `resume.pdf` | 16639239639 / 3573851322@qq.com | 独立 AgentOrchestrator 覆盖 Planning -> Tool Use -> Memory -> Output、asyncio、Pydantic 校验和 SSE。 | 30 分钟强初筛；重点看 GitHub、自研边界、Memory 设计和工具错误拦截。 |

## 6. P2：30 分钟初筛后再决定

| 候选人 | 简历文件 | 联系方式 | 初步判断 | 初筛问题 |
| --- | --- | --- | --- | --- |
| 李炎铭 | `Golang-李炎铭.pdf` | 17877388141 / yuliu666666@outlook.com | Go 后端强，RPA 测开做过小红书、抖音、电商 B/C 端数据采集、处理、发布；LLM Agent 证据弱。 | 问登录态、页面变化、自动发布边界和能否补 Agent 决策层。 |
| 刘聪志 | `刘聪志简历.pdf` | 18336136469 / 948290202@qq.com | Function Calling 工具白名单、错误重试、LangGraph 四角色深度研究，偏应用层。 | 问工具选择、最多重试 2 次、Reviewer 不通过如何循环和执行轨迹。 |
| 张文元 | `张文元的简历 (6).pdf` | 13087078935 / 1227696033@qq.com | QQ Bot + RAG 长期记忆 + Playwright 网页爬取，偏群聊助手。 | 问 Playwright 网页记忆、命令路由、安全防护和代码真实性。 |
| 温博 | `温博-实习简历.pdf` | 19703315953 / 2635658259@qq.com | AI 面试助手，有六类意图识别、有限状态机、混合检索、追问和总评闭环。 | 问状态机、追问触发、LLM 失败兜底和 RAG 评测。 |
| 邢耀文 | `邢耀文的简历.pdf` | 18553583536 / 709450270@qq.com | AI CodeReview、AI 友好型项目、团队知识库、短期/长期记忆和 RAG，反馈意识有，但通用 Agent Runtime 证据少。 | 问 AI CR 是否有真实代码、问题分类如何评估、AIReadMe 对上下文稳定性如何验证。 |
| 牛韦杰 | `简历_副本.pdf` | 18735634480 / 1071294398@qq.com | 航发工业 RAG，证据追溯、测试清单、问题归因较好，更偏 RAG 评测和工业知识库。 | 问 800+ 测试问题、召回片段记录、业务专家校验闭环、Agent 工作流实际做了什么。 |
| 郝海程 | `个人简历_副本.pdf` | 18864771568 / 2020104216@qq.com | GraphRAG、DeepAgents、SFT、vLLM、Coze/Dify 都覆盖，但简历表述偏满，需要核实。 | 问 GraphRAG 多跳推理、DeepAgents 实际调用链、SFT 数据和部署证据。 |
| 于嘉琪 | `于嘉琪-28届-硕士.pdf` | 18397186227 / 3148418980@qq.com | LangGraph + Function Calling + RAG + 短期/长期记忆，完整但偏常规应用。 | 问工具注册机制、记忆持久化、RAG 评测、项目地址是否可打开讲。 |
| 徐志磊 | `求职简历python (1).pdf` | 13522488690 / 1346681005@qq.com | GraphRAG + 多 Agent 旅行规划，适合作为低优先补位。 | 问 4 个 Agent 如何协作、API 不可用时降级策略、GraphRAG schema 注入。 |
| 薛景瑞 | `个人简历-薛景瑞.pdf` | 18035756241 / 18035756241@163.com | 新增 2026-06-22。做过 JD 匹配简历优化 RAG、扫地机器人 ReAct Agent、多 Agent 学习助手，但整体更偏常规应用。 | 低优先初筛；重点问 7 种工具调度、动态 Prompt 切换、工具顺序约束和多 Agent 结果流转。 |

暂缓占用技术一面：

- 丁帅：企业 RAG + Function Call，偏 Java 后端知识库，Agent 决策/反馈闭环弱。
- 张鼎琛：AI 互动叙事和真实业务项目不错，但与当前 Agent 决策反馈方向不够贴。
- 雷嘉圣：主要是 CV/机器学习/管理科学，不适合当前岗位主线。
- 王欣宇：水利/GIS 知识库、知识图谱和智能体，女生候选但主岗匹配一般，可低优先补位。
- 刘佳璇：北航拟入学，Coze 工作流应用较轻，需先确认可实习周期和实际开发深度。
- 黄广荣：UCAS 硕士，企业知识库 RAG 完整但更偏 RAG，不占用主岗优先技术面。
- 李士博：扫地机器人智能客服 Agent + RAG，需先人工补联系方式。
- 徐阳阳：吉林大学硕士，LLM 冗余推理抑制和 LoRA/全参微调强，作为训练加分项备选。
- 黄可心：`黄可心-北理工28届-agent开发.pdf` 当前 PDF 文本抽取不可读，需人工打开确认。
- 刘源哲：`附件简历-刘源哲-agent应用开发工程师-28年应届生.pdf` 文本抽取基本不可读，需人工打开确认后再判断。

## 7. 技术一面结构

时长：60 分钟。

| 时间 | 内容 | 必须拿到的信息 |
| --- | --- | --- |
| 5 分钟 | 项目选择 | 让候选人选一个最能体现原岗位主线和 Agent 思考/决策/反馈的项目，不要泛讲所有项目。 |
| 10 分钟 | 主链路复述 | 用户输入后经过哪些状态：context -> plan -> tool -> observe -> judge -> revise/stop。 |
| 15 分钟 | 决策机制 | 路由、工具选择、重试、降级、停止条件、人工确认分别由谁决定，依据是什么。 |
| 15 分钟 | 反馈闭环 | trace/eval 记录哪些字段，失败样例如何回放，用户纠正如何进入记忆或 benchmark。 |
| 10 分钟 | 代码真实性 | 能否指到 GitHub/demo/核心文件；指标、测试集、baseline、个人负责范围是否说得清。 |
| 5 分钟 | 实习条件 | 到岗时间、每周天数、持续月数、是否能稳定参加后续面试。 |

技术一面一票否决项：

- 只能讲概念，无法画状态图或说清节点输入输出。
- 指标没有数据集、脚本、baseline 或失败样例。
- 声称自己实现 Harness/Runtime，但无法说明核心文件和主循环。
- 对高风险工具调用没有权限、审计、人工确认或回滚意识。

## 8. 技术二面/设计实操

时长：90 分钟。

题目：设计一个“可自我纠错的浏览器自动运营 / 知识工作 Agent 平台”。

候选人必须讲清：

- 任务如何进入系统：用户任务、上下文、历史记忆、权限身份。
- Agent 如何思考：任务拆解、plan 更新、上下文压缩、状态持久化。
- Agent 如何决策：工具选择、检索是否足够、是否重试、是否人工确认、何时停止。
- Agent 如何接收反馈：工具结果、浏览器页面结果、RAG 召回质量、用户纠正、线上 trace。
- 如何避免失控：无限循环、错误工具、越权操作、重复发布、账号风控、低质量检索。
- 如何评测：离线 benchmark、回归集、LLM-as-Judge、RAGAS、人工抽检、线上监控。

评分建议：

| 维度 | 分值 | 判断标准 |
| --- | ---: | --- |
| 原岗位主线匹配 | 20 | 浏览器自动化、通用 Agent 平台、工作流或 RAG 至少有一个方向扎实。 |
| Agent 思考/决策链路 | 25 | 能画状态机，讲清每个决策点和停止条件。 |
| 反馈与评测闭环 | 20 | 有 trace、eval、失败回放、用户反馈进入系统的闭环。 |
| 工具安全与工程落地 | 20 | 有权限、审计、人工确认、重试、熔断、checkpoint/resume。 |
| 真实性与表达 | 15 | 能讲代码、指标来源、个人职责和真实取舍。 |

## 9. 电话确认话术

首次接通：

你好，请问是「候选人姓名」吗？我这边是浏览器自动运营 Agent / RAG / 通用 Agent 平台方向实习岗位的面试安排人。我们看了你的简历，觉得你在浏览器自动化、Agent 平台、RAG、工作流，或者 Agent 思考决策反馈闭环方面比较匹配，想确认你现在是否还在看实习机会。

需要确认：

1. 最早什么时候可以开始实习？
2. 每周可以实习几天？
3. 可以持续几个月？
4. 技术面是否可以展开讲代码、GitHub、demo 或核心文件？
5. 你最熟的 Agent 项目里，是否能讲清 plan / route / tool call / evaluate / retry 这一整条链路？

未接短信：

你好，我是浏览器自动运营 Agent / RAG / 通用 Agent 平台方向实习岗位的面试安排人。看到你的简历和岗位方向比较匹配，刚才电话联系未接。想确认你目前是否还在看实习机会，以及是否方便安排一次技术面。技术面会重点聊项目代码、Agent 工具决策、反馈评测闭环和工程落地。方便的话可以回复可面试时间、最早到岗时间、每周可实习天数和可持续月数，谢谢。
