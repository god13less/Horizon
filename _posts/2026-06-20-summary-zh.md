---
layout: default
title: "Horizon Summary: 2026-06-20 (ZH)"
date: 2026-06-20
lang: zh
---

> 从 19 条内容中筛选出 13 条重要资讯。

---

1. [CSS Quake：完全使用 Web 技术构建的经典 FPS 游戏](#item-1) ⭐️ 8.0/10
2. [DVD-JEPA：LeCun 世界模型的开源实现](#item-2) ⭐️ 8.0/10
3. [ICML 立场论文：时间序列建模需要动力系统视角](#item-3) ⭐️ 8.0/10
4. [大规模 LLM 推理开源手册](#item-4) ⭐️ 8.0/10
5. [开发者构建了简化的 minFLUX 实现以方便研究](#item-5) ⭐️ 8.0/10
6. [TSAuditor：用于时间序列数据完整性的框架](#item-6) ⭐️ 8.0/10
7. [探索数字色彩再现的极限](#item-7) ⭐️ 7.0/10
8. [将网站 HTML 存储在 Favicon 图像中](#item-8) ⭐️ 7.0/10
9. [MCP 的真正价值：隔离认证流程](#item-9) ⭐️ 7.0/10
10. [辩论：没有顶级论文的博士毕业生](#item-10) ⭐️ 7.0/10
11. [全球 PM2.5 预测模型克服方差陷阱](#item-11) ⭐️ 7.0/10
12. [YouTube 发布“从零构建大语言模型”工作坊](#item-12) ⭐️ 6.0/10
13. [如何获取 Books3 数据集用于研究](#item-13) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [CSS Quake：完全使用 Web 技术构建的经典 FPS 游戏](https://cssquake.com/) ⭐️ 8.0/10

cssQuake 是对 1996 年经典游戏 Quake 的完整可玩复刻版，完全在浏览器中运行，使用 HTML、CSS 和 JavaScript。 该项目展示了 Web 技术栈的极端能力，通过仅使用 CSS 变换渲染复杂的 3D BSP 世界，推动了前端工程可能性的边界。 该引擎将原始 Quake 数据预处理为浏览器可用的 JSON，并使用 PolyCSS 渲染几何体，尽管它仍然需要 JavaScript 来处理游戏逻辑，并且目前缺少一些原始机制，例如射击按钮。

hackernews · msalsas · 6月20日 10:49 · [社区讨论](https://news.ycombinator.com/item?id=48608223)

**背景**: Quake（1996 年）是一款具有里程碑意义的第一人称射击游戏，普及了 PC 上的 3D 游戏。该项目通过使用 DOM（文档对象模型）和 CSS 3D 变换来创建一个“假”的 3D 环境，而不是使用 WebGL 或 Canvas，从而重新构想这款游戏。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/LayoutitStudio/cssQuake">GitHub - LayoutitStudio/cssQuake: A port of Quake (1996 ...</a></li>
<li><a href="https://cssquake.wtf/">cssQuake - Quake rendered with HTML and CSS</a></li>
<li><a href="https://www.ic.work/article/cssquake-runs-quake-in-css-but-demo-is-not-product">cssQuake：CSS 跑起《Quake》，但别把 demo 当产品 - ic.work</a></li>

</ul>
</details>

**社区讨论**: 社区普遍赞扬这一技术成就，用户将其体验与经典硬件进行比较，并指出该项目的魅力，尽管也有人指出它仍然依赖 JavaScript 并且存在一些轻微的游戏玩法不一致之处。

**标签**: `#web-development`, `#css`, `#game-dev`, `#retro`, `#engineering`

---

<a id="item-2"></a>
## [DVD-JEPA：LeCun 世界模型的开源实现](https://www.reddit.com/r/MachineLearning/comments/1uatlzx/dvdjepa_an_opensource_fullyreproducible_jepa/) ⭐️ 8.0/10

一个名为 DVD-JEPA 的开源项目通过训练模型来预测 16×16 盒子内弹跳 DVD 标志的未来表示，展示了联合嵌入预测架构 (JEPA)，且无需像素级监督。 该实现验证了 Yann LeCun 在世界建模方面的范式转变，证明预测抽象表示而非像素可以产生有用的、能在浏览器中高效运行的异常检测模型。 该模型使用 32 维潜在空间，并通过线性探针实现高精度，而可选的解码器允许其在潜在漂移发生前“做梦”生成约 20 步的未来帧。

reddit · r/MachineLearning · /u/NielsRogge · 6月20日 10:52

**背景**: 传统世界模型经常因为试图预测下一帧的每个像素而陷入困境，这在计算上既昂贵又往往不可行，因为细节具有不可预测性。Yann LeCun 提出了联合嵌入预测架构 (JEPA) 作为一种替代方案，专注于预测未来的抽象表示，丢弃不可预测的像素细节。这种方法是 I-JEPA 和 V-JEPA 等较新模型的基石。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.turingpost.com/p/jepa">What is Joint Embedding Predictive Architecture (JEPA)?</a></li>
<li><a href="https://arxiv.org/abs/2301.08243">[2301.08243] Self-Supervised Learning from Images with a Joint-Embedding Predictive Architecture</a></li>
<li><a href="https://rohitbandaru.github.io/blog/JEPA-Deep-Dive/">Rohit Bandaru | Deep Dive into Yann LeCun’s JEPA</a></li>

</ul>
</details>

**标签**: `#World Models`, `#JEPA`, `#Representation Learning`, `#Self-Supervised Learning`, `#Computer Vision`

---

<a id="item-3"></a>
## [ICML 立场论文：时间序列建模需要动力系统视角](https://www.reddit.com/r/MachineLearning/comments/1uark0u/time_series_modeling_needs_a_dynamical_systems/) ⭐️ 8.0/10

一篇 ICML 2026 的立场论文论证了引入动力系统视角对于推动时间序列建模超越单纯的预测，转向理解复杂系统底层规则的重要性。 这一视角意义重大，因为它解决了当前基础模型在捕捉混沌系统物理特性方面的根本局限性，并为真正的域外泛化提供了新颖的理论框架。 论文建议优先考虑动力系统重建（DSR）训练技术，如广义教师强迫，在模拟而非人工函数上进行预训练，并从 transformers 转回现代 RNNs 以捕捉长期统计特性。

reddit · r/MachineLearning · /u/DangerousFunny1371 · 6月20日 08:47

**背景**: 自然和工程中的时间序列数据通常源于底层动力系统，复杂系统往往具有混沌特性。动力系统重建（DSR）旨在从时间序列测量中推断底层过程的生成模型，超越简单的预测以理解动力规则。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2306.04406">[2306.04406] Generalized Teacher Forcing for Learning Chaotic Dynamics</a></li>
<li><a href="https://arxiv.org/abs/2504.04011">[2504.04011] Foundation Models for Time Series: A Survey</a></li>

</ul>
</details>

**标签**: `#Time Series`, `#Dynamical Systems`, `#Machine Learning`, `#ICML`, `#Generalization`

---

<a id="item-4"></a>
## [大规模 LLM 推理开源手册](https://www.reddit.com/r/MachineLearning/comments/1uavduv/an_open_handbook_on_llm_inference_at_scale_gpu/) ⭐️ 8.0/10

一位开发者在 GitHub 上发布了名为 'LLM Inference at Scale' 的开源手册，详细介绍了 GPU 内部机制、内存层次结构和瓶颈，并配有 mermaid 图表。 该资源对系统和基础设施社区意义重大，因为它架起了理论知识与实际生产挑战之间的桥梁，提供了优化 vLLM 和 TensorRT-LLM 等推理引擎的可视化指南。 手册特别涵盖了为什么 GPU 在推理期间经常处于空闲状态、内存层次结构如何限制吞吐量，以及与 KV 缓存管理和 DRAM 带宽饱和相关的具体瓶颈。

reddit · r/MachineLearning · /u/YouFirst295 · 6月20日 12:27

**背景**: LLM 推理涉及使用预训练模型生成文本，其中 GPU 内存层次结构和高效的 KV 缓存管理对性能至关重要。vLLM、SGLang 和 TensorRT-LLM 等流行的推理引擎优化了这些过程，但了解底层硬件瓶颈对于最大化吞吐量至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/mastering-llm-techniques-inference-optimization/">Mastering LLM Techniques: Inference Optimization | NVIDIA Technical...</a></li>
<li><a href="https://medium.com/@indiai/gpu-memory-hierarchy-how-ai-training-actually-works-24f00cc13050">GPU Memory Hierarchy — How AI Training Actually Works | by AIQuest | Medium</a></li>
<li><a href="https://arxiv.org/html/2503.08311v2">Mind the Memory Gap: Unveiling GPU Bottlenecks in Large-Batch LLM Inference</a></li>

</ul>
</details>

**标签**: `#LLM`, `#Inference`, `#GPU`, `#Systems`, `#Architecture`

---

<a id="item-5"></a>
## [开发者构建了简化的 minFLUX 实现以方便研究](https://www.reddit.com/r/MachineLearning/comments/1ub1db3/studying_flux_in_diffusers_library_was_hard_so_i/) ⭐️ 8.0/10

Saurabh Purohit 发布了 minFLUX，这是一个简化的 FLUX 扩散模型 PyTorch 实现，包含 VAE 和 transformer 组件，并提供了与官方 HuggingFace diffusers 库的详细逐行映射。 该项目解决了 diffusers 库的复杂性，使研究人员和开发者更容易理解 FLUX 的架构，并比较 FLUX.1 和 FLUX.2 之间的差异。 该实现包括训练和推理循环、RoPE 和时间步嵌入等共享工具，并特别强调了 FLUX.2 在 transformer 块和 VAE 归一化等方面的架构改进。

reddit · r/MachineLearning · /u/Other-Eye-8152 · 6月20日 16:50

**背景**: 扩散模型是生成式 AI 模型，它们学习逆转向数据添加噪声的过程，而 Flow Matching 是一种相关技术，将数据分布建模为连续流。变分自编码器（VAE）通常用于这些模型中，在通过 transformer 架构处理之前，将输入数据压缩到潜在空间。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://learnopencv.com/rope-position-embeddings/">Inside RoPE: Rotary Magic into Position Embeddings - LearnOpenCV</a></li>

</ul>
</details>

**标签**: `#diffusion-models`, `#pytorch`, `#open-source`, `#flux`, `#deep-learning`

---

<a id="item-6"></a>
## [TSAuditor：用于时间序列数据完整性的框架](https://www.reddit.com/r/MachineLearning/comments/1ub15wf/tsauditor_a_timeseries_auditing_framework_p/) ⭐️ 8.0/10

一位开发者发布了 TSAuditor，这是一个开源的 Python 框架，可在 PyPI 上获取，旨在检测时间序列数据集中的数据完整性问题，如时间顺序中断、数据泄露和序列尖峰。 该工具解决了时间序列机器学习中一个关键但常被忽视的问题，即数据完整性问题可能导致模型准确率虚高，因此对于从业者来说，验证其数据管道至关重要。 该框架为为何特定数据点存在故障提供了详细的证据和描述，建议了修复方法，并包含一个对比笔记本，展示了其在识别隐藏数据问题方面优于标准分析工具。

reddit · r/MachineLearning · /u/severecaseofsarcarsm · 6月20日 16:41

**背景**: 机器学习中的数据泄露是指训练期间使用的信息在预测时不可用，这通常会导致性能评估过于乐观。在时间序列背景下，这可能是由于不正确的训练/测试分割或在滚动窗口中使用未来数据造成的。TSAuditor 通过审计数据的时间顺序和全局边界来帮助防止这些微妙错误。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Leakage_(machine_learning)">Leakage (machine learning) - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/data-leakage-machine-learning">What is Data Leakage in Machine Learning? | IBM</a></li>

</ul>
</details>

**标签**: `#time-series`, `#data-validation`, `#machine-learning`, `#data-leakage`, `#open-source`

---

<a id="item-7"></a>
## [探索数字色彩再现的极限](https://moultano.wordpress.com/2026/06/19/where-to-find-the-colors-your-screen-cant-show-you/) ⭐️ 7.0/10

一篇文章探讨了人类视觉的物理学原理以及数字色彩再现的局限性，特别讨论了屏幕无法显示某些颜色的现象。 了解这些局限性对于改进显示技术和数字媒体的色彩准确性至关重要，弥合了技术规格与人类感知之间的差距。 文章指出，虽然仅用三种原色无法再现某些饱和的蓝绿色，但 CIE 1931 色度图可能夸大了它们的重要性，而 sRGB 色彩空间通常无法再现饱和的橙色、红色和紫色。

hackernews · moultano · 6月20日 03:36 · [社区讨论](https://news.ycombinator.com/item?id=48606140)

**背景**: sRGB、DCI-P3 和 Rec. 2020 等色彩空间定义了显示器可以显示的颜色范围。DCI-P3 是用于数字电影的广色域标准，而 Rec. 2020 是超高清标准，其覆盖的可见光颜色范围比 Rec. 709 宽得多。人类视觉也受到眼睛中视锥细胞重叠的限制，这会影响我们感知色彩差异的方式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DCI-P3">DCI-P3 - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Rec._2020">Rec. 2020 - Wikipedia</a></li>
<li><a href="https://pixflow.net/blog/what-is-dci-p3-the-ultimate-guide-to-the-wide-color-gamut-standard-for-displays/">What is DCI-P3? The Ultimate Guide to the Wide Color Gamut ...</a></li>

</ul>
</details>

**社区讨论**: 评论者讨论了 CIE 1931 图表的准确性，指出人类视觉无法区分该区域的许多颜色。其他人分享了他们对磷光屏的个人体验，例如 B&O MX8000，指出了其独特的青色强度，而一些人讨论了单独刺激视锥细胞以看到新颜色的可能性。

**标签**: `#color-science`, `#display-tech`, `#human-perception`, `#hardware`

---

<a id="item-8"></a>
## [将网站 HTML 存储在 Favicon 图像中](https://www.timwehrle.de/blog/i-stored-a-website-in-a-favicon/) ⭐️ 7.0/10

作者演示了一种技术手段，将网站的 HTML 内容编码并存储在 favicon.ico 文件中，然后将其返回给浏览器以渲染页面。 这种创造性的方法突显了浏览器内部机制的灵活性，并引发了关于数据存储限制、潜在隐私风险（如浏览器指纹识别）以及 Web 标准界限的重要讨论。 该实现依赖于将 HTML 编码到 favicon 格式中，浏览器通常会请求 /favicon.ico，但文章指出需要一个小型的引导加载程序来解码图像数据。

hackernews · theanonymousone · 6月20日 05:33 · [社区讨论](https://news.ycombinator.com/item?id=48606619)

**背景**: Favicon 是与网站相关联的小图标，通常显示在浏览器标签页或地址栏中。浏览器通常会从服务器请求一个名为 favicon.ico 的文件，虽然它在技术上是一个图像文件，但可以通过各种方式进行操作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/HTML_favicon">HTML favicon</a></li>

</ul>
</details>

**社区讨论**: 社区成员建议使用 SVG 直接存储标记或使用 PNG 块以获得更好的压缩率等替代方法，而其他人则提出了潜在的安全风险，例如通过 favicon 缓存追踪用户。

**标签**: `#web-development`, `#browser-internals`, `#security`, `#data-storage`, `#hacks`

---

<a id="item-9"></a>
## [MCP 的真正价值：隔离认证流程](https://simonwillison.net/2026/Jun/19/sean-lynch/#atom-everything) ⭐️ 7.0/10

Sean Lynch 指出，Model Context Protocol (MCP) 相比之前的 agent skills 或 CLI 工具的主要优势在于，它能够将认证流程隔离在 agent 的上下文窗口之外。 这一架构见解意义重大，因为它解决了一个关键的安全和设计漏洞，即敏感凭证可能会在上下文窗口中暴露或丢失，从而可能提高 AI agent 的安全性。 Lynch 认为 MCP 的理想形式可能仅作为 API 的认证网关，这仍然是一个重大的架构胜利，因为它将安全逻辑与 agent 的核心执行框架解耦。

rss · Simon Willison · 6月19日 22:45

**背景**: Model Context Protocol (MCP) 是一个开放标准，用于将 Claude 或 ChatGPT 等 AI 应用程序连接到外部数据源和工具，其功能类似于 AI 的“USB-C 端口”。“上下文窗口”指的是 LLM 在单次传递中可以处理的信息量，管理好上下文窗口对于 agent 保持相关历史记录和避免丢失信息至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://modelcontextprotocol.io/docs/getting-started/intro">What is the Model Context Protocol (MCP)?</a></li>
<li><a href="https://www.anthropic.com/news/model-context-protocol">Introducing the Model Context Protocol \ Anthropic</a></li>
<li><a href="https://medium.com/@aryanbkrishnan/ai-agent-engineer-roadmap-2-4-context-window-management-cf427a4ebd37">AI Agent Engineer Roadmap-2.4. Context window ... | Medium</a></li>

</ul>
</details>

**标签**: `#MCP`, `#Model Context Protocol`, `#LLM Architecture`, `#Security`, `#AI Agents`

---

<a id="item-10"></a>
## [辩论：没有顶级论文的博士毕业生](https://www.reddit.com/r/MachineLearning/comments/1uazlhg/would_you_let_an_ml_phd_student_graduate_without/) ⭐️ 7.0/10

一位 Reddit 用户询问机器学习社区，是否应该支持一名博士学生在四年后毕业，尽管其论文工作扎实，但没有在 NeurIPS、ICML 或 ICLR 等顶级会议发表论文，尽管他们有三篇第一作者“A 级”论文。 这场讨论凸显了学术界在顶级会议发表论文的巨大压力，并质疑博士成功的定义是否应仅基于发表指标，而非研究的整体质量。 该学生在四年内完成了一个连贯的论文方向，拥有三篇第一作者“A 级”论文，但未能在 NeurIPS、ICML、ICLR 或 CVPR 等主要会议上被录用。

reddit · r/MachineLearning · /u/Hope999991 · 6月20日 15:36

**背景**: 在机器学习领域，“A*ML 顶级会议”通常指 NeurIPS、ICML、ICLR 和 CVPR 等最负盛名的会议，这些会议的录用率极低，论文也经过严格的排名。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://matejgazda.com/posts/paper-map.html">Paper Map: NeurIPS / CVPR / ICLR / ICML 2024–2025 - Matej Gazda</a></li>
<li><a href="https://algoverseairesearch.org/blog/icml-iclr-aaai-student-guide">Beyond NeurIPS: A Student's Guide to ICML, ICLR, AAAI, and ...</a></li>

</ul>
</details>

**标签**: `#Academia`, `#Machine Learning`, `#PhD`, `#Research`, `#Career`

---

<a id="item-11"></a>
## [全球 PM2.5 预测模型克服方差陷阱](https://www.reddit.com/r/MachineLearning/comments/1uar4vc/built_a_global_aq_pm25_forecaster_ml_model_p/) ⭐️ 7.0/10

作者利用超过 160 万行的 OpenAQ 和 NASA 数据，为四个国家构建了端到端的预测管道，用基于对齐的自动回归架构和波动率矩阵注入，替换了失效的标准梯度提升回归器。 这一突破解决了印度和英国等混乱环境中的“方差陷阱”，标准模型因无法预测突然的动量转变而失效，从而可能提高全球空气质量监测的可靠性。 新架构解耦了预测范围（1、7、14、30 天），并注入 3 天滚动波动率矩阵以防止数据泄漏，在全球范围内实现了 MASE < 1.0，并在 30 天范围内比混乱基线高出 57%的准确率。

reddit · r/MachineLearning · /u/Divyanshailani · 6月20日 08:20

**背景**: 时间序列预测中的“方差陷阱”是指模型的误差在长期范围内递归累积，导致其在混乱环境中失效，此时简单的延续猜测甚至优于复杂模型。自动回归模型基于过去的观测值分解未来值，但标准实现往往难以处理长期依赖和分布偏移。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tech.ajinhub.com/en/blog/the-forecasting-trap-navigating-latent-chaos-in-time-series/">The Forecasting Trap: Navigating Latent Chaos in Time Series</a></li>
<li><a href="https://www.geeksforgeeks.org/machine-learning/time-series-analysis-and-forecasting/">Time Series Analysis and Forecasting - GeeksforGeeks</a></li>
<li><a href="https://arxiv.org/abs/2103.02062">[2103.02062] Variance Reduced Training with Stratified ... Time Series Analysis and Forecasting - GeeksforGeeks Evaluating Time Series Forecasting Models: Metrics and Best ... A Comprehensive Survey of Time Series Forecasting ... Chapter 4 Time Series Forecasting | Time Series with R 5.3 Time Series Forecasting Methods - Principles of Data ...</a></li>

</ul>
</details>

**标签**: `#Machine Learning`, `#Forecasting`, `#Air Quality`, `#Gradient Boosting`, `#Time Series`

---

<a id="item-12"></a>
## [YouTube 发布“从零构建大语言模型”工作坊](https://www.reddit.com/r/MachineLearning/comments/1uazlnd/hi_reddit_i_posted_my_build_your_own_llm_workshop/) ⭐️ 6.0/10

一个综合性的工作坊已在 YouTube 发布，旨在教授如何使用 Python 和 PyTorch 从零开始构建大语言模型，涵盖机器学习基础、Transformer 架构和训练技术。 该资源通过弥合理论数学与实际实现之间的差距，为从业者解构了复杂的 LLM 内部机制，这对于理解现代 AI 生态系统至关重要。 课程涵盖了 SwiGLU 激活函数、Triton GPU 内核和 RoPE 嵌入等高级主题，采用幻灯片、Excel 直观理解和代码示例的三步教学方法。

reddit · r/MachineLearning · /u/JustinAngel · 6月20日 15:36

**背景**: 像 GPT-4 这样的大语言模型依赖于 Transformer 架构和复杂的训练流程，包括权重初始化、注意力机制和优化算法，以处理和生成类人文本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@s_boudefel/exploring-swiglu-the-activation-function-powering-modern-llms-9697f88221e7">Exploring SwiGLU : The Activation Function Powering Modern ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Weight_initialization">Weight initialization - Wikipedia</a></li>

</ul>
</details>

**标签**: `#LLM`, `#Machine Learning`, `#Education`, `#PyTorch`, `#Deep Learning`

---

<a id="item-13"></a>
## [如何获取 Books3 数据集用于研究](https://www.reddit.com/r/MachineLearning/comments/1uaoomx/how_to_access_books3_dataset_for_research/) ⭐️ 6.0/10

一位研究人员在 Reddit 上询问如何获取 Books3 数据集用于学术目的。 Books3 数据集意义重大，因为它曾被用于训练 Meta 的 LLaMA 等主要语言模型，使其成为理解 AI 训练数据和版权问题的关键资源。 Books3 是包含在 The Pile 中的约 20 万本电子书合集，但由于版权违规，该数据集已于 2023 年 8 月被反盗版组织从公开访问中移除。

reddit · r/MachineLearning · /u/xolmnyc · 6月20日 05:55

**背景**: Books3 由 Shawn Presser 于 2020 年创建，作为 EleutherAI 的 The Pile 开源数据集的一部分发布。它包含著名作家的作品，曾被广泛用于训练大型语言模型，尽管后来发现其源自非法文件共享服务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://interestingengineering.com/innovation/anti-piracy-group-shuts-down-books3-a-popular-dataset-for-ai-models">Anti-piracy group shuts down Books3, a popular dataset for AI ...</a></li>
<li><a href="https://rettighedsalliancen.com/rights-alliance-removes-the-illegal-books3-dataset-used-to-train-artificial-intelligence/">Rights Alliance removes the illegal Books3 dataset used to ...</a></li>
<li><a href="https://github.com/psmedia/Books3Info">GitHub - psmedia/Books3Info: Data and information related to ...</a></li>

</ul>
</details>

**标签**: `#datasets`, `#machine-learning`, `#nlp`, `#research`

---