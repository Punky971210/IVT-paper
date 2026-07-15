# 意象向量论（Image Vector Theory）学术大纲

> **跨学科理论框架**：诗学 × 数学 × 认知科学 × 计算机科学 × 创作实践
>
> 核心命题：意象不仅是符号，还可以被构建为向量。诗歌意象的情感生产可以建模为高维情感向量空间中的向量运算。在咏物诗的范畴中，**向量构建由作者完成，向量运算由读者完成**，使得读者在读诗的过程中得以发挥主观能动性，使情感自主扎根、更加牢固，由此形成咏物诗的独特艺术效果。

---

## 一、引言

- **问题意识**：传统诗学（兴、含蓄、以物观物、意象派[7]、客观对应物[8]）描述了"物象能传达情感"这一现象，但未能解释其底层运作机制——为什么"枯藤老树昏鸦"六个名词能传递出萧瑟感？为什么"能跑就行"比任何修饰都更能传递开发者的无力？
- **核心命题**：意象不仅是符号，还可以被构建为向量。诗歌意象的情感生产可以建模为高维情感向量空间中的向量运算。与此同时，在咏物诗的范畴中，**向量构建由作者完成，向量运算由读者完成**，形成情感空间中的图拓扑，使得读者在读诗的过程中得以发挥主观能动性，使情感自主扎根、更加牢固，由此形成咏物诗的独特艺术效果。
  - **图拓扑与"一千个哈姆雷特"**：读者在向量运算中构建的是一份具体的**图拓扑**（节点=意象向量，边=向量关系），不同读者的意象感知权重与向量计算能力不同，所构建的图拓扑必然不同——这给出了"一千个读者有一千个哈姆雷特"的精确认知机制解释
- **方法论**：跨学科整合——诗学（意象研究）+ 数学（向量空间/拓扑学）+ 认知科学（概念空间[13]/神经认知[15]）+ 计算机科学（词嵌入/语义向量空间[27][28]）+ **创作实践**
- **研究范围**：汉语古典诗歌与当代诗歌分析，聚焦于情感生产机制而非审美价值判断

---

## 二、意象的向量定义（数学 × 诗学 × 计算机科学 × 创作实践）

- **2.1 传统意象概念的局限**：意象作为"黑箱"——物象实体与情感方向的未分离
- **2.2 标与向的分离**：意象 = `标（物象实体）` + `向（情感方向）`
  - 标：物象的实体基座（藤、阳、鸦、调用栈）——向量空间中的原点位置
  - 向：状态修饰或文化编码赋予的方向（枯、残、老、非法）——向量方向
- **2.3 意象向量的三维属性**：
  - **方向**：由文化编码预先染色（雄鹰→力量/昂扬，残阳→衰落/终结）
  - **模长**：由意象的感知强度决定（"枯藤"模长 > "藤"，因"枯"强化了方向）
  - **维度**：携带的情感语义维度数，决定与其他意象的匹配精度
- **2.4 创作实践的视角**：蟛蜞在《调用日志》中自然运用的"调用栈""灰色注释""标红报错"等意象，在创作直觉中完成了标与向的分离，得以让理论从实践中反向翻译而来，而非从概念出发的推演
- **2.5 与平行研究的比较**：Rochallyi 向量诗歌[1]（向量方向+长度，但未区分标/向、未涉及文化编码机制）；词嵌入技术[27][28]（验证意象向量化的可行性但无机制解释）
- **2.6 向的两种来源：文化编码与结构赋值（同标异向）**
  - 传统意象的"向"依赖**文化编码**——"枯"的衰败方向在语言共同体中预先染好，作者只需调用既有的文化储备即可（"枯藤老树昏鸦""雄鹰残阳"），对于训练有素的诗读者来说也很容易迅速唤起。
  - 蟛蜞式意象的"向"依赖**结构赋值**——"耳机隔绝世界""人来人往的世界很大/很挤"——标的"向"不是在文化中预先包装好的，而是在文本内部由语言结构的排列产生的
  - **同标异向**：同一个标的被赋两个相反的向。"人来人往的世界很大/挤得下我的卑微身影，人来人往的世界很挤/容不下我的竭力呼喊"——"世界"这个标的在四句中被赋了两个方向：包容（给卑微身影留出空间）和排斥（拒绝竭力呼喊）。同一标在不同位置被赋不同向，读者的运算不是在"枯/残"的单一方向上做加法，而是在两个方向之间做切换
  - **理论意义**：前者是"调用文化储备"——作者从文化储备中提取已染色的意象；后者是"构造语言结构"——作者通过语言排列本身产生方向性，不需要调用任何传统意象储备。IVT的价值在于两种都能分析——分析后者时，该框架拓展了传统诗学"意象"概念的分析边界

