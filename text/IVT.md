# 意象向量论（Image Vector Theory）学术大纲

> **跨学科理论框架**：诗学 × 数学 × 认知科学 × 计算机科学 × 创作实践
>
> 核心命题：意象不仅是符号，还可以被构建为向量。诗歌意象的情感生产可以建模为高维情感向量空间中的向量运算。在咏物诗的范畴中，**向量构建由作者完成，向量运算由读者完成**，使得读者在读诗的过程中得以发挥主观能动性，使情感自主扎根、更加牢固，由此形成咏物诗的独特艺术效果。

## 摘要

传统诗学以"兴""含蓄""意象派""客观对应物"等概念描述了"物象能传达情感"这一现象，但始终未能解释其底层运作机制——为什么"枯藤老树昏鸦"六组名词能精确传递萧瑟感，而任何情感修饰词都无法复现同一效果？本文提出意象向量论（Image Vector Theory, IVT），一个跨诗学、数学、认知科学与计算机科学的分析框架，将诗歌意象的情感生产建模为高维情感向量空间中的向量运算。

IVT 包含四项核心主张。第一，标/向分离：意象可拆解为"标"（物象实体）与"向"（情感方向），前者对应向量空间原点位置，后者对应方向分量。第二，叠加与维度锁定：方向一致的意象（同频叠加）通过多维度协迫锁定单一情感坐标；方向冲突的意象（异频叠加）则需要更多维度来收敛歧义，由此建立了维度数量与情感歧义度之间的公式。第三，动词-动量与三种轨迹类型：将动词定义为情感空间中的移动向量，识别出静态向量群→末端爆发、单向移动、动作穿插三种情感轨迹类型。第四，读者情感生产责任转移：在咏物诗中，作者完成向量构建，读者完成向量运算，由此给出"一千个读者有一千个哈姆雷特"的精确认知机制解释——不同读者的意象感知权重与向量计算能力不同，构建的图拓扑必然不同。

在上述框架基础上，本文进一步提出 IVS 嵌套空间论，将作为隐含参考系原点的"我"拉平为可被标/向框架处理的操作对象，建立双层标/向嵌套的情感空间模型，使框架能够分析主体自反式诗歌。

IVT 的理论贡献包括：（1）首次将意象拆解为向量分量并形式化；（2）首次用量化公式描述维度-歧义反比关系；（3）首次将动词转化为情感运动学参数；（4）首次用向量运算表述读者情感推导机制。在应用层面，IVT 为 AI 诗歌生成提供了从"修辞优化"到"向量空间构造"的策略转向，以及基于五维机制（标/向分离、维度锁定、动词-动量、责任转移、嵌套空间）的评估框架与参数高效微调指导。

## 关键词：意象向量论；标/向分离；维度锁定；情感向量空间；读者责任转移；咏物诗；计算诗学；嵌套空间；创作实践

---

## 一、引言

- **问题意识**：以"兴"、"含蓄"、"以物观物"、"意象派"[6]、客观对应物[7]为主要学术支柱的传统诗学描述了"物象能传达情感"这一现象，但未能解释其底层运作机制，为什么"枯藤老树昏鸦"六个名词能传递出萧瑟感？为什么"能跑就行"比任何修饰都更能传递开发者的无力？
- **核心命题**：意象不仅是符号，还可以被构建为向量。诗歌意象的情感生产可以建模为高维情感向量空间中的向量运算。与此同时，在咏物诗的范畴中，**向量构建由作者完成，向量运算由读者完成**，形成情感空间中的图拓扑，使得读者在读诗的过程中得以发挥主观能动性，使情感自主扎根、更加牢固，由此形成咏物诗的独特艺术效果。
  - **图拓扑与"一千个哈姆雷特"**：读者在向量运算中构建的是一份具体的**图拓扑**（节点=意象向量，边=向量关系），不同读者的意象感知权重与向量计算能力不同，所构建的图拓扑必然不同，这给出了"一千个读者有一千个哈姆雷特"的精确认知机制解释
