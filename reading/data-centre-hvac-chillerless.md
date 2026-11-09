# 外刊精读（自学版）｜No Chillers, No Problem?
### 英伟达说"不需要冷水机组"，数据中心暖通真的要被淘汰了吗？

> **这份材料怎么用**：这是给你**自己学英语**用的精读，不是教案。讲解都直接对你说，重点放在两件事上：① 看懂并会用外刊里的句子；② 攒下一套能在工作里直接用的**数据中心暖通英文**（和外方厂商开会、看英文资料、写邮件都用得上）。
>
> **文本说明**：正文是**根据 2026 年多篇外刊和行业报道改写的学习版文本**，不是任何一篇原文的照搬（原文网站在当前环境里打不开）。事实和数据来自 NBC News、Facilities Dive、ACHR News、Data Center Frontier、Motivair 等的报道，链接在文末，建议学完后对照原文读一遍。
>
> **难度**：CEFR B2–C1（约六级 / 雅思 6.5–7）
> **建议用时**：每天 30–40 分钟，分 3 天学完（见文末学习计划）

---

## 〇、学前 3 分钟自测

先别看正文，试着用英文说出下面这些词。说不出来很正常，学完再回来测一遍。

冷水机组 · 压缩机 · 自然冷却 · 干冷器 · 供水温度 · 散热（向大气排热） · 冷板 · 冷量分配单元 · 余热回收 · 冗余

<details><summary>点开看答案</summary>

chiller · compressor · free cooling · dry cooler · supply water temperature · heat rejection · cold plate · coolant distribution unit (CDU) · waste-heat reuse / heat recovery · redundancy

</details>

---

## 一、背景：这篇文章在讲什么

2026 年 1 月，英伟达 CEO 黄仁勋在拉斯维加斯 CES 展会上说，下一代 **Vera Rubin** 系统用 **45°C 的水**来冷却，这个水温下数据中心**不需要冷水机组**。消息一出，Johnson Controls（江森自控）、Trane（特灵）等暖通巨头股价当天下跌 5%–7% 左右。

但工程师们很快指出：**不用冷机 ≠ 不用散热**。这篇文章讲的就是这场争论：高温水冷到底改变了什么、没改变什么、暖通行业的角色会怎么变。

对你来说，这篇文章的好处是：专业概念你很熟，所以可以把注意力全放在**英语怎么表达这些概念**上。

---

## 二、正文（Text）

# No Chillers, No Problem?
**Why hot-water cooling won't kill the HVAC plant**

**[1]** In early January, at the CES trade show in Las Vegas, Jensen Huang made a passing remark that sent a shiver through the heating, ventilation and air-conditioning (HVAC) industry. Nvidia's next-generation Vera Rubin systems, its chief executive explained, would be cooled with water at 45°C — and at that temperature, he said, a data centre does not need water chillers. Within hours, shares in Johnson Controls and Trane Technologies, two of the biggest makers of cooling equipment, had fallen by roughly 5–7%.

**[2]** Investors' logic was simple. In a conventional data centre, chillers are the workhorses of the cooling plant. They use compressors to strip heat out of a water loop so that it can be sent back to the data hall cold enough to cool the air around the servers. They are also among the most power-hungry machines in the building. If chips can tolerate water warmer than a summer's day in almost any city, the reasoning went, the compressor becomes redundant: outdoor air, blown across a dry cooler, can bring the water back down to temperature on its own. Engineers call this free cooling.

**[3]** Engineers were also quicker to spot the catch. "Chillerless" does not mean the heat disappears; every kilowatt that goes into a chip still has to be rejected to the atmosphere somewhere. Warm water merely changes how often the mechanical plant has to work — and that depends on the climate. A site in Norway may hardly ever need a compressor, while one in Phoenix or Singapore, where hot or humid weather narrows the gap between the water and the outdoor air, may still lean on chillers for weeks at a time. As Motivair, a cooling-equipment maker, argued, the real question is not whether chillers vanish but how they are integrated.