---

## 三、向量叠加与维度锁定（数学 × 认知科学 × 诗学）

- **3.1 同频叠加**：方向一致的意象叠加，合成向量方向不变、模长增加、情感坐标锁定
  - 案例："枯藤+老树+昏鸦"——三个衰败方向向量锁定萧瑟坐标
  - 认知机制：维度越多，歧义越少（低维→模糊，高维→精确）
- **3.2 异频叠加**：方向冲突的意象叠加，合成向量方向不确定
  - 案例："雄鹰+残阳"——可指向英雄迟暮/悲剧力量/衰败中的尊严
  - 关键发现：异频配对的有效性取决于是否被足够多的额外维度锁定
  - 公式推论：异频向量夹角越大，需要的额外维度越多
- **3.3 维度锁定的拓扑学解释**
  - 高维空间可表达低维空间不存在的情感位置
  - 与层论表征[30]（sheaf theory）和POET[29]拓扑模型的平行关系
  - 维度锁定的数学本质：在情感流形上划定子区域
- **3.4 创作实践验证**：蟛蜞《调试日志》中，"非法配置落入灰色注释"+"超时请求沉进标红报错"两个异源但同频的报错场景叠加，比单一报错场景更精确地固定了"被技术世界困住"的情感坐标

---

## 四、动词作为移动向量（认知科学 × 计算机科学 × 文学）

- **4.1 从静态向量到动态轨迹**
  - 定义：动词/动作 = 在情感空间中推动读者移动的向量操作
  - 形式化：`点（主体）× 移动向量 · 方向（向）· 终点（标）`
  - 案例：`乌鸦（点）× 落入（移动）· 残（向）· 阳（标）`
- **4.2 Gärdenfors[13]双向量事件模型的诗学应用**
  - 力向量（force vector）→ 动词的情感推动力
  - 结果向量（result vector）→ 移动后的情感坐标变化
- **4.3 三种轨迹类型（原创分类）**
  1. **静态向量群→末端爆发**（马致远：枯藤老树昏鸦→断肠人在天涯）：读者被定位→被推送→冲刺爆发
  2. **含移动的单一表达式**（乌鸦落入残阳）：读者跟随单一轨迹→抵达终点
  3. **动作穿插全诗不收敛**（蟛蜞《调试日志》）：读者跟随散乱轨迹→情感无法锁定→徘徊→孤独/流离感的核心机制
- **4.4 认知心理学基础**：Stockwell[17]的心理模拟与指示投射；读者的具身模拟机制

---

## 五、读者情感生产责任转移（神经科学 × 认知理论）

- **5.1 咏物诗中的两阶段协作**
  - **向量构建——作者完成**：选择标的、赋予方向感、控制维度关系、设置轨迹类型
  - **向量运算——读者完成**：读取向量方向、计算叠加关系、推测合成向量、翻译为情感体验
- **5.2 读者认知运算过程（无意识完成）**：
  1. 读取每个意象的向量方向
  2. 计算向量之间的叠加关系
  3. 在向量空间中预测合成向量的方向
  4. 将合成向量方向"翻译"为情感体验
