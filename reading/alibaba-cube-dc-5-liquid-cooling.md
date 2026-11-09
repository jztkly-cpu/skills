# 外刊精读｜Building the Cloud at Factory Speed
### 阿里云 CUBE DC 5.0 模块化液冷数据中心

> **文本说明**：本篇正文是**依据外刊报道改写的教学版文本**（adapted text），不是任何一篇原文的照搬。素材来自 *South China Morning Post*、*DatacenterDynamics*、*TechRadar Pro* 2024–2026 年对阿里云 CUBE DC 5.0 的报道（链接见文末）。文中数据均来自报道中阿里云的公开说法，课堂上可让学生对照原文阅读。
>
> **适用水平**：大学英语四六级 / 雅思 6.0–7.0 / CEFR B2–C1
> **建议课时**：2 课时（90 分钟）
> **话题标签**：科技 · AI 基础设施 · 能源效率 · 中国企业

---

## 一、导读与背景知识（Lead-in）

**读前讨论（5 分钟）**
1. Why do AI models need so much electricity? Where does all that energy go in the end?
2. If you had to build a large building in 100 days instead of two years, what would you change about the process?

**背景知识卡片**

| 概念 | 英文 | 一句话解释 |
|---|---|---|
| 数据中心 | data centre (英) / data center (美) | 集中放置服务器的大楼，为云计算和 AI 提供算力 |
| 机柜功率密度 | rack density | 一个机柜消耗的功率，单位 kW；普通服务器柜约 10–15 kW，AI 柜可达上百 kW |
| 冷板式液冷 | cold-plate liquid cooling | 把带冷却液的金属板直接贴在芯片上带走热量 |
| 浸没式液冷 | immersion cooling | 把整台服务器泡在不导电的冷却液里 |
| 风液混合 | wind-liquid hybrid cooling | 液冷负责大部分热量，风冷"兜底"剩余部分 |
| PUE | power usage effectiveness | 数据中心总耗电 ÷ IT 设备耗电，越接近 1.0 越节能 |
| 预制模块化 | prefabricated modular design | 在工厂里把部件做成标准模块，现场拼装 |

---

## 二、正文（Text）

# Building the Cloud at Factory Speed
**Inside Alibaba's bet on modular, liquid-cooled data centres**

**[1]** For most of the internet era, a data centre was something you built the way you would build an office tower: pour the foundations, raise the walls, and spend the better part of two years fitting it out. The artificial-intelligence boom has made that pace look glacial. Chips that cost tens of thousands of dollars apiece sit idle — or never get bought at all — until there is a building ready to power and cool them.

**[2]** Alibaba Cloud, China's largest cloud provider, thinks it has found a shortcut. Its CUBE DC 5.0 architecture, first unveiled at the company's Apsara Conference in 2024, treats a data centre less as a construction project than as a manufactured product. Power units, cooling systems and server halls are prefabricated in factories as standardised modules, then shipped to site and slotted together like oversized building blocks. In 2026 the company said the approach had cut delivery time for large AI facilities to roughly 100 days, and construction costs per kilowatt by about 10 per cent compared with its previous generation.

**[3]** Speed, however, is only half the story. The other half is heat. A rack of conventional servers might draw 10 to 15 kilowatts; racks packed with AI accelerators can draw ten times that, and air alone simply cannot carry the heat away fast enough. CUBE DC 5.0 therefore relies on what Alibaba calls "wind-liquid hybrid" cooling: liquid — most likely circulated through cold plates clamped directly onto the hottest chips — handles the bulk of the load, while air mops up the rest. Alibaba says a fully built-out site could support racks of up to 200 kW and as much as 200 megawatts of IT capacity.

**[4]** Efficiency is the payoff. Operators measure it with power usage effectiveness, or PUE: the ratio of the total energy a facility consumes to the energy that actually reaches the computers. A perfect score is 1.0. Alibaba's design targets reportedly put liquid-cooled halls at 1.10 or below, meaning that barely a tenth of the electricity is spent on overheads such as cooling and power conversion. The design also distributes power as direct current, sparing the losses that come from converting back and forth between AC and DC.

**[5]** There are reasons for caution. Most of the headline figures come from Alibaba itself and have not been independently verified. Liquid cooling brings headaches of its own, from leaks to the need for technicians with new skills. And prefabrication works best when demand is predictable — a tall order in an industry whose chip designs change every year or so.

**[6]** Still, the direction of travel is clear. Alibaba plans to more than double its global capacity for producing modular data centres this year, and rivals are making similar bets. If the AI race is partly a race to pour concrete, the winners may be those who work out how not to pour it at all.

