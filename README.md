# AwesomeQuickDev

![Packagist Stars](https://img.shields.io/github/stars/bfchengnuo/awesome-quick-dev?style=flat-square)
![GitHub last commit](https://img.shields.io/github/last-commit/bfchengnuo/awesome-quick-dev?style=flat-square)
![status](https://img.shields.io/badge/更新状态-怠惰-%2366ccff?style=flat-square)
[![知识共享协议（CC协议）](https://img.shields.io/badge/License-Creative%20Commons-DC3D24.svg?style=flat-square)](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.zh)



个人兴趣收集的可能用得上的东西；



一些零零碎碎的提示词收集参考：[Prompt.md](./Prompt.md)

## 通用 / 编程 Agent

- [Codex / ChatGPT](https://github.com/openai/codex) — OpenAI 的终端编程 Agent，Rust 实现、Apache-2.0 开源，登录 ChatGPT 账号即可在命令行里读代码、改文件、跑命令和处理 Git 流程。
- [Claude Code](https://github.com/anthropics/claude-code) — Anthropic 的终端编程 Agent，用自然语言理解整个代码库并完成改代码、解释复杂逻辑、走 Git 流程；仓库以文档和问题反馈为主，本体闭源。
- [DSH](https://github.com/deepseek-ai/deepseek-harness) — DeepSeek Harness，官方开源的 Agent 运行框架（MIT），主张「一切皆插件」：模型适配器、工具、会话日志乃至 Agent 主循环都可替换，自带 Web UI，社区大量桌面客户端都基于它封装。
- [Pi Desktop](https://github.com/vastsa/PI-Desktop) — Pi 编程 Agent 的本地优先桌面工作台（Electron + Rust 宿主），把项目、会话、子 Agent、预览拆成各自独立的空间，模型可自带；目前仍是 early preview。
- [Alma](https://github.com/yetone/alma-releases) — 多供应商桌面 AI 客户端（官网 alma.now），一个界面里切换 OpenAI、Anthropic、Gemini、DeepSeek 等，带跨会话记忆、网页搜索、MCP 与插件；仓库只托管发布包。
- [Cindy](https://github.com/makecindy/cindy) — Apache-2.0 的桌面 / 移动 Agent 客户端，把 Claude Code、Codex、Pi 当作底层引擎统一调度，中途换模型不断上下文，记忆与技能跨引擎共用，也能驱动本地浏览器和应用。
- [Cherry Studio](https://github.com/CherryHQ/cherry-studio) — 多模型 AI 桌面工作台，统一接入各厂商 API 与本地模型，内置助手、知识库、MCP 与多助手并行对话。
- [Reasonix](https://github.com/esengine/DeepSeek-Reasonix) — 面向 DeepSeek 的开源终端编程 Agent（MIT，单个 Go 二进制），围绕 prefix-cache 优化长会话成本，适合挂着跑数小时的重构任务，另有桌面端与 VS Code 扩展。
- [WorkBuddy](https://www.workbuddy.cn) — 腾讯出品的 AI 工作台桌面应用（闭源），支持 Skills、MCP、自动化与多智能体协作，可读写本地文件、联网检索并直接产出文档、网页等成品。
- [Qoder](https://qoder.com) — 阿里推出的 Agentic Coding 平台（闭源），覆盖 IDE、CLI、JetBrains 插件和移动端，主打把目标交给智能体自主完成开发任务。





## 辅助工具

- [CloakBrowser](https://github.com/CloakHQ/CloakBrowser) — 从 Chromium 源码层面改指纹逻辑的隐身浏览器（MIT），可直接替换 Playwright，官方称通过 50+ 项机器人检测；反爬严格的站点可以拿它试。
- [StackPrism](https://github.com/setube/stackprism) — 浏览器扩展（Chrome / Edge / Firefox），用静态扫描、响应头、动态资源、JS 版权注释四条通道并行识别网页技术栈，合并去重后按 50+ 类目展示，全程本地运行不上传；注意是 CC BY-NC-SA 协议，仅限非商用。
- [Dokobot](https://dokobot.ai/zh-CN) — 让 Agent 通过你已登录的真实浏览器读页面，按像素级视觉提取而非 DOM，自动滚动续读并输出精简结构化文本（省 token）；本地模式免费无限制，远程连接和并发另收费。
- [Browser Use](https://github.com/browser-use/browser-use) — 用 Python 让 LLM 直接驱动浏览器模拟人操作（底层仍是 Playwright，所以也带着 Playwright 与实际渲染的差异），适合把「查资料、点流程」这类事交给 Agent。
- [ego](https://github.com/citrolabs/ego-lite) — 专为 Agent 定制的浏览器，把你已登录的浏览器状态共享给 Codex、Claude Code 这类 Agent 去自动化操作，互不打扰，零配置。
- [智能体构建指南](https://jimmysong.io/zh/book/ai-handbook/) — Jimmy Song 写的在线手册，按「认知 → 能力 → 交付 → 治理」讲 LLM 生态、提示词工程、RAG、MCP、Agent 运行时和 AI 网关；部分章节仍是草稿，适合先看目录挑着读。
- [agency-agents 中文版](https://github.com/jnMetaCode/agency-agents-zh) — 277 个即插即用的 AI 专家角色定义（含 64 个小红书 / 抖音 / 飞书等中国市场原创），覆盖工程、设计、营销、金融等 20 个部门，角色写不出来时可以抄结构；配 agency-orchestrator 还能让多个角色按 DAG 协作。
- [Langflow](https://github.com/langflow-ai/langflow) — 可视化拖拽搭 Agent 与工作流的开源平台（MIT），带桌面端和 Web 端，适合先跑通流程再决定要不要写代码。
- [Codex Pets](https://codex-pets.net) — 社区桌宠图库，收录大量可下载的 Codex 桌宠；Codex 桌面端的桌宠本身就是任务状态指示器，用动画区分执行中、等你输入、完成待看和卡住四种状态，配合 `hatch-pet` 技能还能用自己的照片生成专属宠物。

## Skill

当然，大概率实际是用不到，这些资源的出现也是因为当前的 AI 还不够聪明，随着大模型的发展，一些很有用的东西肯定会被训练到大模型中，也不再需要外挂来解决。



SKill 是通用的，但是不同的工具配置目录不一致，如果同时使用多个工具，进行统一管理是很有必要的，CC Switch 之类工具已经可以实现类似的功能了，也有一些专门做 Skill 管理的可以看看：[skills-manager](https://github.com/xingkongliang/skills-manager)、SkillsGate。



首先推荐 Anthropic 官方的 [Skills 仓库](https://github.com/anthropics/skills/tree/main/skills)，学习标准 Skill 结构、参考稳定实现、搭建通用工作流的不错选择；最有用的 Skill 大概是让 AI 总结你使用习惯和踩坑经验后总结成的私有 Skill。



- [Humanizer](https://github.com/blader/humanizer) — 去除 AI 写作痕迹的 Agent Skill，基于维基百科「Signs of AI writing」归纳的二十多种模式，把机器味的文字改写成更像人写的表达；支持提供自己的样文来模仿个人文风，也可只处理文件里的正文、不动代码和数据。
- [南鸢写真提示词](https://github.com/nuyoah-ai-works/nuyoah-xiezhen-prompt) — 人像与写真摄影 Agent Skill，提供完整中文 Prompt、系列母版与同系列变体，并支持按原有摄影企划换一位人物重新拍摄分镜。
- [Qwen Image Gen](https://github.com/ZSeven-W/craft-skills/tree/main/skills/qwen-image-gen) — 面向已部署 Qwen-Image 的提示词优化 Skill，覆盖文生图、局部改图、换姿势换场景和画幅选择，并按实际出图结果迭代修正提示词。
- [Awesome Persona Distill Skills](https://github.com/xixu-me/awesome-persona-distill-skills) — 人格蒸馏类 Agent Skills 的收录列表，按自我蒸馏、职场与学术、亲密关系、公众人物方法论、精神性主题分区，每条附一句话说明。
- [Rico Skills](https://github.com/ricocc/rico-skills) — 内容与设计向的 Claude Code skill 组合：把任意网站拆成完整设计系统文档（DESIGN.md / tokens / CSS / Tailwind 主题）或在不同设计格式间互转，也能按 20 套预设主题一键改站点视觉。
- [Matt Pocock Skills](https://github.com/mattpocock/skills) — 面向真实工程而非 vibe coding 的一套小颗粒可组合 skill，用 /grill-me 反复追问把需求问清楚，再用 /tdd、/code-review、/improve-codebase-architecture 管住反馈闭环和代码结构。
- [Archify](https://github.com/tt-a1i/archify) — 把想法、方案或整个代码库画成可交互的独立 HTML 图（工作流、时序、数据流、ERD、时间线等），能点节点看上下游、追指定路径、切主题并导出 PNG/PDF，也能顺着仓库生成带源码定位的架构图。
- [photo-abstract-editorial](https://github.com/ZzzLc0405/photo-abstract-editorial) — 把一张照片做成「原始摄影区域 + 抽象记忆面板 + 诗意英文标题」的竖版编辑作品，抽象形式与配色只从原片提炼，不是滤镜或风格迁移。
- [heytea-style](https://github.com/Hchen1218/heytea-style) — 保留照片里一个真实物件当锚点，配粗黑笨拙的儿童简笔画小人和歪扭手写标题，做成喜茶海报质感的竖版海报，带字版与无字版是两套独立构图。
- [gc-minimal-zine-poster](https://github.com/LiamGvchi/gc-minimal-zine-poster) — 把主题、句子、物件或情绪做成 3:5 做旧纸质的极简 zine 编辑海报，七成以上留白、只留一个视觉主体，同时给出成品图和可复用的提示词。
- [ip-illustration-for-yourself](https://github.com/EverettFish/ip_illustration_for_yourself) — 先用几张参考图立一个「萌粒风」角色锚点，再从它长出文章配图、信息图、贴纸、文件夹图标、信纸、头像和表情包，一整套风格统一的个人 IP 资产。
- [photo-revival](https://github.com/dacnay816y62-hub/photo-revival) — 把随手拍、废片和日常物件重画成 3:4 白纸手绘插画，主体只占一成多、留白八成以上，配一句手写小字，输出的是「一页诗」而不是照片滤镜。
- [tait-crt-interface-skill](https://github.com/TaiT-tt/tait-crt-interface-skill) — 把照片或文字描述做成早期 CRT 计算机界面质感的像素复古插画，多套色卡、悬浮视窗、扫描线和桶形畸变，另带三种风格模板。



其他资源：

- https://colaskill.com/zh/



## 前端

除非是你自己去完整的设计 UI，否则只靠简单描述的话，大概率会生成一堆风格类似的 AI 味很浓的页面。

看了下目前比较火的有 [Taste Skill](https://www.tasteskill.dev/) 这一类减少 AI 设计感的项目。

前端设计方向，A\ 做的还算是不错的，可以参考下它们的 [SKILL](https://github.com/anthropics/skills/tree/main/skills/frontend-design) 是怎么写的。

### 调试

除了数据，另一个目前比较大的问题就是调试，不像后端，前端的调试有很多是样式的问题，并且非常依赖浏览器环境，用自然语言描述的话也很难精确。

[Agentation](https://agentation.com/) 是一款与**Agent 无关**的可视化反馈工具。点击页面上的元素，添加注释，并复制结构化的输出，帮助 AI 编码代理找到您所指的确切代码。



简单说把它引入你的前端项目，给你注入一个调试工具，通过点击选择来精确表达对页面的那个元素有什么要求，之后会生成一份 Agent 看得懂的描述只需要你原样发给 Codex 这类工具就行。



另一种可以通过 Chrome DevTools 的 MCP 协议来让 Agent 了解环境信息，并且 Chrome 也提供了 [chrome-devtools-mcp](https://github.com/ChromeDevTools/chrome-devtools-mcp) 服务来更好的让 Agent 操控浏览器（一般 Slim 模式够用）。



## License

<img src='https://raw.githubusercontent.com/EyreFree/EFArticles/master/res/cc-by-nc-nd.png' width='145.77' height='51'/>

EFArticles 所含文章使用以下协议进行保护：[署名-非商业性使用-禁止演绎](http://creativecommons.org/licenses/by-nc-nd/3.0/cn/)。