- **5.3 为什么自主推测的情感更牢固**
  - 被动接收：情感是"作者的"——读者只是旁观者
  - 自主推测：情感是"自己发现的"——读者无法否认
  - 与Jacobs NCPM[15]模型"意义格式塔闭合"的关系
- **5.4 验证条件**：删去所有情绪词后，物象是否仍能独立撑起完整情感场
  - 案例检验：蟛蜞debug诗删去"悲殇残哀"后，情感场完整——验证通过

---

## 六、意象向量论的理论定位与综合展望（诗学 × 数学 × 认知科学 × 计算机科学）

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
| 标/向分离 | 诗学 | Rochallyi[1]向量诗学、程洁[3]三重转换 |
| 叠加与维度锁定 | 数学×拓扑学 | 层论[30]表征、洛特曼[5]符号圈、POET[29]贝蒂数 |
| 动词-动量与轨迹 | 语言学×认知科学 | Gärdenfors[13]双向量模型、Stockwell[17]指示投射 |
| 读者责任转移 | 认知科学×美学 | Jacobs[15] NCPM、Text World Theory[19] |

**纵向——三级感知链路**：文化编码层（"向"源于语言共同体的历史编码）→ 符号共鸣层（同频共振加强，异频张力创新）→ 认知渲染层（留白迫使读者自主完成情感闭合）

### 6.3 理论定位、比较与局限

**定位**：分析框架而非方法论或创作指南；认知理论而非工程应用或数字人文工具；仅覆盖意象与情感这一特定子问题而非全域理论。在九个理论框架中，IVT是同时使用向量/几何语言、讨论维度锁定、讨论读者责任转移的分析框架。

**局限**：①情感维度定义待经验充实 ②ReaderCompute目前暂没有对应理论研究能精确解析 ③三种轨迹覆盖范围有限 ④最优运算量假设未经实证检验

> **与第七章**：本标准模型（ch2-6）→ 嵌套扩展（ch7），后者打破"我=隐含参考系原点"的假设，将IVT从意象层面扩展到主体层面。

---

## 七、IVS嵌套空间论：主体建模化与情感空间嵌套（诗学 × 认知科学 × 创作实践）

> **核心命题**：将"我"从IVT的隐含参考系原点拉平为可被标/向框架处理的操作对象，建立双层标/向嵌套的情感空间模型。

### 7.1 问题的发现：IVT框架的隐含假设
IVT标准框架将"我"默认为情感向量空间（IVS）的隐含参考系原点。蟛蜞式诗歌（"我不是我""我站在时间之外""从梦乡中归来"）证明这一假设可被打破，"我"可以被建模为新的标 $\text{Obj}_{\text{我}}$。

### 7.2 打破隐含假设
传统诗与蟛蜞式诗歌的情感生产链路公式化对比，揭示传统IVT处理不了"我"被建模为可操作对象时的四层运算结构。

### 7.3 三层空间模型
- **第一空间**（作者→向量场）：作者构造意象标/向，标准IVT覆盖范围
- **第二空间**（向量场→读者）：读者运算向量锁定情感坐标
- **第三空间**（作者→"我"→读者）：作者将"我"建模为标 $\text{Obj}_{\text{我}}$ 并赋轨迹 $\text{Traj}(\text{Obj}_{\text{我}})$，三空间通过内外双层标/向反馈耦合

### 7.4 主体建模化
将"我"建模为 $\langle \text{Obj}_{\text{我}},\ \text{Traj}(\text{Obj}_{\text{我}}) \rangle$，外层标的（$\text{Obj}_{\text{我}}$）与内层意象标/向并行运算。标的嵌套使读者运算从1层升级为至少4层（外层标识别→内层分析→外层轨追踪→耦合校准）。

### 7.5 三种主体模式
- **常规主体**：$\text{Obj}_{\text{我}}$ 不可观测，读者自动投影到原点 $O$，1层运算
- **被动构建体**：$\text{Obj}_{\text{我}}$ 可观测，轨迹低闭合度外力驱动，2层+耦合
- **主动构建体**：$\text{Obj}_{\text{我}}$ 可分解为多重标，多重轨迹/自指，2+层+耦合

