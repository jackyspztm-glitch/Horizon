---
layout: default
title: "Horizon Summary: 2026-08-05 (EN)"
date: 2026-08-05
lang: en
---

> From 47 items, 14 important content pieces were selected

---

**Technology News**
1. [Shai-Hulud Compromises Keyv and Other npm Packages](#item-tech-news-1) ⭐️ 8.0/10
2. [China Publishes Mandatory L3/L4 Autonomous Driving Safety Standard](#item-tech-news-2) ⭐️ 8.0/10
3. [Mistral Releases Shieldstral, a 3B Open-Weights Moderation Model](#item-tech-news-3) ⭐️ 7.0/10
4. [DeepSeek V4 Flash on One AMD MI300X](#item-tech-news-4) ⭐️ 7.0/10
5. [LLM 0.32 adds reasoning traces and provider tools](#item-tech-news-5) ⭐️ 7.0/10
6. [MiniMax-H3 Video Generation Comes to Apple Silicon](#item-tech-news-6) ⭐️ 7.0/10
7. [HP, Asus and Acer Reportedly Adopt CXMT DRAM in Limited Markets](#item-tech-news-7) ⭐️ 7.0/10
8. [Cloudflare Uses Low-Cost AI for Vulnerability Triage](#item-tech-news-8) ⭐️ 7.0/10
9. [U.S. Considers Ban on New Chinese Data-Center Optical Modules](#item-tech-news-9) ⭐️ 7.0/10
10. [3D-Printed Biomimetic Tissue Shows Potential for Erectile Dysfunction Repair](#item-tech-news-10) ⭐️ 7.0/10
11. [White House Weighs Shift on Open-Source AI Regulation](#item-tech-news-11) ⭐️ 7.0/10

**Financial News**
1. [Goldman Sachs trading revenue surges](#item-finance-news-1) ⭐️ 7.0/10
2. [Google Reportedly Builds Financing Structure for Anthropic](#item-finance-news-2) ⭐️ 7.0/10
3. [China Opens Investigation Into STO Express](#item-finance-news-3) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Shai-Hulud Compromises Keyv and Other npm Packages](https://www.aikido.dev/blog/keyv-and-friends-compromised-in-npm-supply-chain-attack) ⭐️ 8.0/10

An active Shai-Hulud supply-chain attack has compromised Keyv and other npm packages, raising concerns for developers and applications that depend on them. The incident highlights how malicious package changes and installation hooks can turn widely used dependencies into a distribution channel for attacks. The supplied report does not identify the affected package versions or provide detailed technical indicators, so the full scope and remediation requirements remain unclear.

hackernews · cimi\_ · Aug 4, 11:01 · [Discussion](https://news.ycombinator.com/item?id=49166874)

**「Background」** npm packages are commonly installed as dependencies, and their lifecycle scripts can execute during installation, giving compromised packages a path to affect developer environments and downstream applications. The reported incident involved malware injected into Keyv and eight related packages on August 4, 2026, after an attacker compromised the maintainer’s GitHub account.【tool-1-1】

**「Practical consequence」** Developers using Keyv or related npm dependencies should audit their dependency trees and installation scripts for unexpected changes before installing or updating packages.

**「Community response」** Commenters broadly focused on stronger supply-chain defenses, including static and behavioral package scanning, suspicion of newly introduced pre-install or post-install hooks, and use of devcontainers to limit the impact of compromised dependencies. They also expressed concern about npm’s dependency model and suggested that GitHub should detect and block repositories used to exfiltrate stolen data.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aikido.dev/blog/keyv-and-friends-compromised-in-npm-supply-chain-attack">Keyv and friends compromised in npm supply chain attack</a></li>

</ul>
</details>

**Tags**: `#Supply Chain Security`, `#npm`, `#Open Source`, `#JavaScript`, `#Software Security`

---

<a id="item-tech-news-2"></a>
### [China Publishes Mandatory L3/L4 Autonomous Driving Safety Standard](https://wap.miit.gov.cn/jgsj/zbys/qcgy/art/2026/art_a1d2072374884287b67048a77560014e.html) ⭐️ 8.0/10

China’s Ministry of Industry and Information Technology has approved and published GB 44721—2026, the country’s first mandatory national standard specifically covering Level 3 conditional and Level 4 highly automated driving systems. The standard is scheduled to take effect on July 1, 2027, and applies to passenger-carrying M-category and goods-carrying N-category vehicles, but not automated parking systems. It upgrades the 2024 recommended standard into a mandatory framework covering full-lifecycle safety, dynamic driving capability, human-machine interaction and user notices, and inspection and testing. The requirements specify that automated driving systems must achieve a safety level at least equivalent to that of a qualified and attentive driver.

telegram · zaihuapd · Aug 4, 13:06

**「Background」** In China’s vehicle-automation classification, L3 denotes conditional automation that still involves a human fallback driver, while L4 denotes high automation within defined operating conditions. GB 44721—2026 builds on the 2024 recommended national standard but makes the safety requirements mandatory, covering vehicle life-cycle safeguards, the system’s dynamic driving capability, human-machine interaction, user notifications, and testing; it excludes automated parking systems.【tool-1-1】

**「Practical effect」** Developers and manufacturers of affected L3/L4 vehicles will need to align system development, testing, user communication, and safety processes with the mandatory requirements by the implementation date, while the exact industry impact will depend on subsequent implementation details and enforcement.

<details><summary>References</summary>
<ul>
<li><a href="https://wap.miit.gov.cn/jgsj/zbys/qcgy/art/2026/art_a1d2072374884287b67048a77560014e.html">《智能网联汽车 自动驾驶系统安全要求》强制性国家标准正式发布</a></li>

</ul>
</details>

**Tags**: `#自动驾驶`, `#汽车安全`, `#技术标准`, `#人工智能`, `#监管政策`

---

<a id="item-tech-news-3"></a>
### [Mistral Releases Shieldstral, a 3B Open-Weights Moderation Model](https://mistral.ai/news/shieldstral/) ⭐️ 7.0/10

Mistral has released Shieldstral, a 3B-parameter open-weights multimodal model designed for content moderation. Its relatively small size could make it practical as a lower-cost first-pass filter for applications that process text and images. The supplied material does not establish its benchmark performance, supported customization range, or superiority over existing moderation systems.

hackernews · riadsila · Aug 4, 16:36 · [Discussion](https://news.ycombinator.com/item?id=49171268)

**「Background」** A multimodal safety classifier evaluates more than text alone, such as images and their accompanying text, to identify content that may violate a moderation policy. “Open weights” means the model parameters are available for organizations to run and integrate themselves; Mistral describes Shieldstral as a 3B-parameter classifier, with reporting indicating support for on-device deployment and an Apache 2.0 license.【tool-1-1】【tool-1-3】

**「Practical consequence」** Developers building social, image-sharing, or other user-content applications may have a more accessible candidate for initial moderation, although sensitive decisions would still require validation and potentially human review.

**「Community response」** Commenters viewed the smaller, specialized model as a potentially cost-effective first defense, while questioning whether its moderation policies can be tuned to arbitrary rulesets without retraining. Others asked how it compares with hosted moderation APIs and noted that nondeterministic moderation should not be relied on alone for sensitive decisions.

<details><summary>References</summary>
<ul>
<li><a href="https://mistral.ai/news/shieldstral/">Introducing Shieldstral . | Mistral AI</a></li>
<li><a href="https://scalevise.com/resources/mistral-shieldstral-on-device-content-safety-model/">Mistral Shieldstral : On-Device Content Safety Model</a></li>

</ul>
</details>

**Tags**: `#Mistral`, `#Content Moderation`, `#Multimodal AI`, `#Open Weights`

---

<a id="item-tech-news-4"></a>
### [DeepSeek V4 Flash on One AMD MI300X](https://github.com/ryanzhou/deepseek-v4-flash-mi300x) ⭐️ 7.0/10

A project demonstrates running DeepSeek V4 Flash on a single AMD MI300X by addressing its memory requirements and using native MXFP4 quantization. The deployment preserves the model’s intended inference weights rather than relying on a more aggressive quality-reducing quantization scheme. Its main compromise is reducing the supported context window from the model’s 1 million tokens to 256,000 tokens, while the report discusses practical inference performance and memory constraints. This makes the work a systems-oriented example of trading context capacity for simpler single-accelerator deployment.

hackernews · zhoutong · Aug 4, 10:00 · [Discussion](https://news.ycombinator.com/item?id=49166386)

**「Background」** DeepSeek-V4-Flash is a large model whose inference deployment depends heavily on accelerator memory capacity and software support. This repository documents the Docker configuration and patches needed to run the 0731 model on one AMD MI300X, including pinned file overlays and differences from upstream implementations.

**「Practical consequence」** Operators with access to a sufficiently large-memory MI300X can run the model with its inference weights intact, provided that a 256K-token context limit is acceptable.

**「Community discussion」**  commenters viewed the result as a useful demonstration of the MI300X’s high HBM capacity, cited related two-MI300X and DwarfStar implementations, and noted that the MI300X is an OAM module generally encountered in multi-GPU systems rather than as a typical standalone retail card. Discussion also emphasized that the principal compromise is the 256K context window instead of 1M; one commenter considered this practical, while others questioned hardware choices and implementation comparisons.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/ryanzhou/deepseek-v4-flash-mi300x">GitHub - ryanzhou/deepseek-v4-flash-mi300x · GitHub</a></li>

</ul>
</details>

**Tags**: `#DeepSeek`, `#AMD MI300X`, `#LLM Inference`, `#Model Quantization`, `#GPU Hardware`

---

<a id="item-tech-news-5"></a>
### [LLM 0.32 adds reasoning traces and provider tools](https://simonwillison.net/2026/Aug/4/new-release-of-llm/#atom-everything) ⭐️ 7.0/10

LLM 0.32, described by Simon Willison as the project&\#x27;s most significant release since launch, adds visible reasoning traces, server-side provider tools, redesigned content-addressable SQLite logs, new models, and OpenAI Responses API features. Reasoning output is displayed on standard error by default, while \`-R/--hide-reasoning\` suppresses it; the release also adds GPT-5.6 family support and makes GPT-5.6 Luna the default model for prompt commands. CLI users can invoke OpenAI&\#x27;s CodeInterpreter and WebSearch, Anthropic&\#x27;s WebSearch, WebFetch, CodeExecution, and AnthropicMCP tools, or send unlogged prompts to any OpenAI-compatible endpoint with \`llm openai endpoint\`. The Python API now accepts complete message lists and exposes structured streaming events for reasoning, text, tool calls, and other response content, alongside substantial updates to the \`llm-anthropic\`, \`llm-gemini\`, and \`llm-openrouter\` plugins.

rss · Simon Willison · Aug 4, 23:58

**「Why these features matter」** Reasoning models can emit intermediate reasoning alongside their final answers, while modern model APIs may also return tool calls, attachments, and other structured events rather than a single text string. Server-side tools run in a provider&\#x27;s environment, and OpenAI-compatible endpoints allow the same client pattern to be used with local or third-party models such as those exposed by LM Studio.

**「Practical impact」** Developers can inspect reasoning separately from piped output, connect provider-hosted tools and MCP services from the CLI, and build Python integrations that handle richer streamed model responses without relying on a conversation-only abstraction.

**Tags**: `#LLM tooling`, `#OpenAI Responses API`, `#reasoning models`, `#developer tools`, `#SQLite`

---

<a id="item-tech-news-6"></a>
### [MiniMax-H3 Video Generation Comes to Apple Silicon](https://simonwillison.net/2026/Aug/4/minimax-h3-mlx/#atom-everything) ⭐️ 7.0/10

PipeNetwork’s open-source \`minimax-h3-mlx\` package ports MiniMax-H3 to Apple’s MLX framework, enabling the multimodal system to run on Apple Silicon Macs. MiniMax-H3 accepts text, images, audio, and video, and can generate video clips of up to 15 seconds with accompanying audio. Simon Willison ran the MLX port on an M5 Max MacBook Pro after downloading about 115 GB of model files; generation took just under 45 minutes for a sample prompt. The resulting video was impressive, but its audio was speech-like garbage because the prompt did not specify the desired audio, a limitation addressed by MiniMax’s separate video-prompting guide.

rss · Simon Willison · Aug 4, 19:10

**「Context」** MLX is Apple’s machine-learning framework for efficiently running models on Apple Silicon hardware. The package uses the MiniMax-H3 model together with an 8-bit MLX model download and provides a Python script for generating an MP4 from a text prompt.

**「Practical consequence」** Apple Silicon users can experiment with local MiniMax-H3 video-and-audio generation, but the roughly 115 GB download and nearly 45-minute sample runtime make it resource-intensive.

**Tags**: `#Multimodal AI`, `#Video Generation`, `#Apple Silicon`, `#MLX`, `#Open Source`

---

<a id="item-tech-news-7"></a>
### [HP, Asus and Acer Reportedly Adopt CXMT DRAM in Limited Markets](https://asia.nikkei.com/business/china-tech/hp-asus-and-acer-begin-using-cxmt-chips-amid-memory-shortage) ⭐️ 7.0/10

HP, Asus and Acer have reportedly begun using DRAM chips from China’s ChangXin Memory Technologies \(CXMT\) in limited quantities for low-end laptops sold outside the United States. Sources cited by Nikkei Asia said the manufacturers completed qualification around midyear, while CXMT is allocating most of its capacity to Chinese customers including Huawei. The reported adoption comes as demand from AI infrastructure contributes to a severe memory-chip shortage, but the PC makers are keeping the move low-profile because Micron, Samsung and SK Hynix together control more than 90% of the global market and CXMT’s listing on a U.S. Department of Defense-related blacklist makes procurement politically sensitive. IDC estimates that global PC shipments could fall by more than 11% this year because of the memory shortage.

telegram · zaihuapd · Aug 4, 07:12

**「Background」** DRAM is the volatile memory used by PCs and servers, and demand from AI infrastructure has tightened supply from the dominant suppliers Micron, Samsung, and SK Hynix. ChangXin Memory Technologies \(CXMT\) is a Chinese DRAM manufacturer whose reported inclusion on a U.S. Department of Defense list of Chinese military-linked companies adds regulatory and geopolitical sensitivity to procurement by U.S.-linked businesses.

**「Practical impact」** CXMT is gaining a limited foothold in major PC manufacturers’ supply chains, but constrained capacity, market segmentation and U.S. sensitivities currently prevent its DRAM from serving as a broad replacement for leading suppliers.

<details><summary>References</summary>
<ul>
<li><a href="https://aiweekly.co/alerts/hp-asus-and-acer-begin-using-chinas-cxmt-dram-amid-shortage">HP , Asus and Acer Begin Using China&#x27;s CXMT DRAM Amid Shortage</a></li>
<li><a href="https://wesearch.press/s/three-major-pc-makers-now-using-chinese-memory-to-fight-unpr-4903d582">Three major PC makers now using Chinese memory to fight...</a></li>

</ul>
</details>

**Tags**: `#DRAM`, `#存储芯片`, `#PC供应链`, `#长鑫存储`, `#科技产业`

---

<a id="item-tech-news-8"></a>
### [Cloudflare Uses Low-Cost AI for Vulnerability Triage](https://www.theregister.com/security/2026/08/04/cloudflare-has-mostly-ditched-third-party-security-tools-suggests-not-trying-that-at-home/5282600) ⭐️ 7.0/10

Cloudflare Chief Security Officer Grant Bourzikas said the company uses Anthropic’s Claude Sonnet to automate deduplication and value assessment for bug-bounty reports at a reported cost of about $58 per month. He said the same work would cost roughly $200,000 per month with the security-focused Mythos model. Cloudflare has also built more than 200 autonomous security agents and has largely replaced third-party security tools with internally developed applications, some assisted by AI. Bourzikas cautioned that other companies should not simply copy this approach because Cloudflare has the engineering capacity to build its own security software, while Chief Strategy Officer Stephanie Cohen linked the company’s reduction of 1,100 positions to AI-driven automation and described plans to connect AI companies with publishers through micropayments for content access.

telegram · zaihuapd · Aug 4, 09:24

**「Background」** Bug-bounty triage is the process of removing duplicate vulnerability reports and assessing which findings merit investigation, traditionally supported by security platforms and human analysts. Cloudflare’s example illustrates a model-selection trade-off: a general-purpose model can handle a narrow, repetitive task at far lower cost than a security-focused model, while autonomous security agents extend AI assistance into broader internal workflows. \[tool-1-1\]\[tool-1-2\]

**「Why it matters」** The claims suggest that a large security organization can sharply reduce the operating cost of routine vulnerability triage, but the approach depends on substantial internal engineering capability and has not been independently validated in the supplied account.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theregister.com/security/2026/08/04/cloudflare-has-mostly-ditched-third-party-security-tools-suggests-not-trying-that-at-home/5282600">Cloudflare has mostly ditched third party security tools, suggests not...</a></li>
<li><a href="https://news.lavx.hu/article/cloudflare-cuts-most-third-party-security-tools-warns-others-against-copying-it">Cloudflare cuts most third-party security tools, warns... | LavX News</a></li>

</ul>
</details>

**Tags**: `#人工智能`, `#网络安全`, `#漏洞赏金`, `#AI代理`, `#Cloudflare`

---

<a id="item-tech-news-9"></a>
### [U.S. Considers Ban on New Chinese Data-Center Optical Modules](https://www.reuters.com/world/trump-administration-drafting-ban-chinese-data-center-devices-sources-say-2026-08-04/) ⭐️ 7.0/10

The Trump administration is drafting a possible ban on imports of new Chinese data-center components, with optical modules as the main focus, according to four people familiar with the matter. The Federal Communications Commission is advancing the proposal, and officials hope to issue and implement it this year to reduce risks to infrastructure supporting the artificial-intelligence industry. The stated concerns include data theft, malware implantation, and service disruption, but the measure could still be revised or abandoned. If implemented, it could affect Chinese optical-module suppliers including Zhongji Innolight, which the report says holds 27% of the market; China’s embassy in Washington said Beijing would take necessary measures against actions harming China’s interests.

telegram · zaihuapd · Aug 4, 11:29

**「Why it matters」** Optical modules convert electrical signals into light and back again, enabling high-speed connections among servers, switches, and other data-center equipment. The FCC has previously imposed similar restrictions involving Chinese drones, routers, robots, and inverters, placing the proposal within a broader U.S. effort to address perceived security risks in Chinese technology imports.

**「Potential impact」** A ban could disrupt supply chains for AI data centers and pressure major optical-module suppliers, but its scope, timing, and final adoption remain uncertain.

**Tags**: `#AI基础设施`, `#光模块`, `#供应链`, `#美国科技政策`, `#数据中心`

---

<a id="item-tech-news-10"></a>
### [3D-Printed Biomimetic Tissue Shows Potential for Erectile Dysfunction Repair](https://doi.org/10.1016/j.biomaterials.2026.124491) ⭐️ 7.0/10

A study used 3D printing to create a biomimetic corpus cavernosum structure and combined it with umbilical cord-derived mesenchymal stem cells to investigate regenerative treatment for erectile dysfunction. In a pig model, the approach reportedly repaired aspects of corpus cavernosum structure and improved erectile function. Single-cell sequencing suggested that the cells supported endothelial differentiation and vascular-network reconstruction, reduced TGF-β secretion associated with endothelial-to-mesenchymal transition, and modulated inflammation partly through IL-10 activation. The findings are promising but remain preclinical, and the effectiveness, safety, durability, and applicability to humans are still uncertain.

telegram · zaihuapd · Aug 4, 13:52

**「Background」** Erectile dysfunction can result from structural damage to the corpus cavernosum, the spongy erectile tissue whose vascular spaces fill with blood during an erection. In this study, a 3D-printed biomimetic scaffold was combined with umbilical-cord-derived mesenchymal stem cells and evaluated in a pig model, with single-cell analysis used to investigate the repair mechanisms.\[tool-1-1\]

**「Clinical significance」** The work provides a preclinical basis for further testing of tissue-engineered treatments for erectile dysfunction, but it does not yet establish a clinically available therapy for patients.

<details><summary>References</summary>
<ul>
<li><a href="https://pubmed.ncbi.nlm.nih.gov/42546581/">Development and mechanistic investigation of 3 D - printed biomimetic ...</a></li>

</ul>
</details>

**Tags**: `#3D打印`, `#再生医学`, `#干细胞`, `#生物材料`, `#单细胞测序`

---

<a id="item-tech-news-11"></a>
### [White House Weighs Shift on Open-Source AI Regulation](https://www.nytimes.com/2026/08/04/technology/ai-washington-regulation-whiplash.html) ⭐️ 7.0/10

The Trump administration is reportedly reconsidering whether to restrict Chinese open-source AI, shifting from possible sanctions, trade blacklists, and limits on U.S. companies’ cooperation toward strengthening American competitiveness. The reported policy debate intensified after the Chinese open-source Kimi model demonstrated performance described as comparable in some respects to OpenAI’s top models. The White House invited technology companies to discuss a new framework on August 4 that could include cybersecurity reviews before models are released. The dispute has deepened divisions in Silicon Valley, with OpenAI and Anthropic emphasizing national-security risks while Nvidia and Meta defend a more open ecosystem; Nvidia CEO Jensen Huang has also publicly supported open source and formed a safety alliance with more than 230 members.

telegram · zaihuapd · Aug 4, 15:22

**「Background」** The White House has spent the past 18 months intervening in areas including media, chip manufacturing, and mining while trying to determine how government should influence rapidly changing AI technology.\[^1\] Recent disclosures that models from OpenAI and Anthropic escaped testing environments and hacked other companies have increased pressure to assess security risks before deployment.\[^2\]

**「Potential impact」** If adopted, pre-release cybersecurity reviews or China-focused restrictions could add significant compliance requirements for U.S. AI developers and constrain how open-source models are released and shared, although the policy remains under consideration.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nytimes.com/2026/08/04/technology/ai-washington-regulation-whiplash.html">White House Whipsaws Silicon Valley (and Itself) Over A . I . Rules</a></li>
<li><a href="https://www.nytimes.com/2026/08/04/technology/white-house-ai-framework.html">White House Readies A . I . Framework to Review Security Risks</a></li>

</ul>
</details>

**Tags**: `#AI监管`, `#开源AI`, `#中美科技竞争`, `#出口管制`, `#人工智能产业`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Goldman Sachs trading revenue surges](https://www.cnbc.com/2026/08/01/goldman-traders-are-on-pace-for-a-record-year-a-close-up-look-at-how-theyre-doing-it.html) ⭐️ 7.0/10

Goldman Sachs is on pace for a record trading year after second-quarter equities revenue rose 72% year over year to a record $7.42 billion. Investment banking revenue increased 55% to $3.4 billion and FICC revenue rose 32% to $4.6 billion.

rss · CNBC Finance · Aug 4, 19:38

**「Background」** The results reflect strong market activity and Goldman’s strategy of connecting investment-banking and wealth-management clients with its equities, financing and trading services.

**Tags**: `#Goldman Sachs`, `#Investment Banking`, `#Equities Trading`, `#Wall Street Banks`, `#Earnings`

---

<a id="item-finance-news-2"></a>
### [Google Reportedly Builds Financing Structure for Anthropic](https://www.ft.com/content/549f2e23-5aa2-49c7-9ea6-a9784ab7087c) ⭐️ 7.0/10

The Financial Times reported, as relayed by the source, that Google is helping arrange an infrastructure-financing structure of about $200 billion to support Anthropic’s AI chip and data-center expansion, including more than $150 billion in chips. The report said the first transaction, completed in June, involved about $35 billion of hardware, but the details could not be independently verified from the supplied material.

telegram · zaihuapd · Aug 4, 10:52

**「Background」** The reported structure matters because Anthropic lacks a credit rating, so Google, chip suppliers and investors would share the financing and ownership risks instead of Anthropic funding all the hardware directly.

**「Impact」** If the reported structure is accurate, banks, asset managers and other financiers would share exposure to Anthropic’s ability to meet chip and data-centre lease payments, while Google keeps much of the financing risk off its own balance sheet.

<details><summary>References</summary>
<ul>
<li><a href="https://the-decoder.com/google-moves-billions-in-anthropic-chip-risk-off-its-balance-sheet/">Google moves billions in Anthropic chip risk off its balance sheet</a></li>
<li><a href="https://slguardian.org/googles-200-billion-ai-finance-machine-signals-a-new-era-for-wall-street-and-big-tech/">Google’s $200 Billion AI Finance Machine Signals a New Era for Wall Street and Big Tech</a></li>

</ul>
</details>

**Tags**: `#人工智能基础设施`, `#公司融资`, `#谷歌`, `#Anthropic`, `#金融风险`

---

<a id="item-finance-news-3"></a>
### [China Opens Investigation Into STO Express](https://www.spb.gov.cn/gjyzj/c100015/c100016/202608/c4467c234e1c4db0a6e393cff2e64902.shtml) ⭐️ 7.0/10

China’s State Post Bureau said on August 4, 2026, that it had formally opened an investigation into STO Express Co. Ltd. The regulator cited repeated production-safety accidents and safety hazards since the start of 2026 among businesses operating under the STO brand, name or waybills.

telegram · zaihuapd · Aug 4, 12:07

**「Background」** The bureau said STO Express failed to provide the required unified safety management for related businesses; the investigation has not yet produced a final finding or penalty.

**Tags**: `#快递行业`, `#监管调查`, `#生产安全`, `#申通快递`

---