**[4]** Then there is the heat that the liquid never touches. Cold plates clamped onto processors capture most, but not all, of a rack's heat. Memory, power supplies and networking gear still shed heat into the air, and that residual load — anywhere from a tenth to a third of the total — must be handled by conventional air handlers fed with colder water. Meanwhile, much of the world's AI capacity is still being squeezed into existing buildings designed for air cooling, where operators cannot simply rip out the chiller plant. Hence the industry's new buzzword: hybrid. As one trade publication put it, the debate is no longer air versus liquid; it is about architecture.

**[5]** Reliability adds a further layer. Data centres are designed for the worst hour of the worst day, not for an average afternoon. An operator that has promised customers near-perfect uptime will think hard before betting everything on the weather. Many will keep at least some mechanical cooling as insurance — "trim" chillers that kick in only during heatwaves — even if they run for no more than a few hundred hours a year.

**[6]** None of this means the HVAC industry can relax. Its role is shifting from building giant chiller plants that run all year round to designing smarter systems — coolant distribution units, dry coolers, pumps and controls — that wring the most out of every degree of temperature difference. Warmer water also opens a door that was long closed: at 50°C or more, waste heat becomes warm enough to be worth selling, whether to district-heating networks or to nearby greenhouses. The chiller is not dead. But it is being demoted, from the heart of the cooling plant to its back-up.

*(≈ 560 words)*

---

## 三、逐段精读

> 每段按「这段在干嘛 → 难句拆开看 → 词汇和用法」三步走。建议先自己读一遍整段，能看懂多少算多少，再看讲解。

### 第 1 段｜事件：一句话让暖通股大跌

**这段在干嘛**：新闻导语。时间、地点、人物、事件、后果，一段交代完。

**难句拆开看**
> *Jensen Huang made a passing remark [that sent a shiver through the HVAC industry].*

- 主干：**Huang made a remark**
- `that sent a shiver through…` 定语从句，修饰 remark
- **send a shiver through sth** = 让……打了个寒颤。这里是双关：讲的是冷却行业，用"寒意"做比喻，外刊很爱这样玩

> *Nvidia's next-generation Vera Rubin systems, **its chief executive explained**, would be cooled with water at 45°C…*

- `its chief executive explained` 是插在句中的引述语。新闻常把"某某说"插到句子中间，读起来更自然。你写英文时也可以试：*The new plant, the contractor said, will be ready by June.*
- **would** 用于转述（过去将来），不是虚拟语气

**词汇和用法**
| 词 | 音标 | 意思 / 用法 |
|---|---|---|
| passing remark | /ˈpɑːsɪŋ rɪˈmɑːk/ | 随口一提的话 |
| shiver | /ˈʃɪvə(r)/ | 颤抖、寒意 |
| shares in X | | X 公司的股票（英式说法，美式多用 shares of） |
| fall by roughly 5–7% | | **by** 表示变化幅度。比较：fall **to** 50 = 降到 50 |

---

### 第 2 段｜投资者的逻辑：没有压缩机，冷机就多余了

**这段在干嘛**：解释为什么股价会跌，顺便给外行讲清楚冷机是干嘛的。这段的英文就是**用英语讲冷机原理**的标准范本，值得背下来。

**难句拆开看**
> *They use compressors to strip heat out of a water loop **so that** it can be sent back to the data hall cold enough to cool the air around the servers.*

- 主干：**They use compressors to strip heat out of a water loop**
- **so that + 从句**：目的，"以便"
- **cold enough to do**：足够冷，可以……（adj. + enough + to do，enough 放在形容词**后面**，这是中国学习者常犯的错）
- **strip A out of B**：从 B 中剥离 A。比 remove 更有画面感

> 译：冷机靠压缩机把热量从水环路里"剥离"出来，让水重新回到机房时足够冷，可以给服务器周围的空气降温。

> *If chips can tolerate water warmer than a summer's day in almost any city, **the reasoning went**, the compressor becomes redundant…*