### 7.6 空间嵌套的运作方式
双层标/向耦合的运作机制：情感劳动谱系新增"嵌套转移"层级（透明→轻度→中度→高度→极限→嵌套转移），读者需同时运算内层意象合成和外层"我"的轨迹。

### 7.7 技法体系的对应
技法操作与 IVS 嵌套层级对应映射表，被动构建 vs 主动构建在技法层面的统一解释。

### 7.8 嵌套空间论的理论意义
- 情感劳动从一维（运算量）扩展为二维（运算量 × 标/向层数）
- "我"不是特权原点，可以被建模为标
- 元层级作为创作者的第三只手

### 7.9 隐式/显式构建切换分析

> **核心发现**："我"的构建状态不是一次性二元激活/不激活的开关。同一首诗可在不同阶段在隐式构建↔显式构建之间反复切换，切换次数 $N_{\text{switch}}$ 作为结构复杂度的新度量维度。

#### 7.9.1 问题的提出
仅判断"是否激活嵌套"的二元激活模型无法处理苏轼《念奴娇·赤壁怀古》这类完整切换序列的诗，需从静态门禁升级为动态追踪。

#### 7.9.2 核心概念定义
- **隐式构建**："我"不出现在文本中，读者自动代入默认原点 $O$
- **显式构建**："我"被推到前台成为 $\text{Obj}_{\text{我}}$，读者追踪轨迹
- **再隐式化**："我"从前景退回默认原点

#### 7.9.3 切换序列模型
三阶段循环 $S_{\text{隐}} \xrightarrow{T_{\text{显}}} S_{\text{显}} \xrightarrow{T_{\text{再}}} S_{\text{再}}$，$\text{Traj}_{\text{构建}} = S_{\text{隐}}^{(n_1)} \xrightarrow{T_{\text{显}}^{(1)}} S_{\text{显}}^{(n_2)} \cdots$

#### 7.9.4 典型案例
苏轼《念奴娇·赤壁怀古》五步切换路径：全场域远摄 → 历史场景拉近 → 叙事细节展开 → 显式构建引爆点：“多情应笑我” → 再隐式化：“人生如梦，一尊还酹江月”。$N_{\text{switch}}=2$。

#### 7.9.5 隐式构建细则
- **视角切换即构建操作**：以《山坡羊·潼关怀古》为例，自然物象 → 人文物象的视角跨越默认了"我"的存在情境变化
- **动词类别作为判定信号**：自动/物象动词 → $\mathbf{S_{\text{隐(观)}}}$，他动/社会性动词 → $\mathbf{S_{\text{隐(行)}}}$，视角引领动词→触发构建切换候选
- **补充激活条件**：视角切换和动作切换本身应触发"我"的隐式/显式关系检查
- **扩展意义**：揭示了向量构筑之外增加读者运算复杂度的嵌套构筑维度

#### 7.9.6 理论意义
- (a) 打破二元激活模型：嵌套分析不是一次性门禁
- (b) 隐式构建内部的异构性：功能异构（$\mathbf{S_{\text{隐(观)}}}/\mathbf{S_{\text{隐(行)}}}$）+ 视角异构（$\mathbf{V_{\text{自}}}/\mathbf{V_{\text{文}}}$）
- (c) 内部切换与构建切换的层叠模型：$\Delta_{func}(t)$ 与 $N_{\text{switch}}$ 正交叠加
- (d) 切换次数 $N_{\text{switch}}$ 作为分析维度

#### 7.9.7 与现有IVS结构的关系
嵌套空间论回答"是否存在嵌套"，切换分析回答"构建状态如何动态变化"，两者互补。分析流程：检测嵌套激活→（激活时嵌套分析+切换分析，未激活时检查视角切换→标准IVT分析）。