- **方法论**：跨学科整合：诗学（意象研究）+ 数学（向量空间/拓扑学）+ 认知科学（概念空间[12]/神经认知[14]）+ 计算机科学（词嵌入/语义向量空间[26][27]）+ **创作实践**
- **研究范围**：汉语古典诗歌分析、当代诗歌分析、作者作品分析。聚焦于情感生产机制而非审美价值判断
- **作者的话**：该节讨论了 AI 技术发展、作者自身创作焦虑、文坛腐败现象及本文出发点。

---

## 二、意象的向量定义（数学 × 诗学 × 计算机科学 × 创作实践）

- **2.1 传统意象概念的局限**：意象作为"黑箱"，未分离物象实体与情感方向
- **2.2 标与向的分离**：意象 = `标（物象实体）` + `向（情感方向）`
  - 标：物象的实体基座，如藤、阳、鸦、调用栈——向量空间中的原点位置
  - 向：状态修饰或文化编码赋予的方向，如枯、残、老、非法——向量方向
- **2.3 向量拆分与组合**：
  - 2.3.1 异标同向
  - 2.3.2 同标异向
  - 2.3.3 实例拆解
  - 2.3.4 公式化总结
- **2.4 创作实践的视角**：蟛蜞在《调用日志》中自然运用的"调用栈""灰色注释""标红报错"等意象，在创作直觉中完成了标与向的分离，得以让理论从实践中反向翻译而来，而非从概念出发的推演
- **2.5 与平行研究的比较**：Rochallyi 向量诗歌[1]：向量方向+长度，但未区分标/向、未涉及文化编码机制；词嵌入技术[26][27]：验证意象向量化的可行性但无机制解释

---

## 三、向量叠加与维度锁定（数学 × 认知科学 × 诗学）

- **3.1 同频叠加**：方向一致的意象叠加，合成向量方向不变、模长增加、情感坐标锁定
  - 案例：以"枯藤+老树+昏鸦"为例，三个衰败方向向量锁定萧瑟坐标
  - 认知机制：维度越多，歧义越少，低维趋于模糊，高维趋于精确
- **3.2 异频叠加**：方向冲突的意象叠加，合成向量方向不确定
  - 案例：以"雄鹰+残阳"为例，组合可指向英雄迟暮、悲剧力量或衰败中的尊严
  - 关键发现：异频配对的有效性取决于是否被足够多的额外维度锁定
  - 公式推论：异频向量夹角越大，需要的额外维度越多
- **3.3 维度锁定的拓扑学解释**
  - 高维空间可表达低维空间不存在的情感位置
  - 与层论表征[29]（sheaf theory）和POET[28]拓扑模型的平行关系
  - 维度锁定的数学本质：在情感流形上划定子区域
- **3.4 创作实践验证**：蟛蜞《调试日志》中，"非法配置落入灰色注释"+"超时请求沉进标红报错"两个异源但同频的报错场景叠加，比单一报错场景更精确地固定了"被技术世界困住"的情感坐标

---

## 四、动词作为移动向量（认知科学 × 计算机科学 × 文学）

- **4.1 从静态向量到动态轨迹**
  - 定义：动词/动作 = 在情感空间中推动读者移动的向量操作
  - 形式化：`点（主体）× 移动向量 · 方向（向）· 终点（标）`
  - 案例：`乌鸦（点）× 落入（移动）· 残（向）· 阳（标）`
- **4.2 三种轨迹类型（原创分类）**
  1. **静态向量群→末端爆发**，以马致远"枯藤老树昏鸦→断肠人在天涯"为例：读者被定位后被推送至冲刺爆发
  2. **单向移动**，以"乌鸦落入残阳"为例：读者跟随单一轨迹并抵达终点
  3. **动作穿插**，以蟛蜞《调试日志》为例：读者跟随散乱轨迹，情感无法锁定并形成徘徊与流离感