- **the reasoning went** = 这套逻辑是这样的。同类表达：*the argument goes / the thinking goes*
- **redundant** 在这里是"多余的、被淘汰的"。⚠️ 但在数据中心语境里，**redundancy** 通常指"冗余备份"（N+1、2N）。同一个词两种意思，看上下文

**词汇和用法**
| 词 | 音标 | 意思 / 用法 |
|---|---|---|
| workhorse | /ˈwɜːkhɔːs/ | 主力、干重活的设备 |
| cooling plant | | 冷站、制冷机房 |
| power-hungry | | 耗电大的（*-hungry* 构词：data-hungry, cash-hungry） |
| tolerate | /ˈtɒləreɪt/ | 耐受（*tolerate higher inlet temperatures*） |
| dry cooler | | 干冷器（闭式、无蒸发） |
| bring sth back down to temperature | | 把……降回目标温度 |
| free cooling | | 自然冷却 |

---

### 第 3 段｜转折：热量不会消失

**这段在干嘛**：全文的核心论点。工程师的反驳：冷机少开 ≠ 不需要散热，而且取决于气候。

**难句拆开看**
> *Warm water merely changes **how often** the mechanical plant has to work — and **that** depends on the climate.*

- **how often…** 是宾语从句
- 破折号后的 **that** 指代前面的 *how often…*，用 that 承接上句，是很地道的衔接方法

> *A site in Norway may hardly ever need a compressor, **while** one in Phoenix or Singapore, [where hot or humid weather narrows the gap between the water and the outdoor air], may still lean on chillers for weeks at a time.*

- **while** 表对比："而"
- **one** = a site，避免重复
- `where…` 非限制性定语从句，解释原因
- **narrow the gap between A and B**：缩小 A 与 B 之差。这就是你们说的**温差 / 逼近度**变小。干冷器是看干球温度，冷却塔看湿球温度，所以文中说 *hot **or humid***

> *…the real question is **not whether** chillers vanish **but how** they are integrated.*

- **not whether A but how B**：问题不在于是否……而在于如何……（写邮件、做汇报都特别好用）

**词汇和用法**
| 词 | 音标 | 意思 / 用法 |
|---|---|---|
| spot the catch | | 看出问题、发现猫腻（catch = 隐藏的问题） |
| reject heat to the atmosphere | | 向大气排热（**heat rejection** 是暖通核心词） |
| mechanical plant / mechanical cooling | | 机械制冷（与 free cooling 相对） |
| hardly ever | | 几乎从不 |
| lean on | | 依靠 |
| for weeks at a time | | 一连好几周 |
| integrate | /ˈɪntɪɡreɪt/ | 整合、集成 |

---

### 第 4 段｜液冷管不到的那部分热

**这段在干嘛**：第二个反驳：冷板不能带走全部热量，加上存量风冷机房改不动，所以"混合"成了主流。

**难句拆开看**
> *Cold plates [clamped onto processors] capture **most, but not all,** of a rack's heat.*

- `clamped onto processors` 过去分词后置定语
- **most, but not all, of…**：大部分但不是全部。精确又简洁，写技术文档很好用

> *…and that residual load — anywhere from a tenth to a third of the total — must be handled by conventional air handlers fed with colder water.*

- **anywhere from A to B**：从 A 到 B 不等（表示范围）
- **air handlers fed with colder water**：由低温水供冷的空调末端。fed with 过去分词短语，"被供以……"
- 分数英文：a tenth = 1/10，a third = 1/3，two-thirds = 2/3

> *Hence the industry's new buzzword: hybrid.*

- **Hence + 名词短语**：没有谓语的省略句，"于是有了……"。正式书面语，开头用一下很有气势

**词汇和用法**
| 词 | 音标 | 意思 / 用法 |
|---|---|---|
| clamp | /klæmp/ | 夹紧、紧固 |
| shed heat | | 散出热量 |
| residual load | /rɪˈzɪdjuəl/ | 剩余负荷（这里指残余风冷负荷） |
| air handler / AHU / CRAH | | 空气处理机组 / 机房精密空调末端 |
| squeeze into | | 硬塞进 |
| rip out | | 拆除（口语，力度大） |
| buzzword | /ˈbʌzwɜːd/ | 时髦词、热词 |