#### 7.9.8 对读者情感劳动的影响
- 新增第4层运算：构建状态切换（模式切换运算）
- 切换成本 $C_{\text{switch}}$ 形式化：隐→显成本较高，显→隐中等，多次切换非线性递增
- 隐式内部功能切换成本：$\sum \Delta_{func} \times C_{\text{func}}$ 与 $N_{\text{switch}} \times C_{\text{switch}}$ 叠加
- 情感劳动三维度量：$L = f(\text{运算量}_{\text{Ch5}},\ \text{标/向层数}_{\text{7.8.2}},\ \text{切换次数}_{\text{7.9.8}})$
- 谱系新增"切换转移"层级

### 7.10 IVS运算负荷逐步升级与读者情感劳动
L1-L6六级递进：标/向分离 → 向量叠加 → 动词-动量 → 读者责任转移 → 嵌套空间 → 隐式/显式构建切换。核心机制：信息量 → 信息组织方式 → 元认知监控。

---

## 八、在AI写诗与计算诗学中的潜在应用（计算机科学 × 诗学 × 创作实践）

- **8.1 生成策略转向**：从"修辞优化"（预测最可能的词）→ "向量空间构造"（锁定目标情感坐标的意象组合）
从预测修辞式生成到向量空间构造式生成至少解决了两个重大问题：1.修辞总是要引入额外的物或意象，引入内容一旦稍有偏差，就会导致向量叠加错乱，破坏全诗情感拓扑，导致成诗的语言结构一团乱麻；2.额外引入的内容减少了读者的情感劳动，意象空间被急剧压缩，读者在读诗时的自主性降低，情感生成空间受限
- **8.2 评价标准重塑**：从"语言流畅度" → "向量空间维度与锁定精度"
- **8.3 风格迁移革命**：从"模仿用词"→ "模仿向量布局"
  - 为什么AI仿写蟛蜞总差一口气：在模仿"用词"和"句式"，而非"向量布局"
  - 蟛蜞诗的"没有硅味"源于向量布局是感知实践的产物，而非语料库统计关联
- **8.4 创作经验与情感劳动的感知增长**：创作实践为分析者提供了感知诗歌中情感劳动的能力，非创作者读成品，创作者读生产过程。意象向量论将这一隐性感知翻译为显式知识，构成其理论起点之一

- **8.5 人类创作经验与AI分析能力的差异及IVT向评估工具的迁移**
  - **8.5.1 AI分析的情感盲区**：AI无法感知诗歌中的情感构造过程，只能检测表层语义关联
  - **8.5.2 "什么是差异"的分析差异**：AI统计vs人类结构感知的根本分歧，AI缺少"情感劳动"的感知通道
  - **8.5.3 从差异到迁移**：IVT的分析框架可迁移为AI情感生成评估工具（五维机制映射+三条逻辑链条）
  - **8.5.4 可行性与实用性分析**：五维机制与评估需求的结构性对应（标/向分离→语义清晰度、向量叠加 → ECI、动词-动量 → 叙事结构、责任转移 → 参与度、嵌套空间 → 主体建模）、可操作化路径（ivt-poem-analyzer工具链）、实用性与边界

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
- **9.3 学术空白定位**：现有学术文献中，尚缺乏将诗学、认知科学、计算机科学、数学四个分散传统整合为"标→向→移动→维度锁定→认知渲染→读者推测"的完整因果链。而"创作实践"作为理论源头，进一步确保了该框架不是纯理论的空中楼阁，而是从真实的创作直觉中翻译出来的可操作模型
## 9.4 未来方向

意象向量论的分析框架在理论建构完成后，已通过 `ivt-poem-analyzer` 技能的形式实现为可操作的诗歌分析工具，并基于蟛蜞50+首精选原创诗歌以及50+首中外名篇完成了验证。这一验证确认了理论框架的核心机制：标/向分离的可操作性、同频/异频叠加的可识别性、三种轨迹类型的可分类性、读者责任转移的可度量性、以及IVS嵌套空间论中主体建模化的可检测性在真实创作素材中均具有稳定的解释力。