- **4.3 三种轨迹类型的拓扑对比**
- **4.4 创作实践验证**

---

## 五、读者情感生产责任转移（神经科学 × 认知理论）

- **5.1 从信息接收到运算执行**
  - **向量构建由作者完成**：选择标的、赋予方向感、控制维度关系、设置轨迹类型
  - **向量运算由读者完成**：读取向量方向、计算叠加关系、推测合成向量、翻译为情感体验
- **5.2 责任转移的发生条件与阈值**：
  - 5.2.1 向量信息的维度充足时的责任转移
  - 5.2.2 向量信息的不完整迫使读者介入时的责任转移
  - 5.2.3 阈值的动态性
- **5.3 留白美学的解释：负优化、无解意象**
  - 5.3.1 负优化
  - 5.3.2 无解意象
  - 5.3.3 责任转移的强度谱系
- **5.4 认知负荷与情感强度的关系**
  - 5.4.1 运算量作为强度指标
  - 5.4.2 最优运算量假设

---

## 六、意象向量论的理论定位（诗学 × 数学 × 认知科学 × 计算机科学）

### 6.1 四大核心主张与原创贡献

| 主张 | 核心机制 | 原创贡献 |
|------|---------|---------|
| 标/向分离 | 意象 = 标(物象实体) + 向(情感方向) | 首次将意象拆解为向量分量并形式化；"向"是连续方向向量而非单一情感标签 |
| 叠加与维度锁定 | 同频→锁定情感坐标，异频→扩展维度以锁定 | 首次用量化公式描述维-歧义反比关系；区分同频/异频两种认知机制 |
| 动词-动量与三种轨迹 | 动词=情感空间中推动读者的速度向量 | 首次将动词转化为情感运动学参数；提出三种轨迹类型分类法 |
| 读者责任转移 | 读者=主动完成向量合成的运算者 | **重要的学术空白**——首次用向量运算表述读者情感推导；提出ReaderCompute、负优化、最优运算量假设 |

### 6.2 跨学科整合的双重结构

**横向——四大主张的对称映射**：

| 主张 | 对接学科 | 平行参照系 |
|------|---------|-----------|
| 标/向分离 | 诗学 | Rochallyi[1]向量诗学 |
| 叠加与维度锁定 | 数学×拓扑学 | 层论[29]表征、洛特曼[4]符号圈、POET[28]贝蒂数 |
| 动词-动量与轨迹 | 语言学×认知科学 | Gärdenfors[12]双向量模型、Stockwell[16]指示投射 |
| 读者责任转移 | 认知科学×美学 | Jacobs[14] NCPM、Text World Theory[18] |

**纵向三级感知链路**：文化编码层——"向"源于语言共同体的历史编码；符号共鸣层——同频共振加强而异频张力创新；认知渲染层——留白迫使读者自主完成情感闭合

### 6.3 理论定位、比较与局限

**定位**：分析框架而非方法论或创作指南；认知理论而非工程应用或数字人文工具；仅覆盖意象与情感这一特定子问题而非全域理论。在九个理论框架中，IVT是同时使用向量/几何语言、讨论维度锁定、讨论读者责任转移的分析框架。

**局限**：①情感维度定义待经验充实 ②ReaderCompute目前暂没有对应理论研究能精确解析 ③三种轨迹覆盖范围有限 ④最优运算量假设未经实证检验

> **与第七章的差异**：本标准模型（第2至6章）→ 嵌套扩展（第7章），后者打破"我=隐含参考系原点"的假设，将IVT从意象层面扩展到主体层面。

---

## 七、IVS嵌套空间论：主体建模化与情感空间嵌套（诗学 × 认知科学 × 创作实践）

> **核心命题**：将"我"从IVT的隐含参考系原点拉平为可被标/向框架处理的操作对象，建立双层标/向嵌套的情感空间模型。