---

### 第 5 段｜可靠性：按最坏情况设计

**这段在干嘛**：第三个反驳：数据中心按极端工况设计，所以会留"调峰冷机"做保险。

**难句拆开看**
> *Data centres are designed for **the worst hour of the worst day**, not for an average afternoon.*

- 一句话讲清**设计工况**的概念，可以直接借用
- 对比结构 **A, not B**

> *Many will keep at least some mechanical cooling as insurance — "trim" chillers that **kick in** only during heatwaves — **even if** they run for **no more than** a few hundred hours a year.*

- **trim chiller**：调峰冷机 / 补冷冷机，只在高温时补充冷量
- **kick in**：（设备）启动、开始起作用（口语，工程师常说）
- **even if**：即使（假设或让步）
- **no more than** = only，"不超过、仅仅"，强调少

**词汇和用法**
| 词 | 意思 / 用法 |
|---|---|
| uptime | 正常运行时间（*99.999% uptime*） |
| think hard before doing | 做……之前慎重考虑 |
| bet everything on | 把一切押在……上 |
| as insurance | 作为保险 |
| heatwave | 热浪 |

---

### 第 6 段｜结论：冷机没死，但被"降级"了

**这段在干嘛**：总结暖通行业角色的变化，再加一个新机会：余热回收。

**难句拆开看**
> *Its role is shifting **from** building giant chiller plants that run all year round **to** designing smarter systems — CDUs, dry coolers, pumps and controls — that wring the most out of every degree of temperature difference.*

- **shift from doing A to doing B**：从 A 转向 B
- 两个 that 从句分别修饰 plants 和 systems
- **wring the most out of**：榨取最大价值（wring 本义"拧干毛巾"）
- **every degree of temperature difference**：每一度温差

> *The chiller is not dead. But it is being demoted, from the heart of the cooling plant to its back-up.*

- 短句 + 短句，有力的结尾
- **demote** 降级、降职（反义词 promote）。拿人事上的词来说设备，是拟人化写法

**词汇和用法**
| 词 | 意思 / 用法 |
|---|---|
| open a door that was long closed | 打开一扇久闭的门（比喻新机会） |
| waste heat | 余热、废热 |
| district heating | 区域供热 |
| greenhouse | 温室 |
| back-up | 备用（名词，也写 backup） |

---

## 四、数据中心暖通术语表（重点）

这部分是你工作里最用得上的，建议做成单词卡反复看。文中出现过的打了 ★。

### 冷源与散热
| 中文 | English | 备注 |
|---|---|---|
| 冷水机组 ★ | chiller | air-cooled / water-cooled chiller |
| 压缩机 ★ | compressor | |
| 制冷站 ★ | cooling plant / chiller plant | |
| 机械制冷 ★ | mechanical cooling | |
| 自然冷却 ★ | free cooling / economiser (美 economizer) | water-side / air-side economiser |
| 干冷器 ★ | dry cooler | adiabatic dry cooler 绝热（喷淋）干冷器 |
| 冷却塔 | cooling tower | |
| 散热 / 排热 ★ | heat rejection | |
| 调峰冷机 ★ | trim chiller | |
| 干球 / 湿球温度 | dry-bulb / wet-bulb temperature | |
| 逼近度 | approach (temperature) | |

### 液冷系统
| 中文 | English | 备注 |
|---|---|---|
| 冷板 ★ | cold plate | direct-to-chip (DTC) cooling 直接芯片冷却 |
| 浸没式液冷 | immersion cooling | single-phase / two-phase |
| 冷量分配单元 ★ | coolant distribution unit (CDU) | |
| 一次侧 / 二次侧 | primary / secondary loop | facility water / technology cooling system (TCS) |
| 供水 / 回水温度 | supply / return water temperature | |
| 背板换热器 | rear-door heat exchanger (RDHx) | |
| 液冷捕获率 | liquid capture ratio | 文中 "most, but not all" 说的就是它 |