分析工具的成型与验证，使IVT框架完成了从"理论假设"到"可重复分析操作"的跨越。当前的核心方向已从分析层面的验证转向**生成算法层面的研究**，将IVT的核心主张从分析框架转化为生成算法的约束条件。

### 9.4.1 向量空间构造式生成的形式化建模

将第八章提出的五步生成范式：确定目标情感坐标→选择标的→分配向的方向→构造动词-动量轨迹→留白与责任转移——转化为可编码的算法约束。核心挑战在于：情感空间中的"目标坐标"如何被形式化为生成模型的输入参数？标的选取与向的分配如何在向量空间中实现精确的合成方向控制？这一形式化的完成将使AI诗歌生成从"预测下一个最可能的词"转向"在情感空间中构造一个精确的几何结构"，也为AI模仿人类情感提供新的范式和可能性。

### 9.4.2 嵌套空间结构的生成参数化

第七章揭示的IVS嵌套空间结构，特别是主体建模化中 $\text{Obj}_{\text{我}}$ 的可观测性、$\text{Traj}(\text{Obj}_{\text{我}})$ 的轨迹赋值、以及三种主体模式（常规/被动构建/主动构建）的连续谱，为AI生成中的"我"提供了可参数化的控制维度。嵌套空间的结构参数（外层标的可观测性、轨迹闭合度、标的分解程度）可被编码为生成模型中的额外控制变量，使AI能够有意识地在生成中控制读者端的情感劳动层级（单层运算 vs 双层耦合运算）。

### 9.4.3 负优化与留白程度的算法控制

第五章提出的负优化概念，有意识地不提供足量向量信息以增加读者端的运算量这一写作方式在生成算法中具有独特的应用价值。核心问题在于：如何量化一首诗的"留白程度"（即候选区域 $A_{\text{候选}}$ 的大小）？如何在生成过程中精确控制"向"信息的提供量，使读者端的运算量处于最优区间？可能的探索路径包括：通过向量密度估算 $A_{\text{候选}}$、通过异频夹角总和估算方向不确定性、以及通过动词-动量的方向一致性量化轨迹的收敛程度。

### 9.4.4 向量布局的风格迁移与风格发现

第八章提出的"向量布局"概念：风格差异 = 标的分布偏好 × 向的分配策略 × 轨迹类型选择 × 留白程度——将诗歌风格从"用词层面的模仿"提升为"几何结构层面的模仿"。在生成算法中，意味着可以不依赖于词频分布来度量风格，而通过分析特定诗人的意象向量布局参数，使生成算法可以在"向量布局空间"而非"词向量空间"中实现风格迁移。更进一步，这一方法可能发现传统风格分类无法捕捉的"跨诗人的结构相似性"，两位用词迥异的诗人可能在向量布局参数上高度一致。

### 9.4.5 IVS嵌套构建可能存在更多的维度

上述四个方向构成了从分析框架向生成算法迁移的核心探索路径。但 IVS 嵌套构建的复杂性是否已被充分揭示？从第七章的分析来看，主体建模化中的 $\text{Obj}_{\text{我}}$ 可能还承载着更多尚未被形式化的维度，如"我"的时间性（过去的我与现在的我的轨迹差异）、"我"的群体性（"我们"是否可以被建模为主体的复合标）、以及"我"的主体间性（两个"我"在同诗中的交互）等。这些方向在现有框架中被识别为可能的延伸点，但尚未进行系统性分析，有待后续研究根据生成算法实验的初步结果进行收敛与调整。

> **注**：以上五个方向属于探索性拟定，后续版本中需根据生成算法实验的初步结果进行收敛与调整。当前IVT分析工具的批量化验证使算法研究有了可靠的评估基准，即生成结果是否成功，可通过既有的IVT分析工具做逆向检验：生成文本的标/向分离是否合理、向量方向是否一致、读者责任转移是否处于最优区间。

