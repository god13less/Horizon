---
layout: default
title: "Horizon Summary: 2026-06-30 (ZH)"
date: 2026-06-30
lang: zh
---

> 从 20 条内容中筛选出 17 条重要资讯。

---

1. [Claude Code 在请求中嵌入隐藏标记](#item-1) ⭐️ 8.0/10
2. [PostgreSQL 19 路线图与功能揭晓](#item-2) ⭐️ 8.0/10
3. [欧盟数字身份证钱包依赖谷歌和苹果](#item-3) ⭐️ 8.0/10
4. [美国劳动收入份额降至二战后最低水平](#item-4) ⭐️ 8.0/10
5. [shot-scraper 1.10 添加视频分镜功能](#item-5) ⭐️ 8.0/10
6. [交互式地图按语义相似性可视化 1100 万篇研究论文](#item-6) ⭐️ 8.0/10
7. [经典金融狂热与群体心理分析（1852 年）](#item-7) ⭐️ 7.0/10
8. [中等强度与高强度运动对老年人体成分的影响](#item-8) ⭐️ 7.0/10
9. [Astral-sh/uv 0.11.26 发布，包含性能优化](#item-9) ⭐️ 6.0/10
10. [弗吉尼亚县因数据中心成本要求学校节约用电](#item-10) ⭐️ 6.0/10
11. [Knoppix：开创性的 Live CD Linux 发行版](#item-11) ⭐️ 6.0/10
12. [Simon Willison 分享了“AI 指南针”测验](#item-12) ⭐️ 6.0/10
13. [Simon Willison 发布 HTML 表格提取工具](#item-13) ⭐️ 6.0/10
14. [CVIL 检查清单新增分割、OCR 和 VLM 专题](#item-14) ⭐️ 6.0/10
15. [EACL 2027 引入分阶段同行评审流程](#item-15) ⭐️ 6.0/10
16. [分析表示学习中的 MLE 与 NCE 损失函数](#item-16) ⭐️ 6.0/10
17. [关于修改被拒 MICCAI 论文的建议](#item-17) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Claude Code 在请求中嵌入隐藏标记](https://thereallo.dev/blog/claude-code-prompt-steganography) ⭐️ 8.0/10

安全研究人员发现 Claude Code 在其系统提示词中嵌入隐写标记，以识别用户并执行使用策略，特别是根据用户的时区修改“今天是……”这一行。 这一发现凸显了流行 AI 编程助手用户的重大隐私和安全问题，引发了关于隐蔽追踪的伦理问题以及其他专有 AI 工具可能存在类似做法的讨论。 这些标记是通过微妙地更改系统提示词中的日期格式来实现的；例如，中国用户看到的日期格式可能与来自其他地区的用户不同，这可以通过逆向工程 API 来检测。

hackernews · kirushik · 6月30日 15:44 · [社区讨论](https://news.ycombinator.com/item?id=48734373)

**背景**: 隐写术是将信息隐藏在另一个文件、消息、图像或视频中以避免被发现的做法。在 AI 语境下，这通常用于水印或追踪，尽管这引发了关于用户隐私的伦理问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cybersecuritynews.com/anthropic-claude-hidden-code/">Anthropic's Claude Code Reportedly Uses Hidden Code to Detect Chinese Users</a></li>
<li><a href="https://github.com/CMLKevin/ClaudeCode_ARGBuster">GitHub - CMLKevin/ClaudeCode_ARGBuster: Advanced ARG investigation ...</a></li>

</ul>
</details>

**社区讨论**: 用户对实现的笨拙感到惊讶，争论该技术是否属于安全不可知论，并将 Claude Code 与 Codex CLI 等开源替代品进行了不利比较，后者不太可能使用这种隐蔽方法。

**标签**: `#security`, `#privacy`, `#AI`, `#steganography`, `#anthropic`

---

<a id="item-2"></a>
## [PostgreSQL 19 路线图与功能揭晓](https://www.snowflake.com/en/blog/engineering/postgresql-19-features-beta/) ⭐️ 8.0/10

Snowflake 的工程博客概述了即将到来的 PostgreSQL 19 路线图，重点介绍了 JIT 编译、压缩和逻辑复制方面的改进，同时指出已移除 RADIUS 认证。 这一路线图意义重大，因为它解决了关键的性能瓶颈和架构限制，可能会延长 PostgreSQL 对企业工作负载和大规模分析任务的适用性。 关键的技术更新包括 toast 压缩默认为 lz4，移除 RADIUS 认证，以及基于 SQL:2011 标准引入原生应用时间时态数据支持。

hackernews · thinkingemote · 6月30日 14:14 · [社区讨论](https://news.ycombinator.com/item?id=48733031)

**背景**: PostgreSQL 是一种强大、开源的对象关系数据库系统，以其可靠性和功能集而闻名。该项目是一个非商业、全志愿的努力，开发版本如 19 目前处于 beta 阶段，计划于 2026 年底发布。社区经常讨论架构限制，例如基于行的存储模型和单节点约束，这可能会阻碍在非常大的数据集上的性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/developer/roadmap/">PostgreSQL: Roadmap</a></li>
<li><a href="https://www.postgresql.org/about/news/postgresql-19-beta-1-released-3313/">PostgreSQL: PostgreSQL 19 Beta 1 Released!</a></li>

</ul>
</details>

**社区讨论**: 社区辩论集中在连接管理上，用户对每个连接的高内存占用表示担忧，并认为缺乏原生列式存储来处理大数据分析，这需要复杂的扩展。

**标签**: `#PostgreSQL`, `#Database`, `#SQL`, `#Software Engineering`, `#Database Systems`

---

<a id="item-3"></a>
## [欧盟数字身份证钱包依赖谷歌和苹果](https://waag.org/en/article/european-digital-id-wallets-are-gift-google-and-apple/) ⭐️ 8.0/10

一项关键分析显示，欧盟新的数字身份证钱包实际上被迫依赖谷歌和苹果的服务，这与数字主权的目标背道而驰。 这种依赖引发了关于数字主权和隐私的严重担忧，因为它迫使欧洲公民依赖美国科技巨头的关键基础设施。 钱包的欧盟参考规范严格要求使用谷歌 Play 服务，这意味着像意大利的 IO 应用这样的程序无法在 GrapheneOS 或其他非谷歌安卓实现上运行。

hackernews · donohoe · 6月30日 10:36 · [社区讨论](https://news.ycombinator.com/item?id=48730729)

**背景**: 欧盟数字身份证钱包是由法规 (EU) 2024/1183 创建的安全平台，旨在让公民能够在成员国之间存储和验证身份。数字主权是指国家对其依赖的数字基础设施、数据和软件拥有实质性控制权的概念。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/EU_Digital_Identity_Wallet">EU Digital Identity Wallet - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Digital_sovereignty">Digital sovereignty</a></li>
<li><a href="https://en.wikipedia.org/wiki/Google_Play_Services">Google Play Services</a></li>

</ul>
</details>

**社区讨论**: 评论者认为法规创造了垄断，要求使用谷歌 Play 服务是对数字自主权的攻击，有些人认为只有通过诉讼才能带来改变。

**标签**: `#digital-sovereignty`, `#privacy`, `#regulation`, `#eu`, `#android`

---

<a id="item-4"></a>
## [美国劳动收入份额降至二战后最低水平](https://libertystreeteconomics.newyorkfed.org/2026/06/the-post-covid-decline-in-the-labor-share/) ⭐️ 8.0/10

美联储的分析显示，美国的劳动收入份额已降至二战后的最低水平，自 2000 年以来出现了明显的结构性下降。 这一趋势对软件行业和更广泛的经济具有重要意义，因为它表明经济收益的分配方式发生了变化，可能会影响工资增长和劳动力市场动态。 虽然最近的新冠疫情后下降符合历史周期性模式，但自 2000 年以来的长期下降代表了一种独特的结构性转变，而非临时波动。

hackernews · loughnane · 6月30日 15:35 · [社区讨论](https://news.ycombinator.com/item?id=48734234)

**背景**: 劳动收入份额是指作为工资和福利支付给工人的国民总收入部分，而非资本所有者的利润。劳动收入份额的下降表明经济增长越来越归因于资本而非劳动。

**社区讨论**: 评论者大多同意文章标题具有耸动性，指出美联储未发现与过去 episodes 有明显不同的证据，尽管有些人担心长期趋势可能会继续。

**标签**: `#economics`, `#labor-market`, `#policy`, `#data-analysis`, `#federal-reserve`

---

<a id="item-5"></a>
## [shot-scraper 1.10 添加视频分镜功能](https://simonwillison.net/2026/Jun/30/shot-scraper/#atom-everything) ⭐️ 8.0/10

shot-scraper 1.10 版本引入了新的 `shot-scraper video` 命令，该命令接受一个 `storyboard.yml` 文件来定义针对 Web 应用的例行程序，并使用 Playwright 录制这些例程的视频。 该功能对 AI 代理和自动化工作流具有重要意义，因为它使编码代理能够直观地展示其工作成果，提供了一种证明代码按预期工作的方法。 该工具使用 YAML 配置文件来定义服务器、URL、视口尺寸和要执行的 JavaScript 操作，并支持通过 JSON 文件进行基于 Cookie 的身份验证。

rss · Simon Willison · 6月30日 15:10

**背景**: shot-scraper 是一个用于对网页进行截图和生成 PDF 的 Python 工具，它以前曾用于测试 Web 应用。这个新的视频功能扩展了其功能，以支持自动化录制用户工作流。

**标签**: `#web-scraping`, `#automation`, `#video`, `#tools`, `#python`

---

<a id="item-6"></a>
## [交互式地图按语义相似性可视化 1100 万篇研究论文](https://www.reddit.com/r/MachineLearning/comments/1ujn3u5/a_map_of_the_latest_11_million_papers_split_by/) ⭐️ 8.0/10

发布了一款新的交互式 2D 地图，通过将最新的 1100 万篇研究论文按语义聚类和时间切片进行可视化。 该工具通过提供每日研究趋势的宏观视角，解决了科学文献中信息过载的关键挑战，使研究人员更容易追踪其领域的演变。 该可视化使用 SPECTER 2 嵌入进行编码，使用 UMAP 进行降维，并使用 Voronoi 镶嵌对高密度峰值进行标记，同时支持关键词和语义查询，并从 OpenAlex 和 Arxiv 进行每日自动摄取。

reddit · r/MachineLearning · /u/icannotchangethename · 6月30日 11:55

**背景**: 科学文献呈指数级增长，使得研究人员很难跟上最新论文的步伐。OpenAlex 等工具提供了海量的研究元数据数据集，而 SPECTER 2 是一种基于 transformer 的模型，用于生成嵌入向量以表示科学文本的语义含义。

**标签**: `#visualization`, `#scientific-literature`, `#machine-learning`, `#research`, `#openalex`

---

<a id="item-7"></a>
## [经典金融狂热与群体心理分析（1852 年）](https://www.gutenberg.org/ebooks/24518) ⭐️ 7.0/10

查尔斯·麦凯的经典著作《非凡的普遍错觉与群体的疯狂》已在古腾堡计划上发布为免费电子书，使现代读者能够接触到这部 19 世纪对历史金融泡沫的分析。 这本书是行为经济学和群体心理学的奠基之作，为理解非理性和羊群行为如何驱动市场狂热提供了永恒的见解。 书中详细描述了南海泡沫和郁金香狂热等历史事件，尽管现代历史学家指出麦凯有时会夸大或渲染这些事件的规模。

hackernews · lstodd · 6月30日 12:47 · [社区讨论](https://news.ycombinator.com/item?id=48731989)

**背景**: 苏格兰记者查尔斯·麦凯于 1852 年撰写了这本书，书中探讨了群体心理如何导致金融泡沫和社会狂热，如荷兰郁金香狂热和密西西比泡沫。

**社区讨论**: 读者们称赞这本书引人入胜的故事讲述及其对理解人类非理性的影响，尽管有些评论指出关于郁金香狂热规模的部分可能并不完全符合历史事实。

**标签**: `#behavioral-economics`, `#psychology`, `#history`, `#finance`, `#crowd-psychology`

---

<a id="item-8"></a>
## [中等强度与高强度运动对老年人体成分的影响](https://www.maturitas.org/article/S0378-5122(25)00571-7/fulltext) ⭐️ 7.0/10

一项涉及 123 名健康老年人的临床研究发现，中等强度跑步机训练和高强度间歇训练（HIIT）在六个月内均显著改善了身体成分。 这项研究意义重大，因为它提供了证据表明老年人可以安全地从高强度训练中受益，与传统中等强度运动相比，这为老年人群提供了更高效的健身解决方案。 参与者每周完成三次 45 分钟的监督训练，HIIT 训练包括 4 分钟 85-95%心率区间和 3 分钟 60-70%心率区间的间歇，同时使用双能 X 线吸收法测量身体成分。

hackernews · bookofjoe · 6月30日 10:31 · [社区讨论](https://news.ycombinator.com/item?id=48730694)

**社区讨论**: 社区评论指出，该研究侧重于有氧训练而非阻力训练，一些用户分享了高强度运动的风险轶事，例如患房颤，而另一些人则提到了新手效应，即未经训练的人在初期会看到快速改善。

**标签**: `#health`, `#exercise`, `#gerontology`, `#fitness`, `#science`

---

<a id="item-9"></a>
## [Astral-sh/uv 0.11.26 发布，包含性能优化](https://github.com/astral-sh/uv/releases/tag/0.11.26) ⭐️ 6.0/10

Astral-sh/uv 版本 0.11.26 于 2026 年 6 月 30 日发布，包含针对依赖解析的性能优化，以及一项新警告，用于防止构建缓存被放置在源代码目录内。 这些性能改进使依赖解析更快、更高效，这对于管理复杂项目或大规模 CI/CD 流水线的 Python 开发者至关重要。 此次发布包含四项具体的性能增强：适配仅 ID 的 PubGrub 依赖、避免在 `ForkMap::contains` 中分配内存、跨迭代重用解析器工作，以及加快不相交范围的候选选择速度。

github · github-actions[bot] · 6月30日 14:53

**背景**: uv 是一个用 Rust 编写的高性能 Python 包安装器和解析器，旨在通过提供显著更快的依赖解析和安装速度来取代 pip 和 pip-tools 等传统工具。

**标签**: `#Python`, `#Dependency Management`, `#Performance`, `#uv`

---

<a id="item-10"></a>
## [弗吉尼亚县因数据中心成本要求学校节约用电](https://www.404media.co/henrico-virginia-datacenter-energy-cost-email/) ⭐️ 6.0/10

弗吉尼亚州的亨里科县给当地学校发邮件，要求它们节约用电，原因是受数据中心扩张和可再生能源指令的影响，能源成本高昂。 这种情况凸显了数据中心快速扩张和向可再生能源过渡带来的财政挑战，以及其对当地电力基础设施造成的日益增长的负担。 高昂的成本主要归因于 2020 年通过的弗吉尼亚清洁经济法案，该法案强制要求电力公司 Dominion 到 2045 年实现 100%可再生能源转型。

hackernews · 01-_- · 6月30日 16:05 · [社区讨论](https://news.ycombinator.com/item?id=48734699)

**背景**: 亨里科县拥有 37 个数据中心，使其成为数字基础设施的重要枢纽。当地电力公司 Dominion 目前正在大力投资建设尚未投入使用的可再生能源项目。

**社区讨论**: 社区评论争论了弗吉尼亚清洁经济法案的利弊，一些人认为短期成本对于长期可持续性是必要的，而另一些人则批评科技公司的所谓贪婪。

**标签**: `#data-centers`, `#energy`, `#infrastructure`, `#sustainability`, `#Virginia`

---

<a id="item-11"></a>
## [Knoppix：开创性的 Live CD Linux 发行版](https://www.knopper.net/knoppix/index-en.html) ⭐️ 6.0/10

Knoppix 正被怀旧地视为一个里程碑，因为它开创了 Live CD Linux 发行版的先河，允许用户从光盘运行完整的操作系统而无需安装。 这一回顾强调了 Knoppix 在普及 Debian 和 KDE 访问方面的历史意义，为现代便携式操作系统铺平了道路，并影响了更广泛的开源生态系统。 Knoppix 基于 Debian，当时 Debian 的安装以困难著称，并且使用了 KDE 桌面环境来提供用户友好的体验。

hackernews · hoangvmpc · 6月30日 12:54 · [社区讨论](https://news.ycombinator.com/item?id=48732056)

**背景**: Debian 是由志愿者开发的一个通用免费操作系统，也是仍在开发中最古老的 Linux 发行版。它作为许多其他发行版（如 Ubuntu）的基础，以其稳定性和长期支持而闻名。KDE 桌面环境是一个流行的开源桌面环境，为类 Unix 操作系统提供图形用户界面。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Debian_Linux">Debian Linux</a></li>
<li><a href="https://en.wikipedia.org/wiki/KDE_Desktop_Environment">KDE Desktop Environment</a></li>

</ul>
</details>

**社区讨论**: 社区成员分享了使用 Knoppix 在学校计算机实验室学习编程以及在禁止双系统的家庭 PC 上实验 Linux 的美好回忆。

**标签**: `#Linux`, `#Open Source`, `#History`, `#Debian`, `#KDE`

---

<a id="item-12"></a>
## [Simon Willison 分享了“AI 指南针”测验](https://simonwillison.net/2026/Jun/30/the-ai-compass/#atom-everything) ⭐️ 6.0/10

Simon Willison 正在展示“AI 指南针”，这是一个由 bambamramfan 创建的 29 道题测验，根据用户对 AI 的伦理和技术观点将其归类为 30 种不同的 AI 原型。 这个测验提供了一种新颖且引人入胜的方式来可视化并讨论 AI 社区中多样化的观点，作为一个有趣的对话开场白，而不是严肃的技术分析。 该测验作为一个单页 React 应用程序实现，使用 <code>&lt;script type="text/babel"&gt;</code> 技巧在没有构建步骤的情况下运行，源代码可在 GitHub 上获取。

rss · Simon Willison · 6月30日 17:39

**背景**: 政治指南针是一个二维图表，用于根据经济和社会轴将政治观点归类为象限。本新闻将这一概念改编到了 AI 领域，使用“好”与“坏”以及“过度炒作”与“变革性”等轴来映射不同的 AI 哲学。

**标签**: `#AI`, `#Quiz`, `#Ethics`, `#Community`, `#Simon Willison`

---

<a id="item-13"></a>
## [Simon Willison 发布 HTML 表格提取工具](https://simonwillison.net/2026/Jun/29/html-table-extractor/#atom-everything) ⭐️ 6.0/10

Simon Willison 发布了一款新工具，该工具可以接受粘贴的包含 HTML 表格的富文本，并将其转换为 HTML、Markdown、CSV、TSV 或 JSON 格式。 该工具简化了数据提取和转换的工作流程，使用户无需编写复杂的脚本即可轻松处理来自网页的表格数据。 该工具通过开放的 CORS API 支持自动提取 Wikipedia 表格，用户界面允许使用选项卡在 TSV 和 JSON 等不同输出格式之间切换。

rss · Simon Willison · 6月29日 23:38

**背景**: TSV（制表符分隔值）是一种简单的文件格式，用于存储表格数据，其中每一行代表一行，每一列由制表符分隔。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/TSV_Fortuna_Sachsenross">TSV Fortuna Sachsenross</a></li>

</ul>
</details>

**标签**: `#web scraping`, `#data extraction`, `#productivity`, `#tools`, `#utilities`

---

<a id="item-14"></a>
## [CVIL 检查清单新增分割、OCR 和 VLM 专题](https://www.reddit.com/r/MachineLearning/comments/1ujlmy2/update_on_cvil_the_free_cv_interview_prep/) ⭐️ 6.0/10

开源项目 CVIL 的作者更新了其免费的面试准备检查清单，新增了三个专题：分割、OCR 和 VLM，并保留了现有的 ReID 和部署专题。 此次更新通过提供结构化的、针对特定角色的学习路径，解决了计算机视觉就业市场不断变化的需求，帮助候选人更有效地准备现代技术面试。 该项目托管在 GitHub 上，欢迎社区贡献，并开放了 3D 视觉和姿态估计等专题，作者鼓励用户提交反馈或拉取请求，如果发现内容过时。

reddit · r/MachineLearning · /u/PolarIceBear_ · 6月30日 10:40

**背景**: CVIL 是由机器学习爱好者创建的实用资源，旨在梳理计算机视觉和机器学习面试所需的关键主题，超越了教科书理论，专注于获得实习机会所需的特定阶段和专题。

**标签**: `#computer-vision`, `#interview-prep`, `#resources`, `#open-source`, `#machine-learning`

---

<a id="item-15"></a>
## [EACL 2027 引入分阶段同行评审流程](https://www.reddit.com/r/MachineLearning/comments/1ujj63g/eacl_2027_author_response_and_authorreviewer/) ⭐️ 6.0/10

EACL 2027 将作者回复和作者与评审人讨论分为两个独立阶段，并延长了截止日期。 这一变化通过缓解评审周期中作者和评审人的时间压力，解决了学术出版中的一个常见瓶颈。 新安排将作者回复时间分配为 5 天（2026 年 9 月 14 日至 19 日），评审参与和讨论时间为 5 天（2026 年 9 月 20 日至 24 日），而以前总共只有 5 天。

reddit · r/MachineLearning · /u/S4M22 · 6月30日 08:16

**社区讨论**: 发帖者对这一变化表示强烈赞同，指出之前的紧张日程往往迫使作者在讨论期间进行新的实验，但这并非讨论的初衷。

**标签**: `#EACL`, `#Academic Publishing`, `#Peer Review`, `#NLP`, `#Conference Updates`

---

<a id="item-16"></a>
## [分析表示学习中的 MLE 与 NCE 损失函数](https://www.reddit.com/r/MachineLearning/comments/1uj8nse/loss_functions_in_instance_representation/) ⭐️ 6.0/10

该帖子讨论了使用最大似然估计（MLE）进行实例表示学习时的计算挑战，并建议使用噪声对比估计（NCE）作为替代方案。 该主题对从事表示学习的研究人员和从业者具有重要意义，因为选择正确的损失函数对于平衡计算可行性和模型偏差至关重要。 作者指出，虽然 NCE 近似了困难的损失函数，但它仍然需要估计分母，从而引发了关于直接在 MLE 公式中近似分母是否是更好方法的讨论。

reddit · r/MachineLearning · /u/No_Balance_9777 · 6月29日 23:34

**背景**: 在表示学习中，当处理大型数据集（例如包含大量图像的数据集）时，最大似然估计（MLE）往往变得计算上不可行。噪声对比估计（NCE）是一种用于近似难以计算的似然函数的技术，它将问题视为二分类任务。

**社区讨论**: 用户询问了关于估计分母时的偏差问题，并对其在 NCE 密度估计公式与在此背景下作为损失函数使用之间的联系感到困惑。

**标签**: `#Machine Learning`, `#Deep Learning`, `#Representation Learning`, `#Loss Functions`, `#NCE`

---

<a id="item-17"></a>
## [关于修改被拒 MICCAI 论文的建议](https://www.reddit.com/r/MachineLearning/comments/1uj35gh/rejected_miccai_paper_workshop_journalconference/) ⭐️ 6.0/10

一名初级研究人员寻求社区建议，关于如何修改一篇被拒的可解释性论文的最佳策略，具体权衡了研讨会投稿与直接期刊投稿的利弊。 此次讨论对学术界具有重要意义，因为它解决了初级研究人员面临的常见出版挑战，并提供了关于不同出版流程利弊的可操作见解。 该论文专注于机器学习中的可解释性，被 MICCAI 拒稿，作者在改进模型大小和实验时间后，正在考虑 MLCN/iMIMIC 等研讨会或直接期刊投稿。

reddit · r/MachineLearning · /u/KingPowa · 6月29日 19:58

**背景**: MICCAI 是医学图像计算和计算机辅助干预领域的顶级会议，研讨会通常作为初步结果在提交给主会议或期刊之前的垫脚石。

**标签**: `#Academic Publishing`, `#Machine Learning`, `#Career Advice`, `#MICCAI`

---