### 风侧与机房
| 中文 | English | 备注 |
|---|---|---|
| 机房 ★ | data hall / white space | |
| 精密空调（冷冻水型） | CRAH (computer room air handler) | |
| 精密空调（直膨型） | CRAC (computer room air conditioner) | |
| 冷 / 热通道 | cold / hot aisle | containment 封闭 |
| 进风温度 | inlet temperature | |
| 剩余风冷负荷 ★ | residual air-side load | |

### 指标与运维
| 中文 | English | 备注 |
|---|---|---|
| 电能利用效率 | PUE (power usage effectiveness) | |
| 用水效率 | WUE (water usage effectiveness) | |
| 冗余 ★ | redundancy | N+1, 2N |
| 正常运行时间 ★ | uptime | |
| 余热回收 ★ | waste-heat reuse / heat recovery | |
| 区域供热 ★ | district heating | |
| 存量 / 新建项目 | brownfield / greenfield | 文中 "existing buildings" 就是 brownfield |

---

## 五、拿来就能用的表达（工作场景）

| 文中表达 | 换个场景这样用（暖通 / 工作邮件） |
|---|---|
| **not whether A but how B** | *The question is not whether we need chillers, but how we size them.* |
| **most, but not all, of** | *The CDU handles most, but not all, of the heat load.* |
| **anywhere from A to B** | *The residual air load could be anywhere from 15% to 25%.* |
| **depends on** + 名词 | *How many hours of free cooling we get depends on the site's wet-bulb profile.* |
| **narrow the gap between A and B** | *A higher supply temperature widens the gap between the water and ambient air.*（反用 widen） |
| **designed for the worst hour of the worst day** | *The plant is designed for the worst hour of the worst day, not the average.* |
| **kick in** | *The trim chiller kicks in when ambient exceeds 35°C.* |
| **as insurance** | *We kept one chiller as insurance against heatwaves.* |
| **shift from A to B** | *Our scope is shifting from chiller plants to CDUs and controls.* |
| **wring the most out of** | *Good controls let you wring the most out of every degree of ΔT.* |

---

## 六、练习

### A. 理解自测
1. Why did HVAC companies' shares fall?
2. According to the article, does "chillerless" mean no heat rejection is needed? Why or why not?
3. Why might a site in Singapore still need chillers?
4. Give two reasons why air cooling will not disappear completely.
5. What new business opportunity does warmer water create?

### B. 用英文说出来（口语输出）
用 3–4 句英文，向一位外国同事解释：**为什么 45°C 供水能减少冷机运行时间，但在新加坡这样的地方仍然需要冷机。** 尽量用上：*supply water temperature, free cooling, dry cooler, wet-bulb, trim chiller*。录下来自己听一遍。

### C. 汉译英（用括号里的表达）
1. 问题不在于要不要上液冷，而在于怎么和现有风冷系统整合。（not whether … but how …）
2. 冷板能带走大部分但不是全部的热量。（most, but not all, of）
3. 剩余的风冷负荷可能在 10% 到 30% 之间。（anywhere from … to …）
4. 只有当室外温度超过 35°C 时，调峰冷机才会启动。（kick in）
5. 我们的工作重点正从建大型冷站转向设计更智能的控制系统。（shift from … to …）

### D. 改错（中国学习者常见错误）
1. The water is not enough cold to cool the servers.
2. Shares fell 7% to the price of $80, a drop by 7%.
3. The system has redundant, so it is very reliable.

---

## 七、参考答案

<details><summary>点开看答案</summary>

**A.**
1. Nvidia's CEO said the next-generation chips could be cooled with 45°C water, so data centres would not need chillers, which are a major product for those companies.
2. No. The heat still has to be rejected to the atmosphere; warm water only reduces how often mechanical cooling runs.
3. Hot, humid weather narrows the gap between the water and the outdoor air, so free cooling isn't enough on many days.
4. Any two: liquid cooling doesn't capture all the heat (residual air-side load); many AI deployments are in existing air-cooled buildings; operators keep mechanical cooling as insurance for reliability.
5. Selling or reusing waste heat, e.g. for district heating or greenhouses.