## 附录：四大核心素材

### 附录A：元创作案例——debug诗（理论原点）

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

**理论意义**：全诗无传统"诗意"意象（月光、落叶、孤影），以"调用栈""函数名""二进制洪流""灰色注释""标红报错"等技术物象作为核心意象群，是意象向量论"物象本身即情绪"的典型例证。经"删去所有情绪词"验证条件检验——删掉"悲殇残哀"后情感场完整——通过。

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

[1] ROCHALLYI R. Vector Poetry[EB/OL]. MAA Math Values, 2023-06-29. https://maa.org/math-values/vector-poetry/. [2026-07-11].

[2] KURZYNSKI M. The game of keys and queries: parallelism and cognitive geometry in Chinese regulated verse[J/OL]. International Journal of Humanities and Arts Computing, 2025, 19(2). https://doi.org/10.3366/ijhac.2025.0355. [2026-07-11].

[3] 程洁. 汉语古典诗歌意象系统研究：物象—心象—语象的三重转换机制[M]. 北京: 北京大学出版社, 2018.

[4] 刘勰. 文心雕龙[M]. 北京: 人民文学出版社, 1958.

[5] LOTMAN Y. Universe of the mind: a semiotic theory of culture[M]. Bloomington: Indiana University Press, 1990.

[6] FAUCONNIER G, TURNER M. The way we think: conceptual blending and the mind's hidden complexities[M]. New York: Basic Books, 2002.

[7] POUND E. A retrospect[M]//Literary essays of Ezra Pound. London: Faber and Faber, 1954.

[8] ELIOT T S. Hamlet and his problems[M]//The sacred wood: essays on poetry and criticism. London: Methuen, 1920.

[9] 王国维. 人间词话[M]. 上海: 上海古籍出版社, 1998.

[10] 严羽. 沧浪诗话[M]. 北京: 中华书局, 2014.

[11] 司空图. 二十四诗品[M]. 北京: 人民文学出版社, 1963.

[12] FAUCONNIER G. Mental spaces: aspects of meaning construction in natural language[M]. Cambridge: Cambridge University Press, 1994.

### 二、认知科学与神经认知诗学

[13] GÄRDENFORS P. Conceptual spaces: the geometry of thought[M]. Cambridge, MA: MIT Press, 2000.

[14] GÄRDENFORS P. The geometry of meaning: semantics based on conceptual spaces[M]. Cambridge, MA: MIT Press, 2014.

[15] JACOBS A M. Neurocognitive poetics: methods and models for investigating the neuronal and cognitive-affective bases of literature reception[J]. Frontiers in Human Neuroscience, 2015, 9: 186.

[16] JACOBS A M. SentiArt: a vector space model for the computation of emotion potential in texts[C]//Proceedings of the 2018 Conference on Empirical Methods in Natural Language Processing. Brussels: ACL, 2018.

[17] STOCKWELL P. Cognitive poetics: an introduction[M]. London: Routledge, 2002.

[18] STOCKWELL P. Cognitive poetics: a new introduction[M]. 2nd ed. London: Routledge, 2024.

[19] WERTH P. Text worlds: representing conceptual space in discourse[M]. London: Longman, 1999.

[20] GAVINS J. Text world theory: an introduction[M]. Edinburgh: Edinburgh University Press, 2007.

[21] ISER W. The act of reading: a theory of aesthetic response[M]. Baltimore: Johns Hopkins University Press, 1978.

[22] ISER W. The implied reader: patterns of communication in prose fiction from Bunyan to Beckett[M]. Baltimore: Johns Hopkins University Press, 1974.

[23] FRISTON K. The free-energy principle: a unified brain theory?[J]. Nature Reviews Neuroscience, 2010, 11(2): 127-138.

