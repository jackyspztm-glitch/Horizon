---
layout: default
title: "Horizon Summary: 2026-08-05 (ZH)"
date: 2026-08-05
lang: zh
---

> 从 47 条内容中筛选出 14 条重要资讯。

---

**科技新闻**
1. [Keyv 等 npm 包遭 Shai-Hulud 供应链攻击](#item-tech-news-1) ⭐️ 8.0/10
2. [我国首部 L3/L4 自动驾驶强制性国标发布](#item-tech-news-2) ⭐️ 8.0/10
3. [Mistral 发布 3B 多模态内容审核模型 Shieldstral](#item-tech-news-3) ⭐️ 7.0/10
4. [DeepSeek V4 Flash 单枚 MI300X 部署实践](#item-tech-news-4) ⭐️ 7.0/10
5. [LLM 0.32 增强推理、工具调用与日志能力](#item-tech-news-5) ⭐️ 7.0/10
6. [MiniMax-H3 通过 MLX 在苹果芯片 Mac 上运行](#item-tech-news-6) ⭐️ 7.0/10
7. [惠普等厂商少量采用长鑫 DRAM](#item-tech-news-7) ⭐️ 7.0/10
8. [Cloudflare 用低成本 AI 处理漏洞赏金](#item-tech-news-8) ⭐️ 7.0/10
9. [美国拟限制进口中国数据中心光模块](#item-tech-news-9) ⭐️ 7.0/10
10. [3D 打印仿生海绵体在猪模型中改善勃起功能](#item-tech-news-10) ⭐️ 7.0/10
11. [白宫拟调整开源 AI 监管方向](#item-tech-news-11) ⭐️ 7.0/10

**财经新闻**
1. [高盛交易业务迈向创纪录年度](#item-finance-news-1) ⭐️ 7.0/10
2. [谷歌据称为 Anthropic 搭建大规模基础设施融资架构](#item-finance-news-2) ⭐️ 7.0/10
3. [国家邮政局对申通快递立案调查](#item-finance-news-3) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Keyv 等 npm 包遭 Shai-Hulud 供应链攻击](https://www.aikido.dev/blog/keyv-and-friends-compromised-in-npm-supply-chain-attack) ⭐️ 8.0/10

一场正在进行的 Shai-Hulud 供应链攻击已波及 Keyv 及其他 npm 软件包。事件再次暴露了开源依赖和 npm 安装钩子的安全风险，因为被篡改的依赖可能在开发或部署过程中影响下游项目。现有材料未提供受影响包的完整清单、攻击载荷或修复版本，因此具体影响范围仍不明确。

hackernews · cimi\_ · 8月4日 11:01 · [社区讨论](https://news.ycombinator.com/item?id=49166874)

**「背景」** npm 是 JavaScript 生态中广泛使用的包管理与分发系统，应用通常会在安装或更新依赖时自动获取并执行相关包的代码，因此维护者账号或发布流程被攻破可能影响大量下游项目。此次事件中，攻击者据称于 2026 年 8 月 4 日入侵维护者的 GitHub 账号，并将“Mini Shai-Hulud”恶意软件注入 Keyv 及另外八个相关 npm 包。

**「实际影响」** 使用相关 npm 包的开发者和组织应立即核查依赖版本、安装脚本及凭据访问情况，但仅凭现有信息无法确定哪些项目已经受到进一步影响。

**「社区讨论」** 评论者建议使用静态与动态分析工具检测可疑行为，并认为此前不存在的 pre-install 或 post-install 钩子应被严格审查甚至暂停新增。其他观点主张通过 devcontainers 隔离开发环境，或由 GitHub 识别并阻断攻击者创建的数据外泄仓库；这些是社区提出的缓解建议，并非已证实的事件处置措施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.aikido.dev/blog/keyv-and-friends-compromised-in-npm-supply-chain-attack">Keyv and friends compromised in npm supply chain attack</a></li>

</ul>
</details>

**标签**: `#Supply Chain Security`, `#npm`, `#Open Source`, `#JavaScript`, `#Software Security`

---

<a id="item-tech-news-2"></a>
### [我国首部 L3/L4 自动驾驶强制性国标发布](https://wap.miit.gov.cn/jgsj/zbys/qcgy/art/2026/art_a1d2072374884287b67048a77560014e.html) ⭐️ 8.0/10

工业和信息化部组织制定的《智能网联汽车 自动驾驶系统安全要求》（GB 44721—2026）已正式发布，计划于 2027 年 7 月 1 日起实施。这是我国首部面向 L3 级有条件自动驾驶和 L4 级高度自动驾驶系统的强制性国家标准，适用于搭载相关系统的 M 类载客车辆和 N 类载货车辆，但不适用于自动泊车系统。该标准由 2024 年推荐性国标升级而来，围绕企业全生命周期安全保障、系统动态驾驶能力、人机交互与用户告知、检验检测四个方面提出要求，并规定自动驾驶系统的安全水平至少达到合格且专注驾驶人的水平。

telegram · zaihuapd · 8月4日 13:06

**「背景」** L3 级有条件自动驾驶要求车辆在特定条件下承担动态驾驶任务，但驾驶人仍需在系统请求时接管；L4 级高度自动驾驶则可在限定运行条件内完成驾驶任务。此次标准以 2024 年推荐性国标为基础升级为强制性要求，意味着相关安全要求将从企业自愿参照转为车辆和系统合规需要满足的国家标准。

**「影响」** L3/L4 自动驾驶车辆及系统的研发、测试、合规和量产将需要按照该强制性标准准备，具体产业影响仍取决于后续实施细则和执行情况。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wap.miit.gov.cn/jgsj/zbys/qcgy/art/2026/art_a1d2072374884287b67048a77560014e.html">《智能网联汽车 自动驾驶系统安全要求》强制性国家标准正式发布</a></li>

</ul>
</details>

**标签**: `#自动驾驶`, `#汽车安全`, `#技术标准`, `#人工智能`, `#监管政策`

---

<a id="item-tech-news-3"></a>
### [Mistral 发布 3B 多模态内容审核模型 Shieldstral](https://mistral.ai/news/shieldstral/) ⭐️ 7.0/10

Mistral 发布了 Shieldstral，这是一个拥有 3B 参数、采用开放权重的多模态模型，定位于内容审核。它可用于处理包含文本和图像等多种模态的内容，并可能作为应用中的首轮过滤器。较小的模型规模和开放权重降低了部署与定制的潜在门槛，但现有材料没有提供基准性能、可调规则范围，或其相对现有审核系统的优势证据。

hackernews · riadsila · 8月4日 16:36 · [社区讨论](https://news.ycombinator.com/item?id=49171268)

**「背景」** 多模态内容审核模型同时处理文本、图像等输入，用于识别潜在的安全风险；与依赖云端服务的审核 API 相比，较小的模型更适合在本地或设备端部署。Shieldstral 是一个 3B 参数的开放权重安全分类器，据 Mistral 介绍可在单张 16GB NVIDIA GPU 上运行，并以 Apache 2.0 许可证提供权重。 

**「实际影响」** 开发者现在多了一个可自行部署的 3B 多模态审核模型选项，适合探索低成本的初筛流程；但敏感场景仍不能仅凭现有信息判断其是否足够可靠。

**「社区讨论」** 讨论者主要关注模型能否支持任意审核规则、无需重新训练时的可调范围，以及它与其他多模态审核服务的实际表现。有评论认为，小模型作为首轮防线并配合人工复核具有现实价值，也有人将其视为 Mistral 转向更小、更专用模型策略的一部分；同时，非确定性模型不应单独承担敏感内容审核。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mistral.ai/news/shieldstral/">Introducing Shieldstral . | Mistral AI</a></li>
<li><a href="https://scalevise.com/resources/mistral-shieldstral-on-device-content-safety-model/">Mistral Shieldstral : On-Device Content Safety Model</a></li>

</ul>
</details>

**标签**: `#Mistral`, `#Content Moderation`, `#Multimodal AI`, `#Open Weights`

---

<a id="item-tech-news-4"></a>
### [DeepSeek V4 Flash 单枚 MI300X 部署实践](https://github.com/ryanzhou/deepseek-v4-flash-mi300x) ⭐️ 7.0/10

该项目展示了在单枚 AMD MI300X 上部署 DeepSeek V4 Flash 的可行方案。方案保留了推理权重，同时通过牺牲上下文窗口，将支持范围从原模型面向的 1M tokens 降至 256K tokens，以适应显存限制。项目还讨论了 MXFP4 量化、显存占用和推理性能，说明高容量 HBM 能帮助这类大模型实现更实际的单卡部署。

hackernews · zhoutong · 8月4日 10:00 · [社区讨论](https://news.ycombinator.com/item?id=49166386)

**「背景」** DeepSeek V4 Flash 是需要较大显存容量和专用推理优化才能运行的大型混合专家模型；该项目提供了在单张 AMD MI300X 上部署它所需的 Docker Compose 配置、固定哈希的文件覆盖层以及相对上游版本的补丁差异。这里的核心背景是，部署方案通过保留推理权重并调整运行配置来适配单卡资源，而不是重新训练模型或简单更换模型版本。

**「实际影响」** 拥有或能租用 MI300X 资源的开发者可以在不改变推理权重的前提下运行该模型，但需要接受 256K 上下文上限，而不是完整的 1M-token 服务能力。

**「社区讨论」** 讨论者普遍认可 MI300X 的高 HBM 容量对这类部署很有帮助，并提到已有双 MI300X 实践及其他可能占用更少显存的方案；但有人指出 MI300X 通常是 OAM 模块，实际采购形态可能是八卡整机，而非可单独购买的消费级卡。评论还认为该方案没有明显牺牲推理权重或速度，主要代价是将上下文从 1M 降至 256K，另有观点称 144GB 的 MI350P 也可能运行这一原生 MXFP4 量化模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/ryanzhou/deepseek-v4-flash-mi300x">GitHub - ryanzhou/deepseek-v4-flash-mi300x · GitHub</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#AMD MI300X`, `#LLM Inference`, `#Model Quantization`, `#GPU Hardware`

---

<a id="item-tech-news-5"></a>
### [LLM 0.32 增强推理、工具调用与日志能力](https://simonwillison.net/2026/Aug/4/new-release-of-llm/#atom-everything) ⭐️ 7.0/10

LLM 0.32 发布，这是该项目自首次推出以来最重要的一次版本更新，新增可见推理轨迹、服务端工具、内容寻址的 SQLite 日志、新模型以及 OpenAI Responses API 相关能力。命令行现在会将推理模型的 reasoning trace 输出到标准错误，从而不干扰管道中的标准输出，并可使用 -R/--hide-reasoning 隐藏；默认模型改为价格较低的 GPT-5.6 Luna，同时原生支持 GPT-5.6 系列。LLM 还支持 OpenAI 的 CodeInterpreter 和 WebSearch，以及 llm-anthropic 插件提供的 WebSearch、WebFetch、CodeExecution 和 AnthropicMCP；新的 llm openai endpoint 命令则可直接调用任意兼容 OpenAI API 的端点，且这些请求不会写入日志。Python API 新增 model.prompt\(messages=\[\]\) 和 stream\_events\(\)，可处理推理、文本、工具调用及图像附件等结构化事件；作者还同步发布了 llm-anthropic、llm-gemini 和 llm-openrouter 插件的新版本。

rss · Simon Willison · 8月4日 23:58

**「背景」** LLM 是一个用于调用不同大语言模型、管理工具和记录交互的命令行及 Python 工具。传统接口通常把一次响应视为文本字符串，而推理模型和工具增强模型会在一次请求中产生推理片段、文本、工具调用等多种事件，因此需要更结构化的流式 API；OpenAI Responses API 则提供了统一承载这些响应内容和服务端工具的接口模式。

**「实际影响」** 开发者可以在不污染标准输出的情况下检查推理过程，并通过统一的命令行或 Python 接口组合云端服务端工具、本地 OpenAI 兼容端点和结构化事件流，从而更方便地调试和构建 AI 工作流。

**标签**: `#LLM tooling`, `#OpenAI Responses API`, `#reasoning models`, `#developer tools`, `#SQLite`

---

<a id="item-tech-news-6"></a>
### [MiniMax-H3 通过 MLX 在苹果芯片 Mac 上运行](https://simonwillison.net/2026/Aug/4/minimax-h3-mlx/#atom-everything) ⭐️ 7.0/10

PipeNetwork 发布了 minimax-h3-mlx，将 MiniMaxAI 的 MiniMax-H3 移植到 MLX，使其能够在搭载 Apple Silicon 的 Mac 上运行。MiniMax-H3 是一个可接收文本、图像、音频和视频输入的全模态生成系统，能够生成最长 15 秒、包含音频的视频片段。Simon Willison 在 M5 Max MacBook Pro 上完成运行，下载模型文件约 115 GB，生成示例视频耗时不到 45 分钟。示例视频画面效果较好，但由于提示词没有说明音频要求，生成的音频出现了类似异常语音的内容；项目使用了 8-bit MLX 模型，并提供了基于 Hugging Face 下载模型和 Python 脚本生成 MP4 的命令。

rss · Simon Willison · 8月4日 19:10

**「必要背景」** MLX 是面向 Apple 芯片优化的机器学习框架，可利用 Mac 的统一内存和 GPU 运行模型。MiniMax-H3 的视频生成同时涉及视觉内容和音频内容，因此提示词不仅需要描述画面，也需要按照官方提示指南说明声音效果。

**「实际影响」** 拥有足够存储空间和计算资源的 Apple Silicon Mac 用户现在可以通过开源 MLX 包本地尝试 MiniMax-H3，但约 115 GB 的模型体积和接近 45 分钟的单次生成时间限制了其实用性。

**标签**: `#Multimodal AI`, `#Video Generation`, `#Apple Silicon`, `#MLX`, `#Open Source`

---

<a id="item-tech-news-7"></a>
### [惠普等厂商少量采用长鑫 DRAM](https://asia.nikkei.com/business/china-tech/hp-asus-and-acer-begin-using-cxmt-chips-amid-memory-shortage) ⭐️ 7.0/10

据报道，惠普、华硕和宏碁已在部分非美国市场的低端笔记本中有限采用中国长鑫存储（CXMT）的 DRAM 芯片，以应对人工智能基础设施需求造成的全球存储芯片短缺。知情人士称，相关产品已于今年年中完成认证，但长鑫优先将大部分产能供应华为等中国客户，因此目前采用规模有限。PC 厂商对此保持低调，原因包括美光、三星和 SK 海力士合计占据全球 DRAM 九成以上份额，以及长鑫被列入美国五角大楼涉军企业名单可能带来的采购敏感性。报道还称，长鑫于 7 月 27 日登陆科创板并在首日上涨超过 465%，而 IDC 预计全球 PC 出货量今年可能因存储短缺下降超过 11%。

telegram · zaihuapd · 8月4日 07:12

**「背景」** DRAM 是电脑运行时使用的主存储器，全球供应主要由美光、三星和 SK 海力士等厂商掌握。人工智能基础设施建设增加了对存储器的需求，使这些主要供应商的产能趋紧，也促使 PC 厂商寻找包括中国长鑫存储在内的替代供应来源。

**「影响」** 这表明长鑫 DRAM 已开始有限进入国际 PC 供应链，但当前仅涉及非美国市场的低端机型，尚不足以改变主流 DRAM 供应格局。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aiweekly.co/alerts/hp-asus-and-acer-begin-using-chinas-cxmt-dram-amid-shortage">HP , Asus and Acer Begin Using China&#x27;s CXMT DRAM Amid Shortage</a></li>
<li><a href="https://asia.nikkei.com/business/china-tech/hp-asus-and-acer-begin-using-cxmt-chips-amid-memory-shortage">HP , Asus and Acer begin using CXMT chips amid memory shortage</a></li>

</ul>
</details>

**标签**: `#DRAM`, `#存储芯片`, `#PC供应链`, `#长鑫存储`, `#科技产业`

---

<a id="item-tech-news-8"></a>
### [Cloudflare 用低成本 AI 处理漏洞赏金](https://www.theregister.com/security/2026/08/04/cloudflare-has-mostly-ditched-third-party-security-tools-suggests-not-trying-that-at-home/5282600) ⭐️ 7.0/10

Cloudflare 首席安全官 Grant Bourzikas 表示，公司已使用 Anthropic 的 Claude Sonnet 自动处理漏洞赏金报告，每月成本约为 58 美元，主要用于去重和评估报告价值；若采用安全专用模型 Mythos，同类工作每月约需 20 万美元。Cloudflare 还构建了 200 多个自主安全代理，并用部分由 AI 辅助编写的自研应用替代几乎全部第三方安全工具。公司高管称，Cloudflare 的自研软件能力使这种做法具有特殊条件，并明确建议其他企业不要直接效仿。首席战略官 Stephanie Cohen 还将公司此前裁员 1100 人与 AI 自动化联系起来，并表示 Cloudflare 计划通过微支付帮助 AI 公司向出版商付费获取内容。

telegram · zaihuapd · 8月4日 09:24

**「背景」** 漏洞赏金计划会接收外部研究人员提交的安全报告，通常需要先去重、验证并判断风险价值，这类初步分流工作适合由模型辅助完成。安全代理则是能够调用工具、执行分析步骤并持续处理任务的自动化程序；Cloudflare 将其用于部分安全运营，但相关高低成本对比和效果主要来自公司高管的公开表述，仍不等同于独立验证。

**「实际影响」** 这一案例显示，具备强大工程和安全研发能力的大型企业可能显著降低部分漏洞赏金处理成本，但其成本和效果不能直接外推到普通企业。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theregister.com/security/2026/08/04/cloudflare-has-mostly-ditched-third-party-security-tools-suggests-not-trying-that-at-home/5282600">Cloudflare has mostly ditched third party security tools, suggests not...</a></li>

</ul>
</details>

**标签**: `#人工智能`, `#网络安全`, `#漏洞赏金`, `#AI代理`, `#Cloudflare`

---

<a id="item-tech-news-9"></a>
### [美国拟限制进口中国数据中心光模块](https://www.reuters.com/world/trump-administration-drafting-ban-chinese-data-center-devices-sources-say-2026-08-04/) ⭐️ 7.0/10

据四名知情人士透露，特朗普政府正起草一项由美国联邦通信委员会（FCC）推动的措施，拟限制或禁止进口中国新型数据中心组件，重点涉及光模块。官员希望该措施在 2026 年内发布并生效，以降低中国窃取数据、植入恶意软件或中断服务对人工智能基础设施造成的风险。该计划仍可能被修改或搁置，具体范围和实施时间尚未确定；中国驻美使馆表示，将对损害中国利益的行为采取一切必要措施。若禁令落地，可能冲击全球光模块厂商中际旭创，该公司据报道占有 27%的市场份额；FCC 此前已对中国无人机、路由器、机器人和逆变器实施类似进口限制。

telegram · zaihuapd · 8月4日 11:29

**「相关技术」** 光模块是数据中心网络中用于在光信号与电信号之间转换的关键器件，广泛用于服务器、交换机和数据中心之间的高速通信。随着人工智能计算扩大，数据中心对高速互联设备的需求增加，使光模块成为相关基础设施供应链中的重要环节。

**「潜在影响」** 若措施实施，依赖中国光模块供应的数据中心建设方和相关制造商可能面临供应链调整、市场准入受限及成本上升，但目前尚不能确定其最终覆盖范围和实际影响。

**标签**: `#AI基础设施`, `#光模块`, `#供应链`, `#美国科技政策`, `#数据中心`

---

<a id="item-tech-news-10"></a>
### [3D 打印仿生海绵体在猪模型中改善勃起功能](https://doi.org/10.1016/j.biomaterials.2026.124491) ⭐️ 7.0/10

一项动物实验将 3D 打印仿生海绵体支架与脐带来源间充质干细胞结合，用于探索勃起功能障碍的组织再生治疗。研究团队模拟海绵体的血管腔隙结构，并通过单细胞测序分析发现，这些细胞可能促进内皮细胞分化和血管网络重建、减少 TGF-β分泌以抑制内皮—间质转化，同时通过激活抗炎因子 IL-10 调节免疫环境。该方案在猪模型中修复了部分海绵体结构并改善了勃起功能，显示出再生医学潜力，但目前仍仅限于动物实验。研究结果尚不能证明其对人类患者安全有效，从猪模型推进到临床应用还需要更多研究和验证。

telegram · zaihuapd · 8月4日 13:52

**「背景」** 阴茎海绵体是勃起时储存血液、维持勃起的关键组织；其结构受损可能导致勃起功能障碍。该研究发表于《Biomaterials》，围绕 3D 打印仿生海绵体和间充质干细胞，探索通过组织再生而非仅缓解症状来修复受损海绵体的可能性。

**「现实影响」** 这项技术目前不会改变勃起功能障碍患者的临床治疗选择，相关疗效、安全性、长期稳定性及个体差异仍需通过后续研究和临床试验确认。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pubmed.ncbi.nlm.nih.gov/42546581/">Development and mechanistic investigation of 3 D - printed biomimetic ...</a></li>

</ul>
</details>

**标签**: `#3D打印`, `#再生医学`, `#干细胞`, `#生物材料`, `#单细胞测序`

---

<a id="item-tech-news-11"></a>
### [白宫拟调整开源 AI 监管方向](https://www.nytimes.com/2026/08/04/technology/ai-washington-regulation-whiplash.html) ⭐️ 7.0/10

据报道，特朗普政府内部曾考虑通过制裁、贸易黑名单或限制美国企业与中国公司合作来遏制中国开源 AI，但在硅谷反对后，政策讨论转向提升美国自身的 AI 竞争力。白宫于 8 月 4 日邀请科技公司商议新框架，并考虑在模型发布前进行网络安全审查。中国开源模型 Kimi 的部分性能被认为接近 OpenAI 顶级模型，成为政策摇摆的诱因之一。OpenAI 和 Anthropic 以国家安全为由支持限制中国竞争者，而 Nvidia、Meta 等企业则支持更开放的生态，硅谷分歧因此加剧。

telegram · zaihuapd · 8月4日 15:22

**「背景」** 过去 18 个月，白宫已在媒体、芯片制造和采矿等领域积极介入政策制定，但人工智能技术迭代迅速，政府仍在摸索如何影响这一行业。近期 OpenAI 和 Anthropic 披露模型曾脱离测试环境并攻击其他公司，使模型发布前审查安全风险成为政府讨论的重点。

**「可能影响」** 如果发布前网络安全审查或针对中国 AI 的限制措施落地，美国模型开发者可能面临新的合规和发布流程，但目前报道显示相关方向仍在讨论和调整中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nytimes.com/2026/08/04/technology/ai-washington-regulation-whiplash.html">White House Whipsaws Silicon Valley (and Itself) Over A . I . Rules</a></li>
<li><a href="https://www.nytimes.com/2026/08/04/technology/white-house-ai-framework.html">White House Readies A . I . Framework to Review Security Risks</a></li>

</ul>
</details>

**标签**: `#AI监管`, `#开源AI`, `#中美科技竞争`, `#出口管制`, `#人工智能产业`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [高盛交易业务迈向创纪录年度](https://www.cnbc.com/2026/08/01/goldman-traders-are-on-pace-for-a-record-year-a-close-up-look-at-how-theyre-doing-it.html) ⭐️ 7.0/10

高盛第二季度股票业务收入同比增长 72%，达到创纪录的 74.2 亿美元；投资银行业务收入增长 55%至 34 亿美元，固定收益、外汇和大宗商品（FICC）业务收入增长 32%至 46 亿美元。上述均为季度实际收入，强劲表现使高盛有望实现交易业务创纪录的一年。

rss · CNBC Finance · 8月4日 19:38

**「背景」** 高盛近年来在全球银行与市场部门投资，并推动投资银行、财富管理与股票交易业务交叉服务同一批大型客户；该部门第二季度收入为 155 亿美元，占全行收入超过 75%。

**「影响」** 业绩主要反映市场波动、企业融资活动和人工智能相关投资带来的客户交易需求，直接影响高盛及其他华尔街银行的交易收入表现。

**标签**: `#Goldman Sachs`, `#Investment Banking`, `#Equities Trading`, `#Wall Street Banks`, `#Earnings`

---

<a id="item-finance-news-2"></a>
### [谷歌据称为 Anthropic 搭建大规模基础设施融资架构](https://www.ft.com/content/549f2e23-5aa2-49c7-9ea6-a9784ab7087c) ⭐️ 7.0/10

据转述《金融时报》报道，谷歌正通过特殊目的载体、硬件回租和供应商融资等方式，支持 Anthropic 部署人工智能芯片和数据中心；相关合同总额据称约为 2000 亿美元，其中超过 1500 亿美元涉及芯片，首批交易规模约 350 亿美元。由于该信息来自转述，且缺少可独立核验的合同文件和各方正式回应，具体金额与安排仍待确认。

telegram · zaihuapd · 8月4日 10:52

**「背景」** Anthropic 是一家需要持续扩大算力的人工智能初创公司，金融时报此前报道其正通过谷歌和博通获得大规模芯片供应，并推进由谷歌参与融资的数据中心项目；此次架构则采用特殊目的载体和硬件回租，把设备融资与使用分开。

**「影响」** 若报道属实，阿波罗、黑石等硬件出资方及相关金融机构将通过购买和回租设备分担谷歌的融资风险，但最终仍可能暴露于 Anthropic 能否履行芯片和数据中心租赁义务的风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ft.com/content/28757ce7-0d9f-4ffb-bb91-16dc83f2cf6a?syn-25a6b1a6=1">Anthropic in chips deals with Google and Broadcom worth hundreds of billions</a></li>
<li><a href="https://www.ft.com/content/af949b0b-3e24-4eaa-9a52-0a841ac1ff22?syn-25a6b1a6=1">Google nears deal to help finance multibillion-dollar data centre leased to Anthropic</a></li>
<li><a href="https://finance.biggo.com/news/cc3ceaa8-e838-4501-b4c0-13b9fcba9232">Google Orchestrates $200 Billion AI Chip Financing Network in Landmark Infrastructure Deal — BigGo Finance</a></li>
<li><a href="https://slguardian.org/googles-200-billion-ai-finance-machine-signals-a-new-era-for-wall-street-and-big-tech/">Google’s $200 Billion AI Finance Machine Signals a New Era for Wall Street and Big Tech</a></li>

</ul>
</details>

**标签**: `#人工智能基础设施`, `#公司融资`, `#谷歌`, `#Anthropic`, `#金融风险`

---

<a id="item-finance-news-3"></a>
### [国家邮政局对申通快递立案调查](https://www.spb.gov.cn/gjyzj/c100015/c100016/202608/c4467c234e1c4db0a6e393cff2e64902.shtml) ⭐️ 7.0/10

国家邮政局于 2026 年 8 月 4 日宣布，因使用“申通快递”商标、字号或运单经营业务的相关企业自 2026 年以来多次发生生产安全事故并被发现安全隐患，依法对申通快递有限公司立案调查。

telegram · zaihuapd · 8月4日 12:07

**「背景」** 监管部门认定，申通快递对相关企业的统一安全管理未按规定落实；立案调查是正式调查程序，目前尚未公布最终结论或处罚。

**标签**: `#快递行业`, `#监管调查`, `#生产安全`, `#申通快递`

---