**B. 参考说法**
> With a supply water temperature of 45°C, a dry cooler can reject the heat to outdoor air for most of the year, so we get a lot more free-cooling hours and the chillers barely run. But in a place like Singapore, the wet-bulb temperature stays high all year, so the gap between the water and the ambient air is small. That's why we'd still keep trim chillers to kick in on the hottest, most humid days.

**C.**
1. The question is not whether to adopt liquid cooling, but how to integrate it with the existing air-cooling system.
2. Cold plates remove most, but not all, of the heat.
3. The residual air-side load could be anywhere from 10% to 30%.
4. The trim chiller kicks in only when the outdoor temperature exceeds 35°C.
5. Our focus is shifting from building large chiller plants to designing smarter control systems.

**D.**
1. The water is not **cold enough** to cool the servers.（enough 放在形容词后）
2. Shares fell **by** 7% **to** $80.（by 表幅度，to 表结果；a drop **of** 7%）
3. The system **has redundancy** / **is redundant**, so it is very reliable.（redundant 是形容词，名词是 redundancy）

</details>

---

## 八、3 天学习计划

| 天 | 做什么 | 时间 |
|---|---|---|
| Day 1 | 通读正文两遍，不查词，先抓大意 → 看第 1–3 段精读 → 背第 2 段（冷机原理那段） | 35 min |
| Day 2 | 看第 4–6 段精读 → 过一遍术语表，做单词卡 → 做练习 A、D | 35 min |
| Day 3 | 跟读（shadowing）第 3、5 段各 3 遍 → 做练习 B（录音）和 C → 回到开头重做"学前自测" | 40 min |

> **跟读小技巧**：可以用任何 TTS 工具（如手机自带朗读）把第 3、5 段读出来，你落后半句跟着读，注意 *chillerless, compressor, atmosphere, integrated* 的重音位置。

---

## 九、素材来源

- NBC News — *AI boom warning sign? Nvidia's new chips hit data center cooling stocks*: https://www.nbcnews.com/business/markets/nvidia-vera-rubin-chip-warning-ai-investing-boom-rcna252679
- Facilities Dive — *No chillers needed for Vera Rubin server racks, Nvidia CEO says*: https://www.facilitiesdive.com/news/no-chillers-needed-for-vera-rubin-server-racks-nvidia-ceo/809216/
- ACHR News — *Nvidia's Vera Rubin has chilling effect on HVAC industry*: https://www.achrnews.com/articles/165683-nvidias-vera-rubin-has-chilling-effect-on-hvac-industry
- The Motley Fool — *Here's why shares in Johnson Controls slumped today*: https://www.fool.com/investing/2026/01/07/heres-why-shares-in-johnson-controls-slumped-today
- Motivair — *The truth about chillerless AI data centers*: https://www.motivaircorp.com/news/the-truth-about-chillerless-ai-data-centers/
- Data Center Frontier — *Cooling's new reality: it's not air vs. liquid anymore, it's architecture*: https://www.datacenterfrontier.com/cooling/news/55360274/coolings-new-reality-its-not-air-vs-liquid-anymore-its-architecture
- Data Center Knowledge — *The rise of flexible hybrid cooling for AI data centers*: https://www.datacenterknowledge.com/infrastructure/the-rise-of-flexible-hybrid-cooling-for-ai-data-centers
- Vertiv — *Beyond the compressor-less hype: matching data center cooling technology to climate reality*: https://www.vertiv.com/en-latam/insights/articles/educational-articles/beyond-the-compressor-less-hype-matching-data-center-cooling-technology-to-climate-reality/

> **说明**：各家报道的股价跌幅不一（Johnson Controls 约 7.4%–7.5%，Trane 约 5.3%–7.6%），正文取"约 5–7%"。"剩余风冷负荷占 10%–33%" 是行业常见量级，具体取决于服务器设计。