### 7.1 问题的发现：IVT框架的隐含假设
IVT标准框架将"我"默认为情感向量空间（IVS）的隐含参考系原点。蟛蜞式诗歌——如"我不是我""我站在时间之外""从梦乡中归来"——证明这一假设可被打破，"我"可以被建模为新的标 $\text{Obj}_{\text{我}}$。

### 7.2 打破隐含假设
传统诗与蟛蜞式诗歌的情感生产链路公式化对比，揭示传统IVT处理不了"我"被建模为可操作对象时的四层运算结构。

### 7.3 三层空间模型
- **第一空间**——作者到向量场的空间：作者构造意象标/向，标准IVT覆盖范围
- **第二空间**——向量场到读者的空间：读者运算向量锁定情感坐标
- **第三空间**——作者经"我"到读者的空间：作者将"我"建模为标 $\text{Obj}_{\text{我}}$ 并赋轨迹 $\text{Traj}(\text{Obj}_{\text{我}})$，三空间通过内外双层标/向反馈耦合

### 7.4 主体建模化
将"我"建模为 $\langle \text{Obj}_{\text{我}},\ \text{Traj}(\text{Obj}_{\text{我}}) \rangle$，外层标的（$\text{Obj}_{\text{我}}$）与内层意象标/向并行运算。标的嵌套使读者运算从1层升级为至少4层，包括外层标识别、内层分析、外层轨追踪与耦合校准。

### 7.5 三种主体模式
- **常规主体**：$\text{Obj}_{\text{我}}$ 不可观测，读者自动投影到原点 $O$，1层运算
- **被动构建体**：$\text{Obj}_{\text{我}}$ 可观测，轨迹低闭合度外力驱动，2层+耦合
- **主动构建体**：$\text{Obj}_{\text{我}}$ 可分解为多重标，多重轨迹/自指，2+层+耦合

### 7.6 空间嵌套的运作方式
双层标/向耦合的运作机制：情感劳动谱系新增"嵌套转移"层级（透明→轻度→中度→高度→极限→嵌套转移），读者需同时运算内层意象合成和外层"我"的轨迹。

### 7.7 技法体系的对应
技法操作与 IVS 嵌套层级之间的对应映射表，被动构建与主动构建在技法层面的统一解释。

### 7.8 嵌套空间论的理论意义
- 情感劳动从一维（运算量）扩展为二维（运算量 × 标/向层数）
- "我"不是特权原点，可以被建模为标
- 元层级作为创作者的第三只手

### 7.9 隐式/显式构建切换分析
- "我"的构建状态不是一次性二元激活/不激活的开关。同一首诗可在不同阶段在隐式构建↔显式构建之间反复切换，切换次数 $N_{\text{switch}}$ 作为结构复杂度的新度量维度。

---

## 八、在AI写诗与计算诗学中的潜在应用（计算机科学 × 诗学 × 创作实践）

- **8.1 生成策略转向**：从"修辞优化"（预测最可能的词）→ "向量空间构造"（锁定目标情感坐标的意象组合）
从预测修辞式生成到向量空间构造式生成至少解决了两个重大问题：1.修辞总是要引入额外的物或意象，引入内容一旦稍有偏差，就会导致向量叠加错乱，破坏全诗情感拓扑，导致成诗的语言结构一团乱麻；2.额外引入的内容减少了读者的情感劳动，意象空间被急剧压缩，读者在读诗时的自主性降低，情感生成空间受限
- **8.2 评价标准重塑**：从"语言流畅度" → "向量空间维度与锁定精度"
- **8.3 风格迁移范式**：从"模仿用词"→ "模仿向量布局"
  - 为什么AI仿写总差一口气：在模仿"用词"和"句式"，而非"向量布局"
  - 蟛蜞诗的"没有硅味"源于向量布局是感知实践的产物，而非语料库统计关联