*(≈ 470 words)*

---

## 三、段落精讲（Paragraph by Paragraph）

### 第 1 段｜提出问题：传统建法太慢
**段落功能**：用"盖写字楼"的类比引出矛盾——AI 芯片等不起漫长的建设周期。

**长难句拆解**
> *For most of the internet era, a data centre was something [you built **the way** you would build an office tower]: pour the foundations, raise the walls, and spend the better part of two years fitting it out.*

- 主干：**a data centre was something**
- `[you built the way …]`：定语从句修饰 something，省略了 that
- **the way + 从句** = in the way that…，"以……的方式"
- 冒号后三个并列动词短语 *pour / raise / spend* 具体展开"盖楼的方式"，节奏感强（三连排比 tricolon）
- **spend + 时间 + doing**：fitting it out 中 fit out = 装修、配备设施

> 译：在互联网时代的大部分时间里，建数据中心就像盖写字楼：打地基、砌墙，再花上近两年时间完成内部装配。

**词汇点**
- **the better part of** = 大半、几乎全部 → *the better part of two years* 将近两年
- **glacial** /ˈɡleɪʃl/ 冰川的 → 比喻"慢得像冰川移动"
- **apiece** 每个（放在数量词后）→ *cost $30,000 apiece*
- **sit idle** 闲置

---

### 第 2 段｜阿里的解法：把盖楼变成"造产品"
**段落功能**：介绍 CUBE DC 5.0 的核心理念与关键数据（100 天、成本降 10%）。

