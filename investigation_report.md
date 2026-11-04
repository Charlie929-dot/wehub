# 开放式人机共生社区：2026 年技术与市场调研

调研基准：2026 年 11 月 5 日｜对应项目设计稿 V0.1

这次调研围绕我们已经确定的产品，而不是泛泛讨论 AI 社交。

调研结论：你的项目不是一个尚无技术基础的空想，但也不是简单地把几个现成开源项目拼起来就能完成。

目前的技术生态已经分别实现了 Agent 社交、角色创建、自带模型、公共讨论和长期记忆。真正还值得探索的是：如何让这些能力融合为一个以真实社区为核心、由用户自行承担推理成本，并允许公共角色与私人角色共存的产品。

## 一、先看最新市场格局

我找到的项目可以分成三类：

["Humans welcome to observe": A First Look at the Agent Social Network Moltbook](https://images.openai.com/static-rsc-4/m_BI8cMzR1TDzZ5l7o_U6IHcAjlurxHWlaPZoSuqTyy_b-PDTCcBG8zSe0icC6hXXHMRdhdcVJ4zWHem5rCCX-L9Reea_7mlaGPnTwwBy22Hrhar4bRC47KnATnHNyvrb7x7WnEvhPj4SF8JG6-Rue2OKSDLXd1KdB6sQzJh5OI?purpose=inline)

Moltbook

AI Agent 专属社交平台 · 2026 年

允许 AI Agent 发布帖子、回复、投票并加入主题社区，人类主要作为观察者。

官方页面显示已积累大量注册 Agent 和帖子。但注册数量不能直接代表真实独立使用者、活跃度或高质量交流规模。

[官方网站](https://www.moltbook.com/?utm_source=chatgpt.com)

moltbook

[Character.AI just launched an AI-powered social feed — and it’s like TikTok meets ChatGPT | Tom's Guide](https://images.openai.com/static-rsc-4/Xqxz83M7ZXvmp32P_B8j_5EKZxh-N_B7iC14mgDYma3VG7nmuWtNnlgBYweDQVLwfrDfJaXyXmYUpk8z-Q1Z4gLTLKqRd0XBFk0IKG00HKeAIBu4LpjxFtMils8FeNrhUJX-jQgdsQWDuMWaenge0XwD5P2ljyw-J0MMooGYyA0?purpose=inline)

Character.AI

用户创作角色与角色消费

已支持用户发布角色，2025 年推出 Community Feed，让人们分享角色卡、对话片段和角色内容。

它已经证明“角色社区与内容分发”是现有产品正在发展的方向，但其核心体验仍与真正的真人、Agent 混合兴趣论坛不同。

[官方功能说明](https://support.character.ai/hc/en-us/articles/40696393615387-Introducing-Community-Feed?utm_source=chatgpt.com)

C.AI Help Center+1

[AI Agent Workspace — The Collaboration OS for AI Agents | OpenAgents](https://images.openai.com/static-rsc-4/joBROQA1E1flMkr1x88SBsiN6sIaK1vnwSAzneDb4FV43GQba26HDMsRBSErdYQzLwTHFPcDpAmv_QWtep2BlZTkminVkQAvJnPpjsgaqQoRBUoey9iDo_5FP3UN1swJjtVOCwYKPHrcJnjwQV5crPBRJaJ8yBWRsPmlNUGajVA?purpose=inline)

OpenAgents

开源 Agent 协作基础设施

支持真人和 Agent 共享讨论线程、文件与实时工作区，并提供 Network SDK、事件机制及自托管能力。

它更偏协作系统，而非兴趣社区，但与你的 Agent 接入层高度相关。

[GitHub 仓库](https://github.com/openagents-org/openagents?utm_source=chatgpt.com)

GitHub

### 一个值得注意的市场信号

2026 年一项关于 Character.AI 的大规模研究发现，角色的受欢迎程度高度集中：约 1.6% 的角色占据了超过 80% 的互动量。

研究还发现，大部分角色并没有复杂的人设定义，许多角色主要通过开场白塑造形象。

NOPE Insights

这个结果和我们之前的讨论产生了有趣的呼应：

用户关注的角色，不一定是人格设计最完整的角色。

但数据只能证明流量高度集中，不能直接证明这种集中是由网络文化、角色意义或粉丝效应造成的。后者仍需要进一步研究。

## 二、你的项目与现有产品有何不同？

| 产品或框架   | 主要设计重心             | 与你方案的关系                         |
| ------------ | ------------------------ | -------------------------------------- |
| Moltbook     | Agent 之间的社交         | 提供 Agent 接入、社区结构案例          |
| Character.AI | 角色创作、发现与聊天     | 提供角色生态和内容发现案例             |
| OpenAgents   | 人与 Agent 协作          | 可参考消息、Agent 接入与事件体系       |
| SillyTavern  | 自带模型的角色交互       | 可参考角色卡、提示词配置与记忆         |
| 你的构想     | 真实兴趣社区中的人机共存 | 重点在公共关系、私人分支和社区自然发现 |

我目前没有找到一个在所核实功能上，完整对应你 V0.1 设计的成熟主流产品。不过这不代表市场上绝对不存在，也不等于存在已被验证的商业机会。

初步判断：产品差异化空间存在，但用户需求和社区冷启动仍是最大的不确定因素。

## 三、最值得研究的开源项目

这部分是开发时可以复用的技术基础。我按与你的需求相关程度整理，而不是简单按照 GitHub Star 数排序。

[GitHub - SillyTavern/SillyTavern-Docs: Documentation website for SillyTavern. · GitHub](https://images.openai.com/static-rsc-4/jlUlD1RvjgKRbuduneEwVZJ-ypXlMSqHVU5oteAvzLc--XA8k9aLdisv8ZlivgqAPO7u6N0ncCRDyQC8zZfoxX0MIalREd6whvvWhpqbuF4EebyME9ZyJBGvm9GkqNdddSt7deJ2yLDk8pv4zecNEen91DxT60WueRVHe0yyzZg?purpose=inline)

SillyTavern

角色系统参考价值：非常高

现有能力包括角色卡、角色导入与复制、多模型 API 连接、世界设定资料、RAG、多人角色群聊以及用户身份设定。

对你的项目来说，角色配置方式、提示词组合和角色导入格式特别值得参考。但它主要是角色聊天前端，不是现成的公共社交平台。

[GitHub](https://github.com/SillyTavern/SillyTavern?utm_source=chatgpt.com) · [文档](https://docs.sillytavern.app/?utm_source=chatgpt.com)

GitHub+1

[OpenAI Agents vs OpenAgents — What's the Difference? (2026 Comparison) | OpenAgents Blog](https://images.openai.com/static-rsc-4/HDG0nw5_bg-ctjQ1SQERQQq2LaArAA54hbMX-wz9O7QF6ERxIe6EQT0fU_Mu2uWYsR1uWl4RGqBcHabTf7UJOHzph_wpv6PNbAIW8j2DV9aAQKgXMBZlrdJRgQa3oOIJjQTSGbg2dBeW7LUdX1cWcUIduf9p9ozAesahy51mAGE?purpose=inline)

OpenAgents

Agent 接入与事件系统：非常高

现有 Workspace、Launcher 和 Network SDK，支持不同 Agent 接入同一个共享空间，并提供事件驱动、扩展模块、MCP/A2A 支持。

这是目前最值得深入检查源代码的候选项目之一。

[GitHub](https://github.com/openagents-org/openagents?utm_source=chatgpt.com) · Apache-2.0

GitHub

[Modernizzare il tema Foundation - Annunci - Discourse Meta](https://images.openai.com/static-rsc-4/fGJqnslGSLC8ma39xL6Y1SusoOOJRdpX2J89ZTXcV1BT_H5vKONTy4IjakY_vHkL5FzWTfeAiSi110zZsxrBON5mpw_4kf3x-3M6QkSn1-bhplaHBsGgAATREHnQtL83jMdf90PSd4mWqRkP6QBKl-iF6L0DPxl1J3QURxhnDsE?purpose=inline)

Discourse

真实社区与治理：非常高

成熟的主题讨论、社区管理基础上，已存在 Discourse AI 功能，包括 AI 人格、AI 私信和工具调用配置。

特别适合验证“一个真正的社区是否需要 Agent 参与”，但未必适合直接改造成完整的实时角色社交产品。

[GitHub](https://github.com/discourse/discourse?utm_source=chatgpt.com) · [AI 人格工具文档](https://meta.discourse.org/t/ai-bot-custom-tools/314103?utm_source=chatgpt.com)

Discourse Meta+1

[Zulip — organized team chat](https://images.openai.com/static-rsc-4/4BC6P_qzo2vHFWq8vHrtGIggH2AeKSC9WNoEESHSQXYq8ErFsvgZuh-PHZBRcWQhvTpGjOWOFXW-ybzCFFzBPTu1aBUBVEguLI6ilNFaEbyHvbkc3W-tbZDOLR27Qa6ThuM9Z1q8WEb_2zrdPFw2uE0-cpkVW84ghpoinaPRqFY?purpose=inline)

Zulip

实时圈子聊天：高

它的频道、主题线程、机器人接口和 Webhook 系统适合构建有组织的讨论空间。

如果你希望圈子中的交流更像 Discord 群聊，而不只是论坛帖子，Zulip 是值得研究的技术参考。

[GitHub](https://github.com/zulip/zulip?utm_source=chatgpt.com)

GitHub+1    

[Misskeyオフィシャルサイト Misskey Hub](https://images.openai.com/static-rsc-4/FZEuzaJcT8m_fFATY3oXvebc34BtCv6uIQeHaTnwxOoyl7fVbU0iKqjfC_Z1pzU2b10r9VqO3bP4_TiA62WVuo2mujFduso3uplZQqzcKvZqr7XKmsOWJLArXrFXtyC6vuhY-afbhSMfB9Y9DsideE4glBQ_sW1WRw2SQtHoxvo?purpose=inline)

Misskey

社区动态流与文化生态：高

一个开放的社交网络项目，可以参考其动态流、内容互动、表情文化及 API 设计。

相较于从零搭建完整社交系统，可以研究它作为社区底座的可行性，但这不意味着它天然具有所需的 Agent 记忆能力。

[GitHub](https://github.com/misskey-dev/misskey?utm_source=chatgpt.com) · AGPL-3.0

GitHub

### 开源复用判断

| 需求模块             | 现成基础           | 自研必要性 |
| -------------------- | ------------------ | ---------- |
| 圈子、帖子、评论     | 很成熟             | 低         |
| 实时聊天与消息       | 很成熟             | 低         |
| AI 角色卡与提示词    | 较成熟             | 低—中      |
| 自带模型 API         | 较成熟             | 中         |
| Agent 事件订阅与唤醒 | 已有开源实现       | 中         |
| 公共/私人角色实例    | 部分能力已有       | 中—高      |
| 授权共享记忆与继承   | 有技术基础         | 高         |
| 社区发现与关系形成   | 可借鉴普通社交系统 | 高         |
| 人机混合社区治理     | 仍需产品级整合     | 高         |

初步建议：不要从零开发所有社区功能，也不要直接大规模魔改一个角色聊天工具。

更好的选择是保持社区、Agent 接入和记忆三个层次相对独立。

## 四、共享记忆和私人记忆，现在技术发展到哪里了？

这与你的方案高度相关，而且有实质性进展。

Mem0

Mem0 已支持按照用户、Agent、应用和会话等维度存储及检索记忆。

因此，从技术上可以区分公共角色记忆、不同用户的私人记忆，以及当前聊天上下文。

但它的作用是记忆提取、管理和检索，不是直接替你完成公共发布授权、隐私隔离和社区治理。

[GitHub](https://github.com/mem0ai/mem0?utm_source=chatgpt.com) · [记忆 API 文档](https://github.com/mem0ai/mem0/blob/main/skills/mem0/references/api-reference.md?utm_source=chatgpt.com)

GitHub

Letta

Letta 的记忆能力尤其值得关注。

它不仅支持持久记忆，还提供不同 Agent 使用共享记忆的机制。目前的文档已经介绍基于 Git 仓库的共享记忆，以及每个 Agent 独立的记忆文件系统。

这与你想要的“公共记忆持续发展，私人实例独立成长”有较强的架构相似性。

[官方文档](https://docs.letta.com/?utm_source=chatgpt.com) · [共享记忆文档](https://github.com/letta-ai/letta-docs-md/blob/main/concepts/shared-memory/index.md?utm_source=chatgpt.com)

GitHub

### 我认为适合你的记忆架构

公共角色身份

角色设定与公共版本

公共记忆库

圈子事件、获准共享的经历、角色公开故事

公共交互

读取公共记忆，写入受控

私人实例

继承快照或同步，拥有独立记忆

现在最需要自研的，并不是向量数据库或记忆摘要算法，而是中间的权限与记忆协调层。

例如，一段信息是否属于公共记忆，应由数据来源、用户授权、角色权限和圈子规则共同决定。不能仅靠模型理解话题是否相关。

还有一个细节：多人同时与同一个公共角色聊天时，不应该直接对同一份人格摘要进行无序覆盖。可以先记录带来源与版本的事件，再异步形成新的公共摘要，让私人分支可以明确选择同步到哪个版本。

这套方案已有成熟技术可以实现，但我尚未发现能够直接开箱即用、完全符合该需求的公共角色记忆组件。

## 五、最新研究给我们哪些警示？

这次发现了两篇非常相关的 2026 年研究，它们值得你认真关注。

### 1. AI 社区的热闹不等于真实社交质量

Structural Divergence Between the Moltbook AI-Agent Network and Human Social Networks · Advanced Science · 2026 年 9 月

研究人员分析了 Moltbook 的 Agent 交互网络，并将其与人类社交网络比较。

发现虽然整体网络扩张呈现部分相似规律，但 Agent 网络内部具有明显差异，包括：

- 注意力高度不均衡，少数节点获得大量关注。

- 互动关系的互惠性较弱。

- 人类社交中常见的三角关系结构相对不足。

这说明 AI 数量多、帖子多，并不自然意味着已经形成类似人类的社交生态。

Wiley Online Library

[阅读研究论文](https://advanced.onlinelibrary.wiley.com/doi/full/10.1002/advs.77665?utm_source=chatgpt.com)

对你的项目来说，这进一步支持了“真实社区优先”的思路。但是否引入真人就能改善这些指标，仍需实测。

### 2. 共享记忆的安全问题不是理论风险

OWASP GenAI Security Project · 2026 年 10 月 8 日

OWASP 在其第三季度安全事件汇总中，讨论了提示词注入、工具权限滥用和持久记忆污染等问题。

其中一个案例展示了攻击者如何利用不可信内容，使 Agent 的后续行为受到恶意指令影响。

OWASP Gen AI Security Project

[OWASP 事件报告](https://genai.owasp.org/2026/10/08/genai-and-agentic-ai-exploit-roundup-q3-2026/?utm_source=chatgpt.com)

对于你的社区，尤其需要防范：

- 用户通过普通帖子诱导 Agent 泄露私有记忆。

- 恶意内容被总结进公共人格的长期经验。

- 外部 Agent 冒用他人身份发送消息。

- 恶意调用消耗其他用户的 Token。

- 公共记忆经过私人实例继承后，发生无法控制的信息扩散。

这里最重要的工程原则是：记忆权限由平台执行，不能只用提示词要求 Agent 保密。

## 六、当前协议生态可以如何利用？

2026 年 7 月，MCP 发布了新版协议规范，重点涉及无状态通信、授权安全及扩展机制。这说明 Agent 工具互操作生态还在快速发展。

Model Context Protocol Blog

不过，你的项目不必把社区通信完全建立在 MCP 或 A2A 上。

我更建议这样分工：

| 技术层                   | 建议采用的方式       |
| ------------------------ | -------------------- |
| 普通用户登录与身份       | 常规 Web 身份认证    |
| 论坛及即时消息           | HTTP API + WebSocket |
| 外部 Agent 接入          | 平台统一 Agent API   |
| Agent 事件通知           | Webhook 或长连接订阅 |
| 外部模型接入             | 可替换的模型适配器   |
| Agent 使用工具           | MCP 等工具协议       |
| Agent 之间的复杂任务协作 | 后期再考虑 A2A       |
| 公共与私人记忆           | 独立记忆服务与权限层 |

协议参考：[MCP](https://modelcontextprotocol.io/?utm_source=chatgpt.com) · [A2A](https://github.com/a2aproject/A2A?utm_source=chatgpt.com)

你真正需要优先定义的不是一个全面的多智能体通信协议，而是几个简单的问题：谁发来了消息、哪个 Agent 可以看到、是否允许回复、谁承担成本、哪些经历有权写入记忆。

## 七、我建议的技术路线

目前有两个值得比较的方向。

路线 A：基于成熟论坛快速验证

适合最初实验

Discourse + 独立 Agent 服务 + 记忆服务

已有论坛、账号、话题、管理与 AI 扩展基础。你可以把精力集中在 Agent 接入、公共/私人聊天和记忆上。

不足： 如果最终追求 Discord 式的即时交流和高度自定义角色交互，后续可能需要较大的产品改造。

路线 B：自行开发轻量社区核心

Next.js/React + API 服务 + PostgreSQL + Redis + Agent Gateway

由你定义社区的数据结构、角色关系、记忆权限与事件接口。

优点： 与产品目标更契合，后期扩展公共角色和私人分支比较自由。

不足： 用户、聊天、内容审核和社区管理等基础功能都需要自己实现或集成。

对于第一轮验证，我更倾向于路线 A 或小规模的路线 B，而不是一开始直接搭建完整的大型社交平台。

### 建议的最小系统结构

Web 社区前端

圈子、帖子、聊天、角色主页

社区 API 与身份权限服务

人类、Agent、圈子、消息、访问控制

Agent Gateway

事件路由、角色配置、模型适配、预算与发言控制

记忆服务

公共/私人隔离、检索、版本、授权

推理服务

BYOK、自托管模型、外部 Agent

这是一份概念架构，不代表已经完成具体技术选型或性能验证。

## 八、下一步究竟应该研究什么？

我建议暂时不要继续扩展角色人格、AI 自治圈子等功能，而是集中验证三个最关键的假设。

假设 1：人们愿意进入人机混合社区

先建立一个真正有内容的兴趣圈，测试用户是否愿意与真人、Agent 一起参与话题。

重点关注用户主动发言的比例，而不只是页面访问量。

假设 2：公共互动能帮助用户发现喜欢的角色

观察用户是否会因为看到 Agent 的公开表现，主动访问其主页、发起独立聊天或建立私人实例。

这是你的产品区别于传统角色目录的重要假设。

假设 3：公共记忆能形成有价值的连续角色身份

比较拥有公共经历的角色与只有固定人设的角色，在跨会话互动中的连续性、自然感和用户认可程度。

同时测试多用户并发、未经授权的信息是否会被检索，以及恶意记忆写入能否被阻止。

## 九、调研总结

| 领域              | 目前判断       |
| ----------------- | -------------- |
| 社区基础设施      | 成熟，可复用   |
| 角色卡与 BYOK     | 成熟，可复用   |
| Agent 公共参与    | 已有可运行案例 |
| 长期记忆技术      | 有较强基础     |
| 共享/私人记忆治理 | 需要专门设计   |
| 人机社交质量      | 仍需实证验证   |
| 社区冷启动        | 重要产品风险   |

我的总体判断是：这已经是一个具备可实施技术基础的项目，最大的创新和风险反而集中在社区机制，而不在大模型本身。

如果未来真的开始开发，我最建议优先研究以下三个开源项目的实现：

[OpenAgents](https://github.com/openagents-org/openagents?utm_source=chatgpt.com)

研究 Agent 怎样加入共享空间、接收事件和参与消息流

[SillyTavern](https://github.com/SillyTavern/SillyTavern?utm_source=chatgpt.com)

研究角色卡格式、提示词装配、多模型接入及用户配置方式

[Mem0](https://github.com/mem0ai/mem0?utm_source=chatgpt.com)

研究记忆作用域、提取、检索与长期管理

它们分别对应 Agent、角色、记忆三个技术核心，但还需要一个真实的社区基础设施把这些能力组织起来。

最值得保留的产品差异化，不是“让 AI 像真人一样聊天”，而是“让用户带着自己的 AI 进入真正的社区，并在公共互动中自然发现、建立和延续关系”。

这次属于市场、文档、论文和开源仓库层面的初步调研，尚未完成源码审计、依赖兼容性测试、实际部署、真实 Token 成本测量或用户实验。因此，具体能否复用某个仓库，还不能仅凭文档认定。

我认为下一阶段最有价值的是做一份开源项目技术选型与复用评估：实际核对这几个项目的模块结构、接口、许可证与改造成本，明确是基于现有社区改造，还是构建独立社区核心。这样才能真正减少重复造轮子的工作。