- **8.4 创作经验与情感劳动的感知增长**：创作实践为分析者提供了感知诗歌中情感劳动的能力，非创作者读成品，创作者读生产过程。意象向量论将这一隐性感知翻译为显式知识，构成其理论起点之一
- **8.5 人类创作经验与AI分析能力的差异及IVT向评估工具的迁移**
  - **8.5.1 AI分析的情感盲区**：AI无法感知诗歌中的情感构造过程，仅能检测表层语义关联
  - **8.5.2 差异的分析差异**：AI统计与人类结构感知的根本分歧，AI缺少"情感劳动"的感知通道
  - **8.5.3 从差异到迁移**：IVT的分析框架可迁移为AI情感生成评估工具
  - **8.5.4 可行性与实用性分析**：五维机制与评估需求的结构性对应：标/向分离对应语义清晰度，向量叠加对应ECI，动词-动量对应叙事结构，责任转移对应参与度，嵌套空间对应主体建模；可操作化路径（ivt-poem-analyzer工具链）
- **8.6 意象向量论对参数高效指导诗歌风格微调的意义**
  - **8.6.1 当前的诗歌风格微调及其局限**
  - **8.6.2 标/向分离对 LoRA 训练目标的语义可解释性增强**
  - **8.6.3 维度锁定对异频意象组合质量的约束**
  - **8.6.4 动词-动量约束与轨迹类型选择**
  - **8.6.5 读者责任转移与留白程度的可计算控制**
  - **8.6.6 DoRA 与 IVT 的结构同构：跨层次验证**

---

## 九、结论

- **9.1 意象向量论的整合性**：将诗学（意象研究）、认知科学（概念空间/神经认知）、计算机科学（词嵌入/向量空间）、数学（拓扑学）、**创作实践**五个领域整合为统一的理论框架
- **9.2 原创贡献清单**：
  1. **"标"与"向"的区分**——意象的二分法
  2. **"维度锁定"机制**——维度与歧义度的反比关系
  3. **"动词作为移动向量"**——在诗歌情感分析中的应用
  4. **"读者情感生产责任转移"**——向量化表述
  5. **三种轨迹类型**——静态→爆发 / 含移动单一表达式 / 散列不收敛
  6. **咏物诗的两阶段协作模型**——作者做向量构建，读者做向量运算
  7. **IVT嵌套空间论**——主体向量化与三层空间模型；将"我"从隐含参考系拉平为可被构造的向量；揭示双IVT空间嵌套导致情感劳动剧增的机制
  8. **学术空白定位**
- **9.3 未来方向**
  - **9.3.1 向量空间构造式生成的形式化建模**
  - **9.3.2 嵌套空间结构的生成参数化**
  - **9.3.3 负优化与留白程度的算法控制**
  - **9.3.4 向量布局的风格迁移与风格发现**
  - **9.3.5 IVS嵌套构建可能存在更多的维度**
  - **9.3.6 参数高效微调中的向量布局约束**

---

- **结语**


## 附录：四大核心素材

### 附录A：元创作案例——原为《无题》，本文中统称为《调试日志》

```
调用栈一层又一层
剥开我不曾知晓的技术奥密
函数名一峰又一峰
写出我无法参透的架构细节
面对纷繁杂乱的二进制洪流，
就像我不知道该怎么用悲、殇、残、哀
来表露我的心情
非法的配置落入一行行灰色注释
超时的请求沉进一条条标红报错
我无法窥探它原来的样子
只是一步步跨上系统的手脚架
心中默念，能跑就行
```

**理论意义**：全诗无传统"诗意"意象，以"调用栈"、"函数名"、"二进制洪流"、"灰色注释"、"标红报错"等技术物象作为核心意象群，是意象向量论"物象本身即情绪"的典型例证。经删去所有情绪词后，该理论得到验证。

---

## 附录B：蟛蜞精选创作分析

> 来源：`IVT_result/punky`


