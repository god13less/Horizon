---
layout: default
title: "Horizon Summary: 2026-06-14 (ZH)"
date: 2026-06-14
lang: zh
---

> 从 16 条内容中筛选出 13 条重要资讯。

---

1. [为使用工具的 LLM 代理引入“验证税”](#item-1) ⭐️ 9.0/10
2. [第 10 代本田思域使用不安全的 AOSP 测试密钥进行更新](#item-2) ⭐️ 8.0/10
3. [美国人口普查局禁止在统计产品中使用噪声注入](#item-3) ⭐️ 8.0/10
4. [Z.ai 发布开源 GLM-5.2 作为应对受限访问的反制措施](#item-4) ⭐️ 8.0/10
5. [胰腺癌突破：靶向此前被认为“不可成药”的 KRAS 基因](#item-5) ⭐️ 8.0/10
6. [亚马逊 CEO 与官员谈话引发美国对 Anthropic 模型的打压](#item-6) ⭐️ 8.0/10
7. [ReactOS 在真实硬件上运行 3D 加速版半条命](#item-7) ⭐️ 8.0/10
8. [Pyodide 314.0 允许发布 WASM 轮子到 PyPI](#item-8) ⭐️ 8.0/10
9. [将 SQLite 查询结果列映射回其来源 table.column](#item-9) ⭐️ 8.0/10
10. [选择异常检测还是分类来识别癌症模拟物](#item-10) ⭐️ 8.0/10
11. [对“完美”60fps UI 动画的批评](#item-11) ⭐️ 7.0/10
12. [罕见的 Game Boy WorkBoy 生产力配件被发掘](#item-12) ⭐️ 7.0/10
13. [作者构建免费双语机器学习笔记本课程，寻求社区反馈](#item-13) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [为使用工具的 LLM 代理引入“验证税”](https://www.reddit.com/r/MachineLearning/comments/1u58mkq/the_verifier_tax_horizondependent_safetysuccess/) ⭐️ 9.0/10

研究人员在 ACM CAIS 2026 上提出了一篇论文，介绍了“验证税”，这是一个分析使用工具的 LLM 代理中安全验证与任务完成成功之间权衡的框架。 这项工作意义重大，因为它通过量化安全执行如何影响任务成功率，解决了 AI 安全评估中的一个关键空白，为从业者提供了关于安全与能力权衡在何处产生影响的切实指导。 该研究定义了三种结果——安全成功、不安全成功和失败——并提出了一种使用确定性检查后跟基于 LLM 的验证器的两层验证架构，发现随着任务视野的增加，验证虽然减少了不安全成功，但也降低了任务完成率。

reddit · r/MachineLearning · /u/AccomplishedLeg1508 · 6月14日 02:09

**背景**: τ-bench 是一个旨在模拟用户与提供特定领域工具的语言代理之间动态对话的基准测试，有助于研究人员评估代理处理现实世界场景的能力。“验证税”这一概念源于这样一个观察：向代理添加运行时安全执行通常会引入巨大的运营开销和计算成本，但并不能保证安全的完成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2603.19328">[2603.19328] The Verifier Tax: Horizon Dependent Safety Success Tradeoffs in Tool Using LLM Agents</a></li>
<li><a href="https://www.caisconf.org/program/2026/papers/the-verifier-tax-horizon-dependent-safety-success-tradeoffs-in-tool-using-llm-ag">The Verifier Tax: Horizon Dependent Safety–Success Tradeoffs in Tool Using LLM Agents — CAIS 2026 — ACM CAIS 2026</a></li>
<li><a href="https://github.com/sierra-research/tau-bench">sierra-research/tau-bench: Code and Data for Tau-Bench · GitHub</a></li>

</ul>
</details>

**标签**: `#LLM Agents`, `#AI Safety`, `#Evaluation Metrics`, `#Tool Use`, `#ACM CAIS`

---

<a id="item-2"></a>
## [第 10 代本田思域使用不安全的 AOSP 测试密钥进行更新](https://juniperspring.org/posts/honda-evil-valet/) ⭐️ 8.0/10

研究人员发现，第 10 代本田思域使用不安全的更新机制，系统固件使用公开的 AOSP 测试密钥签名，允许通过 USB 驱动器执行任意代码。 这一漏洞对数百万车主构成重大安全风险，可能允许攻击者未经 root 权限即可入侵车辆的信息娱乐系统，甚至可能影响其他关键组件。 更新机制依赖于 Android 4.2.2rc1 时代的恢复包，并带有本田添加的可被欺骗的版本检查，该漏洞利用仅需物理接触前 USB 端口。

hackernews · librick · 6月14日 00:49 · [社区讨论](https://news.ycombinator.com/item?id=48523080)

**背景**: AOSP 测试密钥是 Android 开源项目源代码树中为测试目的提供的默认加密密钥，与私有发布密钥不同，它们在互联网上公开可用，因此不适合用于保护商业设备。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/wfairclough/android_aosp_keys">GitHub - wfairclough/android_aosp_keys: The platform keys ...</a></li>
<li><a href="https://aospinsider.com/courses/aosp-course-1/43-platform-keys-release-keys/">Platform Keys & Release Keys - AOSP Foundations | AOSPInsider</a></li>
<li><a href="https://source.android.com/docs/core/ota/sign_builds">Sign builds for release | Android Open Source Project</a></li>

</ul>
</details>

**社区讨论**: 社区普遍批评本田的安全实践不佳，一些用户指出漏洞源于更新过程中缺乏签名验证，而不仅仅是签名方法本身。

**标签**: `#security`, `#automotive`, `#hardware`, `#vulnerability`, `#android`

---

<a id="item-3"></a>
## [美国人口普查局禁止在统计产品中使用噪声注入](https://desfontain.es/blog/banning-noise.html) ⭐️ 8.0/10

美国人口普查局决定禁止在统计产品中使用噪声注入（差分隐私），这一决定推翻了自 2020 年人口普查以来一直实行的长期政策。 这一政策转变对政府统计的数据隐私标准产生了重大影响，并可能导致用于重新划分选区和研究的细粒度公开数据减少。 商务部命令专门针对 2030 年人口普查中使用差分隐私，用粗化（coarsening）和抑制（suppression）技术取而代之，同时仍保持保护个人隐私的目标。

hackernews · nl · 6月13日 13:54 · [社区讨论](https://news.ycombinator.com/item?id=48517377)

**背景**: 差分隐私是一种数学上严谨的框架，通过向数据集添加受控的噪声来防止个人被重新识别。美国人口普查局在 2020 年采用了这一技术，以在允许进行有用的统计分析的同时保护受访者的身份。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.npr.org/2026/06/12/nx-s1-5855734/census-bureau-data-differential-privacy">A Trump push to cut 'statistical noise' could mean less data from the Census Bureau - NPR</a></li>

</ul>
</details>

**社区讨论**: 社区成员表达了深切的担忧，一些人认为该禁令移除了武器化敏感政府数据的必要防火墙，而噪声注入对于防止欺诈是必要的。

**标签**: `#privacy`, `#differential-privacy`, `#census`, `#government-data`, `#security`

---

<a id="item-4"></a>
## [Z.ai 发布开源 GLM-5.2 作为应对受限访问的反制措施](https://twitter.com/jietang/status/2065784751345287314) ⭐️ 8.0/10

Z.ai 创始人宣布开源发布 GLM-5.2，将其定位为应对 Fable 等前沿模型受限访问的反制措施。 此次发布凸显了 AI 可访问性方面的关键地缘政治紧张局势，对比了中国实验室的开源方法与美国模型的受限访问。 GLM-5.2 是一个拥有 7440 亿参数的混合专家模型，每个 token 激活 400 亿参数，提供 100 万 token 的上下文窗口和 MIT 许可证。

hackernews · aloknnikhil · 6月13日 16:18 · [社区讨论](https://news.ycombinator.com/item?id=48518684)

**背景**: Z.ai（前身为智谱 AI）自 2025 年 7 月以来一直在以免费开源许可证发布其 GLM 模型，并在更名后继续。最近，美国政府下令 Anthropic 暂停向外国用户开放其最先进的模型，导致了突然的限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/when-ai-access-becomes-geopolitics-why-washington-restricted-veidt-kiyve">When AI access becomes geopolitics: Why Washington restricted ...</a></li>
<li><a href="https://www.reuters.com/technology/us-blocks-foreign-access-anthropics-most-advanced-ai-models-axios-reports-2026-06-13/">Anthropic disables top-tier AI models after US order limiting ...</a></li>
<li><a href="https://www.aimadetools.com/blog/what-is-claude-mythos-5/">What is Claude Mythos 5: The Restricted Frontier Model Explained</a></li>

</ul>
</details>

**社区讨论**: 用户指出此次发布恰逢 Anthropic 模型被禁，并称赞中国实验室开源模型，将其与美国模型的受限访问形成对比。

**标签**: `#AI`, `#Open Source`, `#LLMs`, `#Geopolitics`, `#Z.ai`

---

<a id="item-5"></a>
## [胰腺癌突破：靶向此前被认为“不可成药”的 KRAS 基因](https://economist.com/science-and-technology/2026/06/12/treating-pancreatic-tumours-may-have-revealed-cancers-master-switch) ⭐️ 8.0/10

研究人员成功靶向了此前被认为“不可成药”的 KRAS 基因，使用名为 daraxonrasib 的新药物，该药物在治疗胰腺肿瘤方面显示出前景。 这一突破意义重大，因为 KRAS 突变驱动了约 90%的胰腺癌，这种疾病历史上生存率极低且治疗选择有限。 这一发现具体适用于 20%的肿瘤，虽然这是一个重大进步，但它并非所有癌症的通用疗法。

hackernews · andsoitis · 6月13日 13:34 · [社区讨论](https://news.ycombinator.com/item?id=48517199)

**背景**: KRAS 基因为制造一种参与细胞信号通路传导的蛋白质提供指令。该基因的突变，特别是在 G12、G13 和 Q61 等热点残基处的突变，会导致 RAS/MAPK 通路持续激活，从而引起细胞不受控制的生长和癌症。几十年来，由于 KRAS 蛋白表面光滑且缺乏明显的结合位点，它一直被认为是“不可成药”的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/KRAS">KRAS - Wikipedia</a></li>
<li><a href="https://www.mskcc.org/news/new-kras-targeted-therapy-shows-promise-against-pancreatic">New KRAS Targeted Therapy Shows Promise Against Pancreatic Cancer</a></li>

</ul>
</details>

**社区讨论**: 社区成员在表达治疗希望的同时指出了局限性；一位评论者强调了更好的诊断和早期检测的必要性，而另一位则指出这是仅适用于 20%肿瘤的“关键弱点”。

**标签**: `#oncology`, `#drug-discovery`, `#genetics`, `#biotech`, `#KRAS`

---

<a id="item-6"></a>
## [亚马逊 CEO 与官员谈话引发美国对 Anthropic 模型的打压](https://www.wsj.com/tech/ai/amazon-ceos-talks-with-u-s-officials-triggered-crackdown-on-anthropic-models-dcc90578?st=Yct6gx&reflink=desktopwebshare_permalink) ⭐️ 8.0/10

据《华尔街日报》报道，亚马逊 CEO 安迪·贾西向美国官员提出了关于 Anthropic 模型的安全担忧，这据称导致政府对这些 AI 系统进行了打压。 这则新闻凸显了 AI 安全担忧与政府监管之间日益加深的交集，特别是考虑到亚马逊是 Anthropic 的主要投资者和合作伙伴，这引发了关于创新与国家安全之间平衡的疑问。 此次打压针对的是 Anthropic 最先进的模型，如 Claude Opus 4.8，该模型在 Super-Agent 等基准测试中表现出强大的能力，尽管触发政府行动的具体技术限制或基准测试结果尚不清楚。

hackernews · ls612 · 6月13日 16:57 · [社区讨论](https://news.ycombinator.com/item?id=48519092)

**背景**: Anthropic 是一家领先的 AI 公司，以其开发的 Claude 系列大型语言模型而闻名，该模型采用“宪法 AI”技术进行训练，以提高伦理合规性。该公司与亚马逊有着深厚的战略合作伙伴关系，亚马逊向 Anthropic 投资了 50 亿美元，并为其训练和部署 Claude 提供了高达 5 吉瓦的算力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/anthropic-amazon-compute">Anthropic and Amazon expand collaboration for up to 5 ...</a></li>
<li><a href="https://www.anthropic.com/claude/opus">Claude Opus \ Anthropic</a></li>

</ul>
</details>

**社区讨论**: 社区成员对政府行动的动机进行了辩论，一些人质疑为什么 Anthropic 会被 singled 出来，因为所有大型语言模型都容易受到越狱攻击；而另一些人则认为，打压可能与特定的技术限制或战略关系有关，而非出于恶意。

**标签**: `#AI Safety`, `#Government Regulation`, `#LLM Security`, `#Anthropic`, `#Amazon`

---

<a id="item-7"></a>
## [ReactOS 在真实硬件上运行 3D 加速版半条命](https://www.phoronix.com/news/ReactOS-Running-Half-Life) ⭐️ 8.0/10

ReactOS 成功在真实硬件上运行了 3D 加速版的半条命，这对这个开源操作系统来说是一个重要的里程碑。 这一成就证明了在原生开源环境中运行旧版 Windows 游戏的可行性，而不需要依赖 Wine 或 DOSBox 等模拟层。 这一成功不仅要求 ReactOS 与游戏应用程序兼容，还要求它与驱动程序对底层操作系统的假设兼容，利用了原生的驱动程序堆栈。

hackernews · jeditobe · 6月13日 23:22 · [社区讨论](https://news.ycombinator.com/item?id=48522486)

**背景**: ReactOS 是一个旨在与 Windows NT 内核和 API 兼容的免费开源操作系统。半条命是一款于 1998 年发布的经典第一人称射击游戏，它依赖 OpenGL 进行 3D 图形加速。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://windowsforum.com/threads/reactos-runs-windows-half-life-in-game-on-real-hardware-nt-kernel-driver-win32-progress.425367/">ReactOS Runs Windows Half-Life In-Game on Real Hardware—NT ...</a></li>
<li><a href="https://reactos.org/wiki/Supported_Hardware/Video_cards">Supported Hardware/Video cards - ReactOS Wiki</a></li>

</ul>
</details>

**社区讨论**: 虽然一些用户指出现代 Linux 游戏已经提供了类似的功能，但其他人强调了直接运行原生 NVIDIA 驱动程序堆栈的技术意义，还有一位用户指出 ReactOS 已经开发了 28 年。

**标签**: `#open-source`, `#operating-systems`, `#gaming`, `#ReactOS`, `#hardware-acceleration`

---

<a id="item-8"></a>
## [Pyodide 314.0 允许发布 WASM 轮子到 PyPI](https://simonwillison.net/2026/Jun/13/publishing-wasm-wheels/#atom-everything) ⭐️ 8.0/10

Pyodide 314.0 版本引入了新的标准（PEP 783），允许开发者直接将 WebAssembly Python 轮子发布到 PyPI，从而消除了核心维护者进行手动维护的需求。 这种基础设施改进对 Python 生态系统具有重要意义，因为它将包维护从中心化的瓶颈转变为可扩展的、社区驱动的流程，从而促进了 Python 在浏览器中的更广泛采用。 这些轮子使用新的平台标签 'pyemscripten'，第一个示例包 'luau-wasm' 已经发布，这证明了维护者可以使用 cibuildwheel 等标准工具来构建和部署它们。

rss · Simon Willison · 6月13日 23:55

**背景**: Pyodide 是 CPython 到 WebAssembly 的移植版本，允许在浏览器中运行 Python。此前，核心团队必须手动构建和托管超过 300 个包，这给社区造成了瓶颈。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://peps.python.org/pep-0783/">PEP 783 – Emscripten Packaging | peps.python.org</a></li>
<li><a href="https://blog.pyodide.org/posts/314-release/">Pyodide 314.0 Release | Pyodide blog</a></li>

</ul>
</details>

**标签**: `#Python`, `#WebAssembly`, `#Pyodide`, `#PyPI`, `#PEP 783`

---

<a id="item-9"></a>
## [将 SQLite 查询结果列映射回其来源 table.column](https://simonwillison.net/2026/Jun/13/sqlite-column-provenance/#atom-everything) ⭐️ 8.0/10

Simon Willison 探索使用 AI 和各种方法来程序化地识别 SQLite 查询中每个结果列的来源 `table.column`，包括处理复杂的连接和 CTE。 这项研究使 Datasette 能够以额外的来源信息渲染任意 SQL 查询，提高了开发人员在处理复杂 SQL 查询时的数据透明度和调试能力。 这项研究确定了三种有前景的解决方案：使用 APSW 库、通过 ctypes 访问 SQLite C 函数 `sqlite3_column_table_name()`，以及查询 `EXPLAIN` 命令的输出。

rss · Simon Willison · 6月13日 23:05

**背景**: 通用表表达式（CTE）是 SQLite 中的临时结果集，可以简化复杂查询并提高可读性。SQLite 提供内部元数据 API 来跟踪列的来源，尽管标准 `sqlite3` 模块默认不暴露此信息。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/13/sqlite-column-provenance/">Research: Mapping SQLite result columns back to their source ...</a></li>
<li><a href="https://sqlite.org/c3ref/column_database_name.html">Source Of Data In A Query Result - SQLite</a></li>
<li><a href="https://www.sqlitetutorial.net/sqlite-cte/">SQLite CTE</a></li>

</ul>
</details>

**标签**: `#sqlite`, `#sql`, `#datasette`, `#ai-research`, `#data-tools`

---

<a id="item-10"></a>
## [选择异常检测还是分类来识别癌症模拟物](https://www.reddit.com/r/MachineLearning/comments/1u4obgy/anomaly_detection_vs_classification_for_visually/) ⭐️ 8.0/10

一位研究人员在 Reddit 上寻求建议，询问在医学成像背景下，是应该使用异常检测还是监督分类来区分特定类型的癌症与视觉上相似的模拟物。 这个问题解决了医学成像中的一个关键挑战，其中类别不平衡和特征重叠使得标准分类变得困难，可能会影响诊断工具的可靠性。 用户指出负样本在视觉和形态上与目标癌症非常相似，这创造了一个区分异常与“正常”分布的复杂场景。

reddit · r/MachineLearning · /u/DryHat3296 · 6月13日 11:18

**背景**: 异常检测侧重于识别那些不符合正常数据预期模式的稀有“分布外”样本，而分类是一种监督学习任务，用于将观察结果归类到预定义的类别中。在医学成像中，异常检测对于识别像癌症这样的稀有病理特别相关，因为它通常比传统分类方法更好地处理不平衡的数据集。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@ljyds/differences-between-classification-and-anomaly-detection-f0b4b4b990e2">Differences between Classification and Anomaly Detection A Comprehensive Investigation of Anomaly Detection Methods in ... Anomaly Detection Using Computer Vision: A Comparative ... What are the key differences between anomaly detection and ... Difference between Anomaly detection and classification</a></li>
<li><a href="https://arxiv.org/abs/2507.23411">[2507.23411] Out-of-Distribution Detection in Medical Imaging ... Images Enhancing Medical Imaging Out-of-Distribution Detection with ... Diffusion models for out-of-distribution detection in digital ... Enhancing Medical Imaging Out-of-Distribution Detection with ... DIsoN: Decentralized Isolation Networks for Out-of ... Limitations of Out-of-Distribution Detection in 3D Medical ... MedOODFlow: Out-of-Distribution Detection in Medical Imaging ...</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S1532046424001692">Early multi-cancer detection through deep learning: An ...</a></li>

</ul>
</details>

**标签**: `#anomaly-detection`, `#medical-imaging`, `#classification`, `#deep-learning`, `#research`

---

<a id="item-11"></a>
## [对“完美”60fps UI 动画的批评](https://tonsky.me/blog/every-frame-perfect/) ⭐️ 7.0/10

一篇题为《Every Frame Perfect》的技术博客文章批评了现代 UI 动画趋势，认为追求完美的 60fps 帧率往往会导致混乱和令人困惑的界面。 这场辩论意义重大，因为它挑战了行业优先考虑流畅 60fps 动画的行业标准，突显了人机交互（HCI）中视觉流畅性与用户清晰度之间的权衡。 作者认为，单独的“完美”帧在视觉上可能会令人困惑，而社区讨论则表明，实时渲染利用了人眼视觉系统的特性，可能需要不完美的帧来匹配感知。

hackernews · ravenical · 6月13日 11:40 · [社区讨论](https://news.ycombinator.com/item?id=48516251)

**背景**: 现代 UI 设计通常优先考虑 60fps 动画，以创造速度感和响应性，这一概念植根于人机交互（HCI）研究中，该研究关注用户如何感知和与计算机系统交互。虽然高帧率通常与更好的质量相关联，但本文质疑在运动设计中追求数学上的完美是否会损害可用性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/Performance/Guides/Animation_performance_and_frame_rate">Animation performance and frame rate - MDN Web Docs</a></li>
<li><a href="https://lucky.graphics/learn/web-animation-performance-guide/">Web Animation Performance: The Complete Guide to 60fps UI ...</a></li>

</ul>
</details>

**社区讨论**: 社区成员大多同意某些例子是糟糕的动画，但不同意“完美”帧总是负面的前提，他们认为实时渲染利用了人眼视觉系统的特性，且“错误”的帧在特定语境下可能是视觉效果最好的。

**标签**: `#UI/UX`, `#Animation`, `#Human-Computer Interaction`, `#Computer Graphics`

---

<a id="item-12"></a>
## [罕见的 Game Boy WorkBoy 生产力配件被发掘](https://tcrf.net/Workboy) ⭐️ 7.0/10

一款罕见的未发布 Game Boy WorkBoy 原型机已被发掘并展示，这款设备可以将掌机转变为微型工作站。 这一发现凸显了 Game Boy 生态系统外围设备的丰富创新历史，并提供了对早期掌上生产力概念的怀旧一瞥。 WorkBoy 是一款 PDA 风格的配件，配备键盘和 12 个预装应用，允许用户管理日程、地址，并在五种语言之间进行转换。

hackernews · tosh · 6月13日 17:43 · [社区讨论](https://news.ycombinator.com/item?id=48519552)

**背景**: Game Boy 是任天堂于 1989 年推出的开创性掌机，它普及了掌上游戏并建立了一个巨大的全球市场。后来发布的 Game Boy 相机和打印机等配件扩展了系统的功能，使其不仅能玩游戏。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.syfy.com/syfy-wire/unreleased-nintendo-game-boy-accessory-work-boy-found">Nintendo Game Boy 'WorkBoy' productivity accessory rediscovered after decades - SYFY</a></li>
<li><a href="https://tcrf.net/Workboy">Workboy - The Cutting Room Floor - TCRF</a></li>

</ul>
</details>

**社区讨论**: 社区成员对设备作为现代智能手机替代品的潜力表示感兴趣，有用户指出 Playdate 掌机在非游戏应用方面具有巨大潜力。

**标签**: `#Retro Computing`, `#Hardware`, `#GameBoy`, `#Productivity`, `#Niche History`

---

<a id="item-13"></a>
## [作者构建免费双语机器学习笔记本课程，寻求社区反馈](https://www.reddit.com/r/MachineLearning/comments/1u4zbld/im_building_a_free_bilingual_machinelearning/) ⭐️ 7.0/10

作者在 GitHub 上发布了一个开源的机器学习教程仓库，采用 Jupyter Notebook 格式，并提供英语和波斯语/法语的并行版本。 这一举措通过为机器学习社区中非英语母语的学习者提供易于获取的实践资源，解决了特定的教育缺口。 课程涵盖了广泛的主题，包括数据清洗、特征工程、回归、分类、树模型、集成学习、聚类、降维、评估、时间序列、异常检测、负责任的机器学习和 MLOps 概念。

reddit · r/MachineLearning · /u/abolfazl1363 · 6月13日 19:07

**背景**: Jupyter Notebook 为开发基于 Python 的数据科学应用程序提供了交互式计算环境，使其成为循序渐进的机器学习教程的理想选择。MLOps 是一组将模型开发、基础设施和实际使用连接到持续工作流的实践，以确保机器学习系统保持可靠和可扩展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tutorialspoint.com/machine_learning_with_python/machine_learning_with_python_jupyter_notebook.htm">Machine Learning - Jupyter Notebook - Online Tutorials Library</a></li>
<li><a href="https://www.geeksforgeeks.org/machine-learning/mlops-tutorial/">MLOps Tutorial - GeeksforGeeks</a></li>
<li><a href="https://www.mdpi.com/2673-2688/6/10/257">Data Preprocessing and Feature Engineering for Data Mining ...</a></li>

</ul>
</details>

**标签**: `#education`, `#open-source`, `#bilingual`, `#curriculum`, `#machine-learning`

---