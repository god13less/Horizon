---
layout: default
title: "Horizon Summary: 2026-06-25 (ZH)"
date: 2026-06-25
lang: zh
---

> 从 23 条内容中筛选出 14 条重要资讯。

---

1. [AI 首次成功读取碳化赫库兰尼姆莎草纸卷轴](#item-1) ⭐️ 9.0/10
2. [理论分析：内容路由中的注意力下沉与崩溃](#item-2) ⭐️ 9.0/10
3. [Zig 更新 bitCast 语义并改进 LLVM 后端支持](#item-3) ⭐️ 8.0/10
4. [Anthropic 指控阿里巴巴非法提取 Claude AI 模型能力](#item-4) ⭐️ 8.0/10
5. [通过 GitHub CDN 提供的浏览器兼容性数据 SQLite 数据库](#item-5) ⭐️ 8.0/10
6. [Tom MacWwright 批评 AI 生成的求职申请](#item-6) ⭐️ 8.0/10
7. [将智能体工作流编译为 LLM 权重以实现成本效益](#item-7) ⭐️ 8.0/10
8. [基于 MuJoCo 的 GPU 模拟器结合了 Newton 和 Filament 引擎](#item-8) ⭐️ 8.0/10
9. [Hacker News 趋势：18 年评论索引](#item-9) ⭐️ 7.0/10
10. [《半条命 2》成功移植到网页浏览器](#item-10) ⭐️ 7.0/10
11. [研究人员寻求进化算法优化 LMAPF 导向图的建议](#item-11) ⭐️ 7.0/10
12. [提出高维动态旋转位置编码 (HDD-RoPE)](#item-12) ⭐️ 7.0/10
13. [关于为更快的 LLM 代码生成设计专用语言的推测](#item-13) ⭐️ 6.0/10
14. [ML 背景对申请安全职位是利大于弊还是弊大于利？](#item-14) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [AI 首次成功读取碳化赫库兰尼姆莎草纸卷轴](https://scrollprize.org/firstscroll) ⭐️ 9.0/10

Vesuvius Challenge 团队利用 AI 和机器学习技术，首次成功解读了来自碳化赫库兰尼姆莎草纸卷轴的完整段落文本。 这一突破性进展解锁了长达近 2000 年的古代文本图书馆，为了解罗马帝国的历史和文化提供了前所未有的见解。 这一成就依赖于 X 射线相位衬度断层扫描技术来创建卷轴层级的详细图像，并利用机器学习算法在碳化莎草纸纤维中检测墨迹。

hackernews · verditelabs · 6月25日 15:48 · [社区讨论](https://news.ycombinator.com/item?id=48675179)

**背景**: 这些莎草纸卷轴发现于赫库兰尼姆的帕皮里别墅，在公元 79 年维苏威火山爆发时被碳化，直到现代技术允许无损成像，它们才变得可读。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://scrollprize.org/">Vesuvius Challenge — Reading the Herculaneum Scrolls with AI</a></li>
<li><a href="https://www.theguardian.com/technology/2026/jun/24/ai-read-papyrus-scroll-burnt-vesuvius-eruption">AI helps read papyrus scroll burnt to crisp during Vesuvius eruption | AI (artificial intelligence) | The Guardian</a></li>

</ul>
</details>

**社区讨论**: Vesuvius Challenge 团队的研究人员直接与社区互动以回答技术问题，而用户则讨论了翻译的准确性以及古代语气是否得到保留。

**标签**: `#AI`, `#Machine Learning`, `#Archaeology`, `#History`, `#Computational Science`

---

<a id="item-2"></a>
## [理论分析：内容路由中的注意力下沉与崩溃](https://www.reddit.com/r/MachineLearning/comments/1ufgwxl/r_all_routes_lead_to_collapse_attention_sinks/) ⭐️ 9.0/10

一项理论分析表明，在使用对范数不敏感的相似度度量时，注意力下沉和表示崩溃是内容路由的固有属性，这一现象适用于 Transformer、Mamba、RWKV 和 GAT。 这重新构建了众所周知的 Transformer 病理学，将其不仅仅视为需要修复的缺陷，而是使用对范数不敏感度量时的基本几何后果，为架构稳定性提供了统一的视角。 作者将 softmax 注意力重写为关于欧几里得距离的玻尔兹曼分布，揭示了只有当键的范数相等时这种等价性才成立，而在实践中这种情况很少见。

reddit · r/MachineLearning · /u/entropy_- · 6月25日 17:38

**背景**: 注意力下沉是指少数标记（如 BOS 标记）主导注意力分数，导致表示崩溃，即隐藏状态变得几乎平行。内容路由使用相似度度量动态确定信号路径，通常依赖于 softmax 注意力机制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ultralytics.com/glossary/attention-sinks">Attention Sinks in AI: Stability for LLMs | Ultralytics</a></li>
<li><a href="https://arxiv.org/abs/2206.03126">[2206.03126] Signal Propagation in Transformers: Theoretical Perspectives and the Role of Rank Collapse</a></li>

</ul>
</details>

**标签**: `#transformers`, `#attention-mechanisms`, `#theoretical-math`, `#routing`, `#neural-networks`

---

<a id="item-3"></a>
## [Zig 更新 bitCast 语义并改进 LLVM 后端支持](https://ziglang.org/devlog/2026/#2026-06-25) ⭐️ 8.0/10

Zig 引入了 @bitCast 函数的新语义以确保字节序无关的行为，并改进了对任意宽度整数类型（如 u4 和 i13）的 LLVM 后端支持。 这一变化通过消除位转换操作中的目标依赖行为，显著增强了系统编程的可移植性，使代码在不同架构间更易于维护和理解。 以前，将 [2]u8 位转换为 u16 在大端和小端目标上会产生不同的结果；新的逻辑位表示确保了所有平台上的行为一致。

hackernews · kouosi · 6月25日 14:19 · [社区讨论](https://news.ycombinator.com/item?id=48673825)

**背景**: 字节序决定了如何将整数等多字节数据存储在内存中，大端系统将最高有效字节放在前面，而小端系统将最低有效字节放在前面。LLVM 是一个编译器基础设施，旨在为跨各种后端的代码优化提供语言无关的中间表示。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ziglang.org/devlog/2026/?2026-06-25">Devlog Zig Programming Language</a></li>
<li><a href="https://en.wikipedia.org/wiki/Endianness">Endianness - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/LLVM">LLVM - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 开发者们赞扬了解释的技术深度，指出新的 bitCast 语义结合打包结构体逻辑将大大简化二进制头文件的处理，尽管也有人质疑任意宽度整数的实际必要性。

**标签**: `#Zig`, `#Systems Programming`, `#Compiler Design`, `#Endianness`, `#Low-Level`

---

<a id="item-4"></a>
## [Anthropic 指控阿里巴巴非法提取 Claude AI 模型能力](https://www.reuters.com/world/china/anthropic-says-alibaba-illicitly-extracted-claude-ai-model-capabilities-2026-06-24/) ⭐️ 8.0/10

Anthropic 指控阿里巴巴通过使用 API 令牌来训练竞争对手模型，非法提取了 Claude AI 模型的能力，这一行为据称是由以低于成本价销售 Claude 访问权限的中国转售商所促成的。 这一事件凸显了 AI 行业在知识产权方面的日益紧张局势，并引发了关于“蒸馏”技术和灰色市场转售商商业模式合法性的关键问题。 指控称阿里巴巴利用从中国转售商处购买的 API 令牌来训练模型，实际上是将 Claude 的输出作为训练数据，Anthropic 声称这违反了其服务条款并构成了非法提取。

hackernews · htrp · 6月24日 19:48 · [社区讨论](https://news.ycombinator.com/item?id=48664814)

**背景**: LLM 蒸馏是一种技术，通过训练较小的模型来模仿较大且更复杂的模型，通常用于创建如 GPT-4 等强大模型的高效版本。在此背景下，中国灰色市场转售商利用被盗账户以大幅折扣提供 Claude API 访问权限，收集用户提示和推理链并将其作为训练数据出售。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.datacamp.com/blog/distillation-llm">LLM Distillation Explained: Applications, Implementation & More | DataCamp</a></li>
<li><a href="https://completeaitraining.com/news/chinese-grey-market-resells-claude-api-access-at-90/">Chinese grey market resells Claude API access at 90% discount...</a></li>

</ul>
</details>

**社区讨论**: 社区争论的焦点在于“蒸馏”的定义，一些人认为定向蒸馏是一种类似于微调的标准行业做法，而另一些人则认为违反服务条款并不违法，且 LLM 在训练数据许可方面存在“原罪”。

**标签**: `#artificial-intelligence`, `#anthropic`, `#alibaba`, `#llm-distillation`, `#intellectual-property`

---

<a id="item-5"></a>
## [通过 GitHub CDN 提供的浏览器兼容性数据 SQLite 数据库](https://simonwillison.net/2026/Jun/24/browser-compat-db/#atom-everything) ⭐️ 8.0/10

Simon Willison 创建了一个新的 GitHub 仓库，将 Mozilla MDN 仓库中全面的浏览器兼容性数据转换为约 66MB 的 SQLite 数据库，该数据库使用 Claude Code for web (Opus 4.8) 和 sqlite-utils 生成。 该项目显著降低了开发者以编程方式查询浏览器兼容性数据的门槛，提供了一个轻量级的 MDN MCP 服务替代方案，可以通过 GitHub 的 CDN 以开放的 CORS 头访问。 数据库通过 GitHub Actions 工作流强制推送到 'db' 孤立分支，并带有开放的 CORS 头进行托管，可以直接使用 Datasette Lite 进行探索，而无需下载文件。

rss · Simon Willison · 6月24日 23:59

**背景**: 浏览器兼容性数据对于 Web 开发者了解不同浏览器对功能的支持情况至关重要。Mozilla 的 MDN 提供了这些数据，新的模型上下文协议 (MCP) 服务允许 AI 工具查询这些数据。该项目将这些结构化数据转换为可查询的 SQLite 数据库。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-opus-4-8">Introducing Claude Opus 4.8 \ Anthropic</a></li>
<li><a href="https://sqlite-utils.datasette.io/en/stable/index.html">sqlite - utils</a></li>

</ul>
</details>

**标签**: `#browser-compatibility`, `#sqlite`, `#claude-code`, `#data-engineering`, `#web-development`

---

<a id="item-6"></a>
## [Tom MacWwright 批评 AI 生成的求职申请](https://simonwillison.net/2026/Jun/24/tom-macwright/#atom-everything) ⭐️ 8.0/10

Tom MacWwright 发表了一篇题为《意外匿名》的批评文章，指出求职申请和作品集正越来越多地由大型语言模型（LLM）生成。 这篇评论具有重要意义，因为它解决了软件工程行业中真实性的侵蚀问题，这是一个随着 AI 工具在工作流程中的普及而日益严峻的关键问题。 MacWright 描述了一种特定的模式，即候选人使用由 LLM 生成的作品集网站，这些网站链接到 GitHub 仓库，其中的提交信息完全由 AI 生成，从而导致一种通用且缺乏人情味的职业形象。

rss · Simon Willison · 6月24日 18:13

**背景**: Tom MacWwright 是一位受人尊敬的软件工程师和开源贡献者，以在 Mapbox 和其他重要 Web 技术方面的工作而闻名。“意外匿名”的概念指的是由于使用自动化或非个人的工具，个人失去了独特的身份和声音的现象。

**标签**: `#careers`, `#ai`, `#software-engineering`, `#authenticity`, `#tom-macwright`

---

<a id="item-7"></a>
## [将智能体工作流编译为 LLM 权重以实现成本效益](https://www.reddit.com/r/MachineLearning/comments/1ufgpnh/r_compiling_agentic_workflows_into_llm_weights/) ⭐️ 8.0/10

最近的一篇研究论文表明，通过监督微调将复杂的智能体工作流编译为小型语言模型（SLM）权重，可以在降低两个数量级成本的同时实现接近前沿模型的性能。 这一突破解决了使用大型前沿模型进行编排的高额运营成本问题，为希望在不承担繁重计算负担的情况下部署特定领域 AI 智能体的企业提供了可行的替代方案。 该方法涉及使用前沿模型编排的轨迹对 SLM 进行微调，有效地将复杂的决策逻辑提炼为保留高性能的紧凑权重。

reddit · r/MachineLearning · /u/ThirdWaveCat · 6月25日 17:31

**背景**: 智能体工作流使 LLM 能够自主决定控制流以解决复杂问题，这通常需要昂贵的前沿模型。小型语言模型（SLM）提供了一种具有显著更低计算需求和部署成本的强大 AI 能力的经济替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@pankaj_pandey/understanding-agentic-concepts-in-llm-workflows-fc8115504c06">Understanding Agentic Concepts in LLM Workflows | Medium</a></li>
<li><a href="https://iterathon.tech/blog/small-language-models-enterprise-2026-cost-efficiency-guide">Small Language Models 2026: Cut AI Costs 75% with... | Iterathon</a></li>
<li><a href="https://mindster.com/mindster-blogs/small-language-models-slm-cost-efficiency/">Cut AI Costs by 90%: Why Smart Companies are Downsizing to Small ...</a></li>

</ul>
</details>

**社区讨论**: 该帖子邀请读者分享对这项技术的实际经验，引发了人们对蒸馏过程的复杂性相比成本节约的实际可行性的兴趣。

**标签**: `#LLM`, `#Fine-Tuning`, `#Cost-Efficiency`, `#Agentic Workflows`, `#SLM`

---

<a id="item-8"></a>
## [基于 MuJoCo 的 GPU 模拟器结合了 Newton 和 Filament 引擎](https://www.reddit.com/r/MachineLearning/comments/1uemrch/mujoco_derived_simulator_for_high_fidelity_vision/) ⭐️ 8.0/10

作者介绍了 MuJoFil，这是一个结合了 Nvidia 的 GPU 原生 Newton 物理引擎和 Google 的 Filament 渲染器的新模拟器，旨在创建高保真的基于视觉的强化学习环境。 该项目通过利用 GPU 原生并行化解决了 MuJoCo 中关键的 CPU 依赖瓶颈，可能为无法负担 NVIDIA Isaac Sim 的研究人员普及了高保真机器人模拟的访问权限。 MuJoFil 目前可通过 PyPI 作为开源包提供，需要 CUDA 支持，支持 PBR 纹理和 GLB、OpenUSD 等标准格式，并允许用户从 Sketchfab 和 Polyhaven 等平台导入环境。

reddit · r/MachineLearning · /u/MT1699 · 6月24日 19:07

**背景**: MuJoCo 是机器人研究中广泛使用的物理模拟器，但存在 CPU 限制，阻碍了并行化。为了克服这一问题，NVIDIA、Google DeepMind 和 Disney Research 开发了基于 NVIDIA Warp 的 GPU 原生物理引擎 Newton，而 Google 发布了开源的基于物理的渲染引擎 Filament。Isaac Sim 是另一个流行的基于 GPU 的选项，但通常需要昂贵的硬件和许可证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pub.towardsai.net/isaac-sim-vs-mujoco-the-4-000-question-that-will-define-robotics-in-2025-4c41a2984c2c">Isaac Sim vs MuJoCo 2025: GPU Robotics Simulation... | Towards AI</a></li>
<li><a href="https://vnrobo.com/en/blog/nvidia-newton-physics-engine">NVIDIA Newton 1.0: GPU Physics 475x Faster Than MJX | VnRobo</a></li>
<li><a href="https://github.com/google/filament">GitHub - google / filament : Filament is a real-time physically based...</a></li>

</ul>
</details>

**标签**: `#reinforcement-learning`, `#simulators`, `#robotics`, `#computer-vision`, `#gpu-acceleration`

---

<a id="item-9"></a>
## [Hacker News 趋势：18 年评论索引](https://hackernewstrends.com/) ⭐️ 7.0/10

一位开发者推出了 Hacker News Trends，这是一个可搜索的索引，能够分析 18 年的 Hacker News 评论，以可视化主题随时间的流行度。 该工具通过揭示长期讨论趋势，为技术社区提供了宝贵的背景信息，补充了现有的搜索工具（如 Algolia）。 该索引允许用户比较主题的流行度，但开发者指出它与 Google Trends 不同，因为它统计的是已发布的文本，而不是搜索查询。

hackernews · ytkimirti · 6月25日 14:08 · [社区讨论](https://news.ycombinator.com/item?id=48673671)

**背景**: Hacker News 是一个面向计算机科学和创业爱好者的流行社交新闻网站。虽然 Algolia 提供了当前内容的搜索引擎，但这个新工具专注于讨论的历史分析。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hn.algolia.com/">Hacker News Search, millions articles and comments at your fingertips.</a></li>
<li><a href="https://github.com/devflowinc/hn-search-RAG">GitHub - devflowinc/hn- search -RAG: Hacker News Search and RAG...</a></li>
<li><a href="https://apify.com/benthepythondev/hacker-news-intelligence">Hacker News Intelligence - Tech Jobs Startups Trends API · Apify</a></li>

</ul>
</details>

**社区讨论**: 用户称赞了该项目的实用性，但也报告了错误，包括 504 错误和数据库速率限制，而一位用户建议使用 ClickHouse 来提供类似服务。

**标签**: `#hacker-news`, `#data-analysis`, `#search-engine`, `#web-development`, `#history`

---

<a id="item-10"></a>
## [《半条命 2》成功移植到网页浏览器](https://hl2.slqnt.dev/) ⭐️ 7.0/10

一个名为“网页版半条命 2”的新项目利用 WebAssembly 和模拟技术，使这款经典游戏可以直接在网页浏览器中运行。 这一成就展示了在浏览器中直接运行复杂、高性能应用程序（如视频游戏）的技术可行性日益增强，拓展了基于网页的游戏潜力。 该移植项目利用 WebAssembly 上的 QEMU 来模拟 Source 引擎环境，尽管用户指出目前缺少一些着色器，包括角色眼睛的着色器。

hackernews · panza · 6月25日 06:00 · [社区讨论](https://news.ycombinator.com/item?id=48669534)

**背景**: WebAssembly 是一种二进制指令格式，允许使用 C++ 等语言编写的代码以接近原生的性能在网页浏览器中运行。模拟涉及在另一个系统上运行专为某个系统设计的软件，通常使用硬件虚拟化。这种组合使复杂的遗留软件（如 Valve 的 Source 引擎）能够在现代 Web 环境中运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WebAssembly">WebAssembly - Wikipedia</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/WebAssembly">WebAssembly | MDN</a></li>
<li><a href="https://flashenabled.com/webassembly-gaming/40">WebAssembly Is Quietly Revolutionizing Browser Gaming ...</a></li>

</ul>
</details>

**社区讨论**: 用户讨论了移植的技术局限性，指出缺少着色器，同时也强调了基于网页的模拟的更广泛的可访问性。一位用户提到这解决了没有 32 位支持的 macOS 用户面临的兼容性问题，另一位用户分享了他们自己将 Doom 移植到浏览器的经验。

**标签**: `#webassembly`, `#gaming`, `#emulation`, `#porting`, `#browser`

---

<a id="item-11"></a>
## [研究人员寻求进化算法优化 LMAPF 导向图的建议](https://www.reddit.com/r/MachineLearning/comments/1ufdzsr/optimising_lmapf_guidance_graphs_using/) ⭐️ 7.0/10

一名正在撰写论文的研究人员正在寻求社区建议，希望能利用进化算法优化终身多智能体路径规划（LMAPF）中导向图的边权重，以最大化吞吐量。 该话题通过将进化算法应用于复杂的优化问题，架起了人工智能/机器学习与运筹学之间的桥梁，为在多智能体系统中解决类似挑战的研究人员提供了宝贵的见解。 研究人员实现了一个基本进化算法，种群规模为 10，使用 25x25 网格（3,125 个权重）并模拟 5,000 步，但面临模拟时间过长以及需要有效的变异策略以确保可靠选择等挑战。

reddit · r/MachineLearning · /u/Michi122211 · 6月25日 15:54

**背景**: 终身多智能体路径规划（LMAPF）是多智能体路径规划（MAPF）问题的一个变体，智能体在完成前一个任务后会连续接收新任务。导向图是一种加权图，用于影响 LMAPF 算法生成的路径，其中边权重为智能体提供软引导。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2411.16506v2">Online Guidance Graph Optimization for Lifelong Multi - Agent Path...</a></li>
<li><a href="https://people.eng.unimelb.edu.au/pstuckey/papers/onlineggo.pdf">Online Guidance Graph Optimization for Lifelong Multi-Agent Path...</a></li>
<li><a href="https://expo24.leagueofrobotrunners.org/resources/pikachu.pdf">Scaling Lifelong Multi - Agent Path Finding to More Realistic Settings</a></li>

</ul>
</details>

**标签**: `#Multi-Agent Path Finding`, `#Evolutionary Algorithms`, `#Optimization`, `#Machine Learning`, `#Dissertation`

---

<a id="item-12"></a>
## [提出高维动态旋转位置编码 (HDD-RoPE)](https://www.reddit.com/r/MachineLearning/comments/1uelcm9/high_dimensional_dynamic_rotary_positional/) ⭐️ 7.0/10

作者引入了高维动态旋转位置编码 (HDD-RoPE)，这是一种新颖的位置编码方法，在 TinyStories 数据集上比标准的 RoPE 提高了收敛速度。 这一新颖的架构贡献解决了标准旋转位置编码 (RoPE) 的核心局限性，并在标准基准测试上展示了有前景的实证结果，为 Transformer 模型提供了潜在的改进。 与标准 RoPE 将向量拆分为 2D 向量对不同，HDD-RoPE 将块拆分为任意大小（例如 4），以创建多维位置轴，并根据层激活使旋转量依赖于数据。

reddit · r/MachineLearning · /u/mikayahlevi · 6月24日 18:16

**背景**: 旋转位置编码 (RoPE) 通过在多维空间中旋转向量来编码位置信息，使模型能够自然地学习相对位置。标准 RoPE 通常将高维向量拆分为 2D 向量对，以处理线性序列。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=GQPOtyITy54">RoPE ( Rotary positional embeddings ) explained: The... - YouTube</a></li>
<li><a href="https://mortalapps.com/learn/nlp-and-llms/rotary-positional-embeddings/">Rotary Positional Embeddings — NLP & LLMs | MortalApps</a></li>

</ul>
</details>

**标签**: `#Machine Learning`, `#Positional Embeddings`, `#Transformers`, `#NLP`, `#Research`

---

<a id="item-13"></a>
## [关于为更快的 LLM 代码生成设计专用语言的推测](https://www.reddit.com/r/MachineLearning/comments/1ufgw7z/would_having_a_dedicated_programming_language/) ⭐️ 6.0/10

一位 Reddit 用户提出了一个理论概念，即设计一种专为减少 Token 数量和噪声而优化的专用编程语言，以提高大型语言模型（LLM）的代码生成速度和效率。 这一讨论突显了通过解决分词效率和上下文窗口限制来优化 LLM 推理的潜在前沿，这是当前 AI 发展中的关键瓶颈。 该提议认为，一种密集型语言可以让 LLM 在 100 万个 Token 的上下文窗口中比 Python 容纳多 100 倍的信息，并移除分号和花括号等语法“噪声”。

reddit · r/MachineLearning · /u/Spongebubs · 6月25日 17:38

**背景**: LLM 通过将文本分解为 Token（可以是单词或单词的一部分）来处理文本；优化分词对于提高推理速度和最大化上下文窗口容量至关重要。密集型编程语言的概念借鉴了 Halide 等系统，这些系统旨在最大化信息密度以提高计算效率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@harishpillai1994/optimizing-tokenization-for-faster-and-efficient-llm-processing-bdc87b8f9fe3">Optimizing Tokenization for Faster and Efficient LLM ... | Medium</a></li>
<li><a href="https://cs343d.github.io/archive/winter2023/lectures/lecture5.dense.pdf">lecture5. dense</a></li>

</ul>
</details>

**标签**: `#LLMs`, `#Programming Languages`, `#Inference`, `#Tokenization`, `#Theory`

---

<a id="item-14"></a>
## [ML 背景对申请安全职位是利大于弊还是弊大于利？](https://www.reddit.com/r/MachineLearning/comments/1uff20h/does_ml_background_help_or_hurt_when_applying_for/) ⭐️ 6.0/10

一位机器学习工程师正在寻求建议，询问如何在申请网络安全职位时构建自己的非传统背景，以防止招聘人员将自己归类。 这一讨论解决了专业人士从 AI/ML 向安全领域转型时面临的常见挑战，强调了战略性简历构建对于克服行业刻板印象的重要性。 用户担心在简历上列出“ML/AI 工程师”可能会导致招聘人员忽略他们在该领域的实际动手安全经验。

reddit · r/MachineLearning · /u/Xorphian · 6月25日 16:32

**背景**: 在竞争激烈的软件行业中，“pigeonholing”（刻板印象/归类）指的是被不公平地限制在特定类型的职位或职业道路上，这可能会限制职业发展。同样，信息安全简历往往无法打动招聘人员，因为它们列出了工具和任务，却没有突出可衡量的风险降低或业务影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://workplace.stackexchange.com/questions/63033/career-pigeonholing">software industry - Career Pigeonholing - The Workplace Stack...</a></li>
<li><a href="https://enhancv.com/resume-examples/information-security-engineer/">10 Information Security Engineer Resume Examples & Guide for 2026</a></li>

</ul>
</details>

**标签**: `#Career Advice`, `#Machine Learning`, `#Cybersecurity`, `#Resume`, `#Industry Transition`

---