**意象向量论的创作源头定位**
蟛蜞的物我同构技法（以物寓情→沉默对话→物象意志）是意象向量论"物象本身即情绪"的创作实践源头。其"收束跳水"技法直接对应意象向量论中的"读者责任转移"中把情感生产的责任完全交给读者的理论。"否定式定义"对应"维度锁定"，用"不"来削出边界，既增加向量运算的负责度，又一定程度上压缩情感坐标的歧义空间。

---

## 附录C：中外名篇精选分析

> 来源：`IVT_result/reference`

---

## 附录D：参考文献

### 一、诗学与文学理论

[1] ROCHALLYI R. Vector Poetry[EB/OL]. (2023-06-29)[2026-07-11]. https://maa.org/math-values/vector-poetry/.

[2] KURZYNSKI M, XU X, FENG Y. The game of keys and queries: parallelism and cognitive geometry in Chinese regulated verse[J/OL]. International Journal of Humanities and Arts Computing, 2025, 19(2): 143-157. https://doi.org/10.3366/ijhac.2025.0355. [2026-07-11].

[3] 刘勰. 文心雕龙[M]. 北京: 人民文学出版社, 1958.

[4] LOTMAN Y. Universe of the mind: a semiotic theory of culture[M]. Bloomington: Indiana University Press, 1990.

[5] FAUCONNIER G, TURNER M. The way we think: conceptual blending and the mind's hidden complexities[M]. New York: Basic Books, 2002.

[6] POUND E. A retrospect[M]//Literary essays of Ezra Pound. London: Faber and Faber, 1954.

[7] ELIOT T S. Hamlet and his problems[M]//The sacred wood: essays on poetry and criticism. London: Methuen, 1920.

[8] 王国维. 人间词话[M]. 上海: 上海古籍出版社, 1998.

[9] 严羽. 沧浪诗话[M]. 北京: 中华书局, 2014.

[10] 司空图. 二十四诗品[M]. 北京: 人民文学出版社, 1963.

[11] FAUCONNIER G. Mental spaces: aspects of meaning construction in natural language[M]. Cambridge: Cambridge University Press, 1994.

### 二、认知科学与神经认知

[12] GÄRDENFORS P. Conceptual spaces: the geometry of thought[M]. Cambridge, MA: MIT Press, 2000.

[13] GÄRDENFORS P. The geometry of meaning: semantics based on conceptual spaces[M]. Cambridge, MA: MIT Press, 2014.

[14] JACOBS A M. Neurocognitive poetics: methods and models for investigating the neuronal and cognitive-affective bases of literature reception[J]. Frontiers in Human Neuroscience, 2015, 9: 186.

[15] JACOBS A M. SentiArt: a vector space model for the computation of emotion potential in texts[C]//Proceedings of the 2018 Conference on Empirical Methods in Natural Language Processing. Brussels: ACL, 2018.

[16] STOCKWELL P. Cognitive poetics: an introduction[M]. London: Routledge, 2002.

[17] STOCKWELL P. Cognitive poetics: a new introduction[M]. 2nd ed. London: Routledge, 2019.

[18] WERTH P. Text worlds: representing conceptual space in discourse[M]. London: Longman, 1999.

[19] GAVINS J. Text world theory: an introduction[M]. Edinburgh: Edinburgh University Press, 2007.

[20] ISER W. The act of reading: a theory of aesthetic response[M]. Baltimore: Johns Hopkins University Press, 1978.

[21] ISER W. The implied reader: patterns of communication in prose fiction from Bunyan to Beckett[M]. Baltimore: Johns Hopkins University Press, 1974.

[22] FRISTON K. The free-energy principle: a unified brain theory?[J]. Nature Reviews Neuroscience, 2010, 11(2): 127-138.

[23] VAN DE CRUYS S, FRASCAROLI J, FRISTON K. Order and change in art: towards an active inference account of aesthetic experience[J]. Philosophical Transactions of the Royal Society B: Biological Sciences, 2024, 379(1895): 20220411.

[24] PETERSEN M K. Latent semantics of action verbs reflect phonetic parameters of intensity and emotional content[J]. PLoS ONE, 2015, 10(4): e0121575.

