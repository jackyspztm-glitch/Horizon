---
layout: default
title: "Horizon Summary: 2026-08-04 (EN)"
date: 2026-08-04
lang: en
---

> From 41 items, 16 important content pieces were selected

---

**Technology News**
1. [Thermo Fisher DNA Devices Expose Long-Term Evidence to Tampering](#item-tech-news-1) ⭐️ 8.0/10
2. [Why LLMs Reward Existing Expertise](#item-tech-news-2) ⭐️ 7.0/10
3. [Survey Examines Advances in Mathematics and Theoretical Computer Science](#item-tech-news-3) ⭐️ 7.0/10
4. [ComfyUI Adds Day-One Support for MiniMax H3](#item-tech-news-4) ⭐️ 7.0/10
5. [Andy Pavlo Joins ClickHouse to Establish ClickHouse Labs](#item-tech-news-5) ⭐️ 7.0/10
6. [Jane Street’s Bonsai Brings OCaml-Centric UI Development to the Fore](#item-tech-news-6) ⭐️ 7.0/10
7. [AirLLM Runs 70B Models on a 4GB GPU](#item-tech-news-7) ⭐️ 7.0/10
8. [LLMs Could Make Open-Source Developer Tools More Modifiable](#item-tech-news-8) ⭐️ 7.0/10
9. [Kimi K3 Architecture and Inference Analysis](#item-tech-news-9) ⭐️ 7.0/10
10. [Qwen Announces 3.8-Max with 2.4 Trillion Parameters](#item-tech-news-10) ⭐️ 7.0/10
11. [Investigation Finds Widespread Abuse of U.S. License-Plate Camera Systems](#item-tech-news-11) ⭐️ 7.0/10
12. [Apple Photos Faces $32.5 Billion Illinois Biometric-Privacy Lawsuit](#item-tech-news-12) ⭐️ 7.0/10
13. [Apple Challenges UK Order for iCloud Backup Access](#item-tech-news-13) ⭐️ 7.0/10

**Financial News**
1. [California Diesel Prices Reach $6.92 per Gallon](#item-finance-news-1) ⭐️ 7.0/10
2. [Visa to buy BioCatch for $2.4 billion](#item-finance-news-2) ⭐️ 7.0/10
3. [Shanghai fines 12 ride-hailing platforms more than 25 million yuan](#item-finance-news-3) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Thermo Fisher DNA Devices Expose Long-Term Evidence to Tampering](https://www.wsj.com/tech/cybersecurity/security-flaw-placed-30-years-of-dna-evidence-at-risk-of-hacking-1932775a) ⭐️ 8.0/10

Researchers in forensic science and computer science found a vulnerability in Thermo Fisher Scientific DNA-analysis equipment used by most U.S. crime laboratories. An attacker who bypassed laboratory controls could covertly alter DNA scan files, potentially putting roughly 30 years of evidence dating back to 1995 at risk; in testing, researchers used Anthropic’s Claude to generate code that modified a file in about 45 minutes without triggering commonly used analysis software. Thermo Fisher acknowledged the issue privately in July, issued a high-severity advisory last Friday, and released a software update adding digital signatures. The company said it is working with the U.S. Cybersecurity and Infrastructure Security Agency and that no exploitation has been observed, while the effect on pending or closed cases remains unclear.

telegram · zaihuapd · Aug 3, 05:15

**「Background」** DNA-analysis systems produce digital files that laboratories use to interpret genetic profiles and preserve forensic evidence. Digital signatures can help verify that files were produced or modified by an authorized system, making unauthorized changes easier to detect, although they do not by themselves resolve weaknesses in laboratory access controls or determine whether older files were altered.

**「Impact」** More than 200 U.S. laboratories reportedly have inconsistent security controls, so affected facilities must address the vulnerability and consider the integrity of stored DNA evidence even though no real-world exploitation has been reported.

**Tags**: `#网络安全`, `#数字取证`, `#人工智能`, `#软件供应链`, `#数据完整性`

---

<a id="item-tech-news-2"></a>
### [Why LLMs Reward Existing Expertise](https://www.seangoedecke.com/llms-reward-expertise/) ⭐️ 7.0/10

The piece argues that large language models tend to amplify a user’s existing expertise rather than eliminate the need for it. Domain knowledge helps users frame tasks, steer conversations, recognize errors, and judge whether generated results fit the real problem. This is especially important in software development, where understanding a specific codebase and its constraints may matter as much as general programming knowledge. The argument presents LLMs as powerful extensions of skilled users, but unreliable substitutes for the judgment and context those users provide.

hackernews · MaxMussio · Aug 3, 21:13 · [Discussion](https://news.ycombinator.com/item?id=49161518)

**「Background」** Large language models generate responses from learned patterns, so they can produce plausible material across domains without guaranteeing that it is correct or appropriate. Domain expertise helps users frame precise requests, recognize omissions or errors, and judge whether an answer fits the specific problem; the article argues that this matters more than generic prompting技巧 alone. \[sic\]

**「Impact」** Users without relevant expertise may be able to produce plausible outputs with LLMs but remain less able to detect incorrect assumptions, hidden defects, or unsuitable solutions.

**「Community Discussion」** Commenters broadly agreed that LLMs act as amplifiers or conversational mirrors, adapting their responses to the user’s framing, vocabulary, and apparent level of understanding. The discussion also stressed that practical familiarity with a particular codebase requires hands-on work, and that prompting alone cannot replace that context.

<details><summary>References</summary>
<ul>
<li><a href="https://www.seangoedecke.com/llms-reward-expertise/">LLMs reward expertise</a></li>

</ul>
</details>

**Tags**: `#large-language-models`, `#software-engineering`, `#developer-tools`, `#human-ai-collaboration`

---

<a id="item-tech-news-3"></a>
### [Survey Examines Advances in Mathematics and Theoretical Computer Science](https://openai.com/index/ten-advances-in-mathematics/) ⭐️ 7.0/10

OpenAI’s article surveys ten recent advances in mathematics and theoretical computer science. It also examines how artificial intelligence may be changing mathematical discovery, automated proof generation, and proof verification. The supplied material does not identify the ten advances or provide enough technical detail to evaluate their individual novelty, results, or limitations.

hackernews · milkshakes · Aug 3, 16:27 · [Discussion](https://news.ycombinator.com/item?id=49157930)

**「Background」** Mathematics and theoretical computer science investigate both abstract structures and the limits and methods of computation. The article places recent results in areas including geometry, cryptography, and complexity alongside the broader question of how AI might assist mathematical discovery and proof verification.

**「Impact」** The article frames AI-assisted conjecture generation and mechanically checked proofs as increasingly important areas for mathematicians and theoretical computer scientists, while leaving the practical scale of that change uncertain.

**「Community Discussion」** Commenters broadly agreed that AI is improving computers’ ability to generate, test, or verify mathematical arguments, while emphasizing that this does not mean all mathematics is automatically solved. Others questioned whether current systems can produce mathematical intuition and raised concerns about the article’s apparent promotion and timing.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/ten-advances-in-mathematics/">Ten advances in mathematics and theoretical computer science</a></li>

</ul>
</details>

**Tags**: `#mathematics`, `#theoretical-computer-science`, `#AI-research`, `#automated-reasoning`

---

<a id="item-tech-news-4"></a>
### [ComfyUI Adds Day-One Support for MiniMax H3](https://blog.comfy.org/p/minimax-h3-day-0-support-in-comfyui) ⭐️ 7.0/10

ComfyUI now supports MiniMax H3 from day one, bringing open-weight local generation of high-resolution video with native audio capabilities. The integration is positioned to support video output up to 2K resolution, although inference remains resource-intensive and memory-heavy. Community examples suggest strong results in ordinary scenes, while unusual concepts and some close-up shots can still show artifacts or an AI-smoothing effect.

hackernews · vblanco · Aug 3, 13:34 · [Discussion](https://news.ycombinator.com/item?id=49155629)

**「Required context」** ComfyUI is a node-based interface for running and composing generative-AI models locally. MiniMax H3 is an open-weights, multimodal video model that accepts text, images, video, or audio and can generate clips with stereo sound at up to 2K resolution and 15 seconds in length.【tool-1-1】

**「Practical impact」** Local ComfyUI users can experiment with audio-enabled MiniMax H3 video generation without relying exclusively on a hosted service, but a commenter reported that a 16 GB RTX 4070 Ti Super needed about 10 minutes to generate 10 seconds of 480p video.

**「Community reaction」** Commenters praised several clips as a major improvement over current video models, while noting failures in unconventional scenarios and residual visual smoothing. Discussion also focused on a reported 66% memory-footprint reduction through pruned modulation weights, with questions about whether the technique could generalize to language models.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.comfy.org/p/minimax-h3-day-0-support-in-comfyui">MiniMax H 3 Day-0 Support in ComfyUI : Open Weights, Native Audio ...</a></li>

</ul>
</details>

**Tags**: `#ComfyUI`, `#Open Weights`, `#Video Generation`, `#Generative AI`

---

<a id="item-tech-news-5"></a>
### [Andy Pavlo Joins ClickHouse to Establish ClickHouse Labs](https://clickhouse.com/blog/andy-pavlo-joins-clickhouse) ⭐️ 7.0/10

Andy Pavlo is joining ClickHouse to establish ClickHouse Labs, a move that signals greater company investment in database-systems research and infrastructure innovation. The announcement connects Pavlo’s academic and teaching background with ClickHouse’s work on analytical database systems, but provides few concrete details about the lab’s projects, structure, or timeline. Its potential focus includes advancing database technology and strengthening collaboration between industry and academia.

hackernews · nikolay\_sivko · Aug 3, 14:09 · [Discussion](https://news.ycombinator.com/item?id=49156011)

**「Background」** ClickHouse is an analytical database system designed for high-performance online analytical processing \(OLAP\). ClickHouse says Andy Pavlo is joining the company to establish and lead a new research team called ClickHouse Labs, linking database-systems research with development of its infrastructure.

**「Community Discussion」** Commenters broadly welcomed the appointment, citing Pavlo’s lectures and research while hoping ClickHouse will fund academic database research and continue supporting educational material. Others used the news to raise technical questions about OLAP convergence with Trino, decoupled compute and storage, ingestion, indexing, and table formats such as Iceberg and Paimon.

<details><summary>References</summary>
<ul>
<li><a href="https://clickhouse.com/blog/andy-pavlo-joins-clickhouse">Andy Pavlo joins ClickHouse to establish ClickHouse Labs | ClickHouse</a></li>

</ul>
</details>

**Tags**: `#Databases`, `#ClickHouse`, `#Systems Research`, `#OLAP`, `#Open Source`

---

<a id="item-tech-news-6"></a>
### [Jane Street’s Bonsai Brings OCaml-Centric UI Development to the Fore](https://github.com/janestreet/bonsai) ⭐️ 7.0/10

Jane Street’s Bonsai is an OCaml UI library for building frontend applications, extending the language’s role across application development. Its OCaml foundation could allow teams to share language-level types and code between frontend and backend systems, an approach highlighted in the accompanying discussion. The project also raises practical questions about how it compares with Melange, how much access it provides to the JavaScript ecosystem—including React and GraphQL—and whether teams will adopt it beyond Jane Street’s environment. The supplied material does not provide detailed implementation, compatibility, or performance data.

hackernews · KolmogorovComp · Aug 3, 08:29 · [Discussion](https://news.ycombinator.com/item?id=49152842)

**「Background」** Bonsai is an OCaml library for building performant, reactive web applications, with design inspiration from Elm. It uses js\_of\_ocaml to target web applications and is organized as a collection of libraries for reusable components within an Incremental-style UI framework such as Incr\_dom.

**「Community discussion」** Commenters welcomed the possibility of using one language and shared types across frontend and backend systems, and pointed to a Signals and Threads episode about the project. Others asked how Bonsai compares with Melange and whether its approach sacrifices JavaScript ecosystem integration, while separate comments questioned its visual design and sought evidence of production use in internal applications.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/janestreet/bonsai">GitHub - janestreet / bonsai : A library for building dynamic webapps...</a></li>
<li><a href="https://opam.ocaml.org/packages/bonsai/bonsai.v0.14.0/">The homepage of opam, a package manager for OCaml</a></li>

</ul>
</details>

**Tags**: `#OCaml`, `#UI frameworks`, `#type systems`, `#frontend development`, `#open source`

---

<a id="item-tech-news-7"></a>
### [AirLLM Runs 70B Models on a 4GB GPU](https://github.com/lyogavin/airllm) ⭐️ 7.0/10

AirLLM is presented as a way to run inference with 70-billion-parameter language models using a GPU with only 4GB of memory. It reduces the active memory required for inference, potentially making large open-weight models usable on otherwise constrained hardware. The tradeoff is substantially lower performance than conventional deployment, while the project’s long-term maintainability and distinct advantages over established layer-streaming or quantization tools remain uncertain.

hackernews · Anon84 · Aug 3, 11:15 · [Discussion](https://news.ycombinator.com/item?id=49154228)

**「Background」** A 70B-parameter model can require roughly 130GB just for its weights, far exceeding the memory of typical consumer GPUs and often requiring multiple data-center GPUs to load directly. AirLLM addresses this constraint by reducing the amount of model data that must reside in GPU memory during inference, aiming to run such models on a single 4GB card without quantization, distillation, or pruning.\[tool-1-1\]\[tool-1-2\]

**「Practical consequence」** Users with limited GPU memory can experiment with much larger models, but the resulting latency may make interactive or production use impractical.

**「Community reaction」** Commenters questioned what AirLLM adds beyond quantized models and tools such as llama.cpp, and whether projects in this area will be maintained; one reported a Kimi K3 benchmark of 292 seconds per token on an RTX 6000 Ada with 48GB of memory. Others viewed the work as useful pressure for more efficient model architectures, while asking whether the full model still must be downloaded and how memory is divided between GPU, system RAM, and storage.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/lyogavin/airllm">lyogavin / airllm : AirLLM 70 B inference with single 4 GB GPU · GitHub</a></li>
<li><a href="https://huggingface.co/blog/lyogavin/airllm">Unbelievable! Run 70 B LLM Inference on a Single 4 GB GPU with This...</a></li>

</ul>
</details>

**Tags**: `#LLM inference`, `#Memory optimization`, `#GPU computing`, `#Open source`, `#Large language models`

---

<a id="item-tech-news-8"></a>
### [LLMs Could Make Open-Source Developer Tools More Modifiable](https://simonwillison.net/2026/Aug/3/devtools-must-be-open-source-exedev/#atom-everything) ⭐️ 7.0/10

Simon Willison argues that LLM-assisted programming makes the original promise of open-source developer tools—examining and modifying how they work—more practical for programmers. Previously, compiling, understanding, and changing frequently used tools often required too much time, even for expert developers, so users depended on others to exercise that freedom. Willison now regularly asks Claude to clone repositories and explain code, and uses Codex or Claude Code to check out and build software, treating setup failures as a low-cost experiment. He has not yet made a habit of modifying the tools he uses, so this remains a personal observation about a possible direction rather than an empirical study.

rss · Simon Willison · Aug 3, 15:30

**「Background」** Open-source software gives users the legal and technical ability to inspect, modify, and rebuild the programs they use, but doing so has traditionally required substantial time and programming effort. LLM-based coding assistants can reduce that friction by helping users clone repositories, understand code, resolve build problems, and prepare modifications, although the source item presents this as an emerging possibility rather than an established practice.

**「Why it matters」** For programmers using LLM coding assistants, open-source developer tools may become easier to inspect, build, and eventually customize without investing as much manual time.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Aug/3/devtools-must-be-open-source-exedev/">Comment: Devtools must be open source (exe.dev)</a></li>

</ul>
</details>

**Tags**: `#Open Source`, `#Developer Tools`, `#Large Language Models`, `#Software Engineering`

---

<a id="item-tech-news-9"></a>
### [Kimi K3 Architecture and Inference Analysis](https://newsletter.semianalysis.com/p/kimi-k3-the-manos-the-mythos-the) ⭐️ 7.0/10

The article examines Kimi K3’s architecture and inference characteristics. It focuses on compressed memory, attention across model depth, latent expert routing, and inference performance. The supplied material identifies these technical areas but does not provide enough detail to assess the implementation, measured results, or practical advantages.

rss · Semianalysis · Aug 3, 19:42

**「Background」** Kimi K3 is described as a 2.8-trillion-parameter mixture-of-experts model that activates 104 billion parameters, supports native vision, and provides a one-million-token context window. Its architecture combines Kimi Delta Attention and Attention Residuals for information flow across sequences and model depth, while Stable LatentMoE routes inputs among 896 experts and activates 16 of them per step.【tool-1-2】

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2607.24653v1">[2607.24653v1] Kimi K3: Open Frontier Intelligence - arXiv.org</a></li>

</ul>
</details>

**Tags**: `#Large Language Models`, `#AI Architecture`, `#Mixture-of-Experts`, `#Inference Optimization`

---

<a id="item-tech-news-10"></a>
### [Qwen Announces 3.8-Max with 2.4 Trillion Parameters](https://qwen.ai/blog?id=qwen3.8) ⭐️ 7.0/10

Qwen has announced Qwen 3.8-Max, a model it says contains 2.4 trillion total parameters and 95 billion active parameters, based on the Qwen 3.5 architecture. The company says it will release the model weights next week, marking its first planned open release of a Max-tier model, while an API is already available through QwenCloud. Qwen claims improvements in coding, work, research, and long-horizon tasks, including autonomous project construction lasting more than 10 days and a result in the WWW2025 multimodal dialogue-intent recognition competition that surpassed 458 of 526 teams. The announcement is currently a promotional overview: independent verification, detailed benchmark methodology, licensing terms, and the exact weight-release date are not provided.

telegram · zaihuapd · Aug 3, 02:31

**「Background」** A model’s total parameter count describes the full set of learned weights, while its active-parameter figure indicates how many parameters are used for a given input; these figures are not directly interchangeable for estimating inference cost. “Open-weight” means the model weights are made available for others to download and run, but the practical rights and obligations still depend on the accompanying license, hardware requirements, and release timing.

**「Impact」** If Qwen delivers the weights under a usable license, developers and organizations could gain access to an unusually large open model with 95 billion active parameters, but its practical value remains dependent on the release, documentation, and independently reproducible evaluations.

**Tags**: `#Qwen`, `#开源大模型`, `#大语言模型`, `#模型评测`, `#AI基础设施`

---

<a id="item-tech-news-11"></a>
### [Investigation Finds Widespread Abuse of U.S. License-Plate Camera Systems](https://www.washingtonpost.com/technology/2026/08/02/how-police-officers-used-vast-network-cameras-spy-their-exes/) ⭐️ 7.0/10

A Washington Post investigation published August 2 found that at least 50 U.S. law-enforcement personnel have been accused or charged with misusing Flock and other license-plate recognition systems, including 26 cases involving surveillance of wives, girlfriends, ex-partners, or women they were interested in. At least 46 cases involved Flock, whose network includes more than 120,000 cameras across over 6,000 communities and records about 20 billion plate scans each month. In one case, Georgia police chief Michael Steffman searched for his former girlfriend and her daughter’s plates roughly 600 times; he was arrested in November 2025 and died by suicide before his trial in April 2026. Flock’s CEO said abuse cannot be eliminated entirely, while the company has introduced an optional audit-assistance feature; privacy groups say oversight remains inadequate.

telegram · zaihuapd · Aug 3, 09:03

**「Background」** Automatic license-plate recognition \(ALPR\) cameras capture vehicle plates and associated time and location data, allowing police to search for vehicles across connected camera networks. Flock markets this infrastructure as a crime-fighting tool, but its expansion has prompted disputes over whether persistent vehicle tracking constitutes excessive surveillance and how access should be controlled.【tool-1-1】【tool-1-2】

**「Why it matters」** The cases show that access to large-scale vehicle-location data can enable personal surveillance when agencies lack strong auditing and enforcement safeguards; only 13 states require audits, while at least eight classify such misuse as a crime.

<details><summary>References</summary>
<ul>
<li><a href="https://www.washingtonpost.com/technology/2026/08/02/how-police-officers-used-vast-network-cameras-spy-their-exes/">How rogue officers turned a nationwide camera network into a ...</a></li>
<li><a href="https://www.washingtonpost.com/nation/2026/05/17/citys-ai-license-plate-cameras-led-an-uproar-state-emergency/">AI license plate cameras tore this town apart and led to a ...</a></li>

</ul>
</details>

**Tags**: `#车牌识别`, `#隐私与监控`, `#网络安全`, `#技术治理`

---

<a id="item-tech-news-12"></a>
### [Apple Photos Faces $32.5 Billion Illinois Biometric-Privacy Lawsuit](https://appleinsider.com/articles/26/08/03/apple-photos-facial-features-prompt-a-325b-class-action-lawsuit) ⭐️ 7.0/10

Apple is facing an Illinois class-action lawsuit seeking up to $32.5 billion over allegations that the Photos app processed facial-feature data without users’ informed consent. The complaint alleges that Photos scans people appearing in images, generates facial features for them, uses algorithms to identify iPhone users, and synchronizes related data through iCloud. Apple argued that the process does not create biometric identifiers and that privacy safeguards were in place, but a judge ruled in June that the case could proceed as a class action, and the U.S. Court of Appeals for the Seventh Circuit rejected Apple’s appeal on June 30. The proceedings establish no final finding that Apple violated the law, and the allegations and potential damages remain unresolved.

telegram · zaihuapd · Aug 3, 14:33

**「背景」** 伊利诺伊州《生物识别信息隐私法》（BIPA）是本案所依据的州级隐私法规，涉及企业收集和处理人脸等生物识别信息时的同意与告知义务。苹果 Photos 的相关功能会分析照片中的人脸并生成用于识别的面部特征，因此诉讼争议集中在这些处理是否构成受 BIPA 约束的生物识别数据收集，以及用户是否获得了充分告知和同意。\[tool-1-2\]

**「Impact」** The case could expose Apple to substantial litigation and compliance pressure under Illinois’s Biometric Information Privacy Act and potentially affect about 6.5 million Illinois consumers, depending on the eventual outcome.

<details><summary>References</summary>
<ul>
<li><a href="https://appleinsider.com/articles/26/08/03/apple-photos-facial-features-prompt-a-325b-class-action-lawsuit">Apple Photos&#x27; facial features prompt a $32.5B class-action ...</a></li>

</ul>
</details>

**Tags**: `#隐私与数据保护`, `#人脸识别`, `#苹果生态`, `#生物识别数据`, `#科技诉讼`

---

<a id="item-tech-news-13"></a>
### [Apple Challenges UK Order for iCloud Backup Access](https://www.ft.com/content/2cc9c96a-0e5b-4c33-a95a-3d11072a145c?syn-25a6b1a6=1) ⭐️ 7.0/10

Apple has filed a legal challenge with the UK Investigatory Powers Tribunal against a Technical Capability Notice \(TCN\) requiring access to encrypted iCloud backups for UK users. Apple argues that creating such access, effectively a backdoor, would weaken security for users, while Apple and the UK Home Office have declined to comment because of legal restrictions. The dispute follows the UK’s withdrawal of an earlier demand covering users in both the UK and the United States after a disagreement with the US, followed by a new notice limited to UK users. Apple removed iCloud Advanced Data Protection from the UK in February 2025, and the tribunal is scheduled to hold a case-management hearing next month; the legal challenge has not yet determined whether the government can enforce the notice.

telegram · zaihuapd · Aug 3, 15:40

**「Background」** A technical capability notice \(TCN\) is a UK government demand requiring a communications provider to develop or maintain the technical ability to access data under specified legal conditions. Apple’s Advanced Data Protection feature provides end-to-end encryption for additional iCloud data, including backups, meaning Apple generally cannot access the protected content without the user’s recovery credentials; the challenge was filed with the UK Investigatory Powers Tribunal.【tool-1-1】【tool-1-3】

**「Why it matters」** The case could determine whether the UK can compel a technology company to weaken end-to-end protection for cloud backups and may influence how Apple and other providers handle encryption obligations across different jurisdictions.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theguardian.com/technology/2026/aug/03/apple-legal-challenge-uk-government-data-access">Apple launches legal challenge against UK government demand ...</a></li>
<li><a href="https://www.macrumors.com/2026/08/03/apple-legal-challenge-against-uk-demand/">Apple Launches New Legal Challenge Against UK Backdoor Demand</a></li>

</ul>
</details>

**Tags**: `#数据隐私`, `#加密安全`, `#苹果`, `#英国科技监管`, `#云备份`

---

## Financial News

<a id="item-finance-news-1"></a>
### [California Diesel Prices Reach $6.92 per Gallon](https://www.cnbc.com/2026/08/03/californias-diesel-prices-have-jumped-since-the-iran-war-started-with-ripple-effects-across-the-country.html) ⭐️ 7.0/10

California&\#x27;s average diesel price has risen to $6.92 per gallon from $5.10 before the Iran war, compared with $5.36 nationally, as global refining capacity tightens.

rss · CNBC Finance · Aug 3, 19:20

**「Background」** Experts attribute the tighter diesel market to the Iran conflict and attacks on Russian refining infrastructure; California prices are also elevated by refinery closures, limited fuel pipelines, and strict environmental rules.

**「Potential impact」** Because nearly one-third of containership trade passes through the San Pedro Bay port complex, higher California fuel costs could raise trucking, rail, and delivered-goods costs nationwide, according to JPMorgan analysts.

**Tags**: `#Diesel prices`, `#Energy markets`, `#Supply chains`, `#California economy`, `#Geopolitical risk`

---

<a id="item-finance-news-2"></a>
### [Visa to buy BioCatch for $2.4 billion](https://www.cnbc.com/2026/08/03/visa-buys-biocatch-fraud-detection.html) ⭐️ 7.0/10

Visa said it will acquire fraud-detection company BioCatch for $2.4 billion in cash to strengthen defenses against AI-powered scams and account takeovers; the deal is expected to close by the end of Visa’s fiscal second quarter in 2027, subject to regulatory approval.

rss · CNBC Finance · Aug 3, 16:44

**「Background」** Visa’s value-added services business provides financial institutions with fraud prevention, cybersecurity and analytics tools, while BioCatch’s behavioral-biometrics platform analyzes signals such as keystrokes and touchscreen pressure to distinguish genuine users from scammers and automated attacks.

**「What it means」** Banks and other financial institutions could gain access to BioCatch’s behavioral-biometrics software, which analyzes signals such as typing patterns and touchscreen pressure to identify users, scammers and automated bots before a payment is made.

**Tags**: `#Visa`, `#Mergers and acquisitions`, `#Cybersecurity`, `#Payments fraud`, `#AI scams`

---

<a id="item-finance-news-3"></a>
### [Shanghai fines 12 ride-hailing platforms more than 25 million yuan](https://m.thepaper.cn/newsDetail_forward_33710474) ⭐️ 7.0/10

Shanghai transport authorities reportedly issued the first coordinated administrative penalties against 12 ride-hailing platforms on August 3, totaling more than 25 million yuan. The action covered 479 vehicles found to be noncompliant in cases opened in June 2026.

telegram · zaihuapd · Aug 3, 08:27

**「Background」** The penalties followed investigations opened in June 2026 into illegal passenger transport, focusing on whether ride-hailing platforms had properly verified vehicle and driver qualifications and held the required operating licenses.

**「Impact」** The penalties put greater responsibility on platforms to verify driver and vehicle qualifications, follow compliant dispatch practices, and remove noncompliant transport capacity in Shanghai.

**Tags**: `#网约车监管`, `#行政处罚`, `#平台经济`, `#交通政策`

---