[24] VAN DE CRUYS S, FRASCAROLI J, FRISTON K. Order and change in art: towards an active inference account of aesthetic experience[J]. Philosophical Transactions of the Royal Society B: Biological Sciences, 2024, 379(1895): 20220411.

[25] PETERSEN M K. Latent semantics of action verbs reflect phonetic parameters of intensity and emotional content[J]. PLoS ONE, 2015, 10(4): e0121575.

[26] STOCKWELL P. Texture: a cognitive aesthetics of reading[M]. Edinburgh: Edinburgh University Press, 2009.

### 三、计算机科学与计算诗学

[27] MIKOLOV T, CHEN K, CORRADO G, et al. Efficient estimation of word representations in vector space[C]//Proceedings of ICLR Workshop. Scottsdale: ICLR, 2013.

[28] DEVLIN J, CHANG M W, LEE K, et al. BERT: pre-training of deep bidirectional transformers for language understanding[C]//Proceedings of NAACL-HLT. Minneapolis: ACL, 2019: 4171-4186.

[29] WANG R, LEHMAN J, CLUNE J, et al. POET: paired open-ended trailblazer model for open-ended evolution[J/OL]. arXiv preprint arXiv:1901.01753, 2019.

[30] AYZENBERG A, GEBHART T, MAGAI G, et al. Sheaf theory: from deep geometry to deep learning[EB/OL]. (2025-02-21)[2026-07-11]. https://arxiv.org/abs/2502.15476.

[31] KURZYNSKI M, XU X, FENG Y. Vector poetics: parallel couplet detection in classical Chinese poetry[C]//Proceedings of the 4th International Conference on Natural Language Processing for Digital Humanities (NLP4DH 2024), 2024: 200-208.

### 四、数学与情感科学

[32] COWEN A S, KELTNER D. Semantic space theory: a new approach to understanding emotion[J]. Nature Reviews Psychology, 2024, 3: 88-103.

[33] COWEN A S, KELTNER D. Self-report captures 27 distinct categories of emotion bridged by continuous gradients[J]. Proceedings of the National Academy of Sciences, 2017, 114(38): E7900-E7909.

[34] 段玉聪. 段玉聪 DIKWP 哲学体系解析[EB/OL]. ResearchGate, 2025-11. DOI:10.13140/RG.2.2.15793.65127.

### 六、神经科学实验与实证研究

[35] MERLEAU-PONTY M. Phenomenology of perception[M]. SMITH C, 译. London: Routledge, 1962.

[36] BARSALOU L W. Perceptual symbol systems[J]. Behavioral and Brain Sciences, 1999, 22(4): 577-660.

### 七、语言大模型微调实践方向

[37] HU E J, SHEN Y, WALLIS P, et al. LoRA: low-rank adaptation of large language models[C]//Proceedings of the International Conference on Learning Representations (ICLR 2022), 2022.

[38] DETTMERS T, PAGNONI A, HOLTZMAN A, et al. QLoRA: efficient finetuning of quantized LLMs[C]//Proceedings of NeurIPS 2023, 2023.

[39] LIU S Y, WANG C Y, YIN H, et al. DoRA: weight-decomposed low-rank adaptation[C]//Proceedings of the International Conference on Machine Learning (ICML 2024), 2024.

[40] ZHANG Q, CHEN M, BUKHARIN A, et al. AdaLoRA: adaptive budget allocation for parameter-efficient fine-tuning[C]//Proceedings of ICLR 2023, 2023.

[41] HAN Z, GAO C, LIU J, et al. Parameter-efficient fine-tuning for large models: a comprehensive survey[J/OL]. arXiv:2403.14608, 2024.

[42] LIALIN V, DESHPANDE V, RUMSHISKY A. Scaling down to scale up: a guide to parameter-efficient fine-tuning[J/OL]. arXiv:2303.15647, 2023.

[43] DAI N, LIANG J, QIU X, et al. StylePTB: a compositional benchmark for fine-grained controllable text style transfer[C]//Proceedings of NAACL 2022, 2022.