[25] STOCKWELL P. Texture: a cognitive aesthetics of reading[M]. Edinburgh: Edinburgh University Press, 2009.

### 三、计算机科学与计算诗学

[26] MIKOLOV T, CHEN K, CORRADO G, et al. Efficient estimation of word representations in vector space[C]//Proceedings of ICLR Workshop. Scottsdale: ICLR, 2013.

[27] DEVLIN J, CHANG M W, LEE K, et al. BERT: pre-training of deep bidirectional transformers for language understanding[C]//Proceedings of NAACL-HLT. Minneapolis: ACL, 2019: 4171-4186.

[28] WANG R, LEHMAN J, CLUNE J, et al. POET: paired open-ended trailblazer model for open-ended evolution[J/OL]. arXiv preprint arXiv:1901.01753, 2019.

[29] AYZENBERG A, GEBHART T, MAGAI G, et al. Sheaf theory: from deep geometry to deep learning[EB/OL]. (2025-02-21)[2026-07-11]. https://arxiv.org/abs/2502.15476.

[30] KURZYNSKI M, XU X, FENG Y. Vector poetics: parallel couplet detection in classical Chinese poetry[C]//Proceedings of the 4th International Conference on Natural Language Processing for Digital Humanities (NLP4DH 2024), 2024: 200-208.

### 四、数学与情感科学

[31] COWEN A S, KELTNER D. Semantic space theory: a new approach to understanding emotion[J]. Nature Reviews Psychology, 2024, 3: 88-103.

[32] COWEN A S, KELTNER D. Self-report captures 27 distinct categories of emotion bridged by continuous gradients[J]. Proceedings of the National Academy of Sciences, 2017, 114(38): E7900-E7909.

[33] 段玉聪. 段玉聪 DIKWP 哲学体系解析[EB/OL]. ResearchGate, (2025-11)[2026-07-11]. https://www.researchgate.net/doi/10.13140/RG.2.2.15793.65127.

### 五、神经科学实验与实证研究

[34] MERLEAU-PONTY M. Phenomenology of perception[M]. SMITH C, 译. London: Routledge, 1962.

[35] BARSALOU L W. Perceptual symbol systems[J]. Behavioral and Brain Sciences, 1999, 22(4): 577-660.

### 六、语言大模型微调实践方向

[36] HU E J, SHEN Y, WALLIS P, et al. LoRA: low-rank adaptation of large language models[C]//Proceedings of the International Conference on Learning Representations (ICLR 2022), 2022.

[37] DETTMERS T, PAGNONI A, HOLTZMAN A, et al. QLoRA: efficient finetuning of quantized LLMs[C]//Proceedings of NeurIPS 2023, 2023.

[38] LIU S Y, WANG C Y, YIN H, et al. DoRA: weight-decomposed low-rank adaptation[C]//Proceedings of the International Conference on Machine Learning (ICML 2024), 2024.

[39] ZHANG Q, CHEN M, BUKHARIN A, et al. AdaLoRA: adaptive budget allocation for parameter-efficient fine-tuning[C]//Proceedings of ICLR 2023, 2023.

[40] HAN Z, GAO C, LIU J, et al. Parameter-efficient fine-tuning for large models: a comprehensive survey[J/OL]. arXiv:2403.14608, 2024.

[41] LIALIN V, DESHPANDE V, RUMSHISKY A. Scaling down to scale up: a guide to parameter-efficient fine-tuning[J/OL]. arXiv:2303.15647, 2023.

[42] LYU Y, LIANG P P, PHAM H, et al. StylePTB: a compositional benchmark for fine-grained controllable text style transfer[C]//Proceedings of the 2021 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies. Online: Association for Computational Linguistics, 2021: 2116-2138. DOI:10.18653/v1/2021.naacl-main.171.

[43] LAKOFF G, JOHNSON M. Metaphors we live by[M]. Chicago: University of Chicago Press, 1980.