**长难句拆解**
> *Its CUBE DC 5.0 architecture, [first unveiled at the company's Apsara Conference in 2024], treats a data centre **less as** a construction project **than as** a manufactured product.*

- 主干：**architecture treats a data centre … as …**
- 插入语 `first unveiled …` 是过去分词短语作后置定语，补充背景
- **less as A than as B**：与其说是 A，不如说是 B（重心在 B）——外刊高频句型

> 译：其 CUBE DC 5.0 架构于 2024 年阿里云栖大会首次亮相，与其说把数据中心当作一项建筑工程，不如说当作一件工业制成品。

> *Power units, cooling systems and server halls **are prefabricated** in factories as standardised modules, **then shipped** to site and **slotted together** like oversized building blocks.*

- 三个被动谓语共用一个主语：are prefabricated → (are) shipped → (are) slotted，按时间顺序推进，第二、三个省略了 are
- **slot together** 卡扣式拼装（slot 本义"插槽"）

**词汇点**
- **unveil** 揭幕、首次公开（比 announce 更有"揭开面纱"的画面感）
- **prefabricate** 预制 → prefab（口语）
- **cut A to B / cut A by B**：to 表示"降到"，by 表示"降了"——本段两种都有，是很好的辨析素材

---

### 第 3 段｜核心难题：散热
**段落功能**：转折（*however*），点出第二个关键词 heat，引出液冷。

**长难句拆解**
> *CUBE DC 5.0 therefore relies on what Alibaba calls "wind-liquid hybrid" cooling: liquid — most likely circulated through cold plates clamped directly onto the hottest chips — handles the bulk of the load, while air mops up the rest.*

- **what Alibaba calls …**：所谓的……（作者与说法保持距离，表示这是公司用语）
- 冒号后主干：**liquid handles the bulk of the load, while air mops up the rest**
- 破折号之间是插入成分：*circulated through cold plates* 过去分词修饰 liquid；*clamped onto the hottest chips* 再修饰 cold plates —— 两层后置修饰
- **most likely** 表推测：原报道指出阿里没有完全公开冷却细节，作者用"多半是"体现严谨
- **while** 表对比，"而"

> 译：因此 CUBE DC 5.0 采用阿里所称的"风液混合"冷却：液体（多半是在直接贴合最热芯片的冷板中循环）承担大部分热负荷，而风冷负责处理剩下的部分。

**词汇点**
- **only half the story** 只是故事的一半 → 引出另一面的经典过渡语
- **draw (power)** 消耗（电力）
- **packed with** 塞满了
- **the bulk of** 大部分
- **mop up** 本义"用拖把擦干"，引申为"收拾残局、解决剩余部分"

---

### 第 4 段｜收益：能效（PUE）
**段落功能**：解释专业指标 PUE，展示外刊"术语 + 通俗解释"的写法。

**句型模仿点**
> *Operators measure it with power usage effectiveness, or PUE: the ratio of A to B.*

- **X, or Y**：这里的 or 是"即、也就是"，用于引出缩写或同义解释
- **the ratio of A to B**：A 与 B 之比

> *…meaning that barely a tenth of the electricity is spent on overheads…*

- **, meaning that …**：现在分词作结果状语，"这意味着……"，用来把数据翻译成读者听得懂的话
- **barely** 仅仅、勉强（带"少"的语气），对比 *nearly*

**数学小点**：PUE = 1.10 → 每 1.10 度电中有 0.10 度用于冷却等非 IT 开销，约占总量的 9%，所以说 "barely a tenth"。

**词汇点**
- **payoff** 回报、好处
- **overheads**（英式常用复数）间接开销
- **spare (sb/sth) sth** 使免于…… → *sparing the losses* 省去了损耗

---

### 第 5 段｜让步与质疑
**段落功能**：外刊"平衡报道"的标准动作——指出数据来源与潜在风险。

**亮点结构**：*There are reasons for caution.* 短句开头 → 三个理由依次展开：
1. 数据未经独立核实（*have not been independently verified*）
2. 液冷自身的麻烦（*headaches of its own, from A to B*）
3. 需求不确定（*a tall order*）

**词汇点**
- **headline figures** 宣传口径中最醒目的数据
- **from A to B** 列举范围："从……到……"
- **a tall order** 难以办到的事

---

### 第 6 段｜结论与升华
**段落功能**：*Still* 让步后回到主线，用"浇水泥"的隐喻收尾。

> *If the AI race is partly a race to pour concrete, the winners may be those who work out how **not to pour it at all**.*

- 首尾呼应：第 1 段的 *pour the foundations* ↔ 结尾的 *pour concrete*
- 反转式结尾（twist ending）：赢家不是浇得最快的，而是"根本不用浇"的（预制化）

**词汇点**
- **the direction of travel** 发展方向、大势（英式外刊高频）
- **make a bet on** 押注
- **work out** 想出、弄明白

---

## 四、核心词汇表（Vocabulary）

| # | 词汇 / 短语 | 词性 | 文中义 | 例句 / 搭配 |
|---|---|---|---|---|
| 1 | glacial | adj. | 极其缓慢的 | progress has been glacial |
| 2 | apiece | adv. | 每个 | They cost $5 apiece. |
| 3 | idle | adj. | 闲置的 | sit / lie idle |
| 4 | unveil | v. | 推出，揭幕 | unveil a new model |
| 5 | prefabricate | v. | 预制 | prefabricated homes |
| 6 | standardised | adj. | 标准化的 | standardised modules |
| 7 | slot together | phr. | 拼装在一起 | The parts slot together easily. |
| 8 | delivery time | n. | 交付周期 | cut delivery time by half |
| 9 | accelerator | n. | （AI）加速芯片 | AI accelerators such as GPUs |
| 10 | draw | v. | 消耗（电力） | draw 100 kW |
| 11 | circulate | v. | 循环 | coolant circulates through pipes |
| 12 | clamp | v. | 夹紧、固定 | clamp the plate onto the chip |
| 13 | the bulk of | phr. | 大部分 | the bulk of the work |
| 14 | mop up | phr. v. | 收拾剩余 | mop up remaining tasks |
| 15 | capacity | n. | 容量；产能 | IT capacity; production capacity |
| 16 | payoff | n. | 回报 | The payoff is lower bills. |
| 17 | overheads | n. | 间接成本 | cut overheads |
| 18 | verify | v. | 核实 | independently verified |
| 19 | a tall order | idiom | 难以做到的事 | Finishing in a week is a tall order. |
| 20 | direction of travel | phr. | 发展方向 | The direction of travel is clear. |

---

## 五、地道表达积累（Useful Expressions）

| 表达 | 含义 | 可迁移的写作场景 |
|---|---|---|
| the better part of + 时间 | ……的大部分 | 描述耗时：*the better part of a decade* |
| make sth look glacial | 让……显得极慢 | 对比新旧速度 |
| treat A less as B than as C | 与其说当作 B，不如说当作 C | 提出新视角 |
| X is only half the story. The other half is Y. | 引出另一面 | 议论文转折段首句 |
| what … calls "…" | 所谓的…… | 引用对方术语、保持中立 |
| , meaning that … | 这意味着…… | 解释数据含义 |
| There are reasons for caution. | 需要谨慎看待 | 议论文让步段 |
| headaches of its own | 自身的麻烦 | 指出新方案的副作用 |
| a tall order | 很难办到 | 评价目标难度 |
| Still, the direction of travel is clear. | 尽管如此，大势已明 | 结尾段首句 |

---

## 六、练习（Exercises）

### A. 阅读理解（Comprehension）
1. What problem does Paragraph 1 mainly describe?
   A. Data centres use too much water.
   B. Traditional construction is too slow for the AI boom.
   C. AI chips are too expensive to buy.
   D. Office towers are being turned into data centres.
2. The phrase "less as a construction project than as a manufactured product" suggests that Alibaba ______.
   A. has stopped building data centres
   B. approaches data centres in a factory-style, standardised way
   C. sells data centres to other companies
   D. builds data centres inside existing factories
3. According to Paragraph 3, why is liquid cooling necessary?
   A. Air cooling is too expensive.
   B. Liquid is easier to maintain.
   C. AI racks produce far more heat than air can remove quickly enough.
   D. Government rules require it.
4. A PUE of 1.10 means that ______.
   A. 110% of the energy reaches the computers
   B. about 10% of total energy goes to non-computing overheads
   C. the data centre is 10% faster
   D. the facility uses 1.1 megawatts
5. What is the writer's attitude towards Alibaba's claims?
   A. Completely sceptical  B. Uncritically enthusiastic  C. Cautiously positive  D. Indifferent

### B. 词汇填空（选词并用正确形式）
*glacial / the bulk of / a tall order / unveil / sit idle / payoff*

1. The company ______ its latest smartphone at a press event yesterday.
2. Without enough engineers, finishing the project by June is ______.
3. ______ the budget was spent on marketing.
4. Compared with online shopping, the old mail-order system now seems ______.
5. Thousands of machines ______ because the factory had no power.
6. The ______ for all that hard work was a promotion.

### C. 句型仿写
1. 用 **less as … than as …** 写一句话评价智能手机在当代生活中的角色。
2. 用 **… is only half the story. The other half is …** 写一句关于"考试分数"的句子。

### D. 汉译英（使用括号内表达）
1. 这座桥的建设花了将近十年时间。（the better part of）
2. 与其说这是一场技术竞赛，不如说是一场人才竞赛。（less as … than as …）
3. 电动汽车的普及也带来了自身的麻烦，从充电难到电池回收。（headaches of its own, from … to …）
4. 尽管如此，大势已经很清楚了。（the direction of travel）

### E. 讨论 & 写作（Speaking / Writing）
- **Discussion**: AI is often described as "software", yet this article is about concrete, pipes and electricity. What does this tell us about the real costs of AI?
- **Writing (150–200 words)**: *Should tech companies be required to publish independently verified energy-efficiency data for their data centres?* 要求至少使用本文 3 个地道表达。

---

## 七、参考答案（Key）

**A.** 1-B 2-B 3-C 4-B 5-C
（第 5 题依据：第 5 段 *There are reasons for caution* 体现保留，第 6 段 *the direction of travel is clear* 又给出肯定判断 → cautiously positive）

**B.** 1. unveiled 2. a tall order 3. The bulk of 4. glacial 5. sat idle 6. payoff

**C. 参考**
1. Today, a smartphone functions less as a phone than as a portable office.
2. A test score is only half the story. The other half is what a student can actually do with that knowledge.

**D. 参考**
1. Building the bridge took the better part of a decade.
2. This is less a race for technology than a race for talent.（也可：It should be seen less as a technology race than as a talent race.）
3. The spread of electric vehicles has brought headaches of its own, from a shortage of charging points to battery recycling.
4. Still, the direction of travel is clear.

---

## 八、素材来源（Sources）

- South China Morning Post — *Alibaba says modular design delivers AI data centres in 100 days, 10% lower cost*: https://www.scmp.com/tech/big-tech/article/3363637/alibaba-says-modular-design-delivers-ai-data-centres-100-days-10-lower-cost
- DatacenterDynamics — *Alibaba Cloud claims modular data center can halve build times*: https://www.datacenterdynamics.com/en/news/alibaba-cloud-claims-modular-data-center-can-halve-build-times
- TechRadar Pro — *Alibaba says it is ready for AI demand with new modular datacenter architecture*: https://techradar.com/pro/alibaba-says-its-is-ready-for-ai-demand-with-new-modular-datacenter-architecture
- Digital Today — *Alibaba cuts AI data centre build time to 100 days with modular CUBE 5.0*: https://www.digitaltoday.co.kr/en/view/92475/alibaba-cuts-ai-data-centre-build-time-to-100-days-with-modular-cube-5-0

> 教学提示：文中 "10–15 kW 的普通机柜" 为行业通用量级；"PUE ≤ 1.10" 为报道中的设计目标；"多半采用冷板" 是媒体推测（阿里未完全公开冷却细节）。可借此引导学生讨论外刊如何用 *reportedly / most likely / claims* 等词区分事实、说法和推测。
