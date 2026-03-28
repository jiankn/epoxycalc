# Epoxy Calculator UI/UX Brief v1

## 0. 目的
这份文档用于补充 V2 PRD 中关于“有效停留”和“高信任转化”的设计要求，并审阅现有 UI/UX prompt 是否与产品方向冲突。

核心目标不是单纯拉长停留时间，而是让用户在一个页面内自然完成：

1. 测量输入
2. 结果理解
3. 方案比较
4. 风险确认
5. 采购决策

## 1. 先给结论
你现在这版 prompt 大方向是对的，但有 5 个需要改的地方：

### 1.1 可以保留的部分
- `Industrial Minimalist + Mobile-First Native` 方向是对的。
- 明亮环境下的高对比浅色主题是对的。
- 结果数字必须极强视觉层级，这点是对的。
- 移动端单手操作、48px 以上触控目标，这点是对的。
- 实时计算方向基本正确。

### 1.2 需要修改的部分
- `Inter / Roboto` 太普通，不符合“工具品牌感”。
- “只要出结果，CTA 紧贴结果卡片”过于激进，容易伤害信任。
- `Buy Deep Pour Epoxy - Save 10%` 这种文案太早进入销售状态，而且折扣文案未必合规。
- “用 steppers 替代小控件”不适合精细尺寸输入，尤其是小数和分段宽度。
- 深色结果卡可以有，但不能做成整个产品的视觉中心，否则与“车间强光下易读”目标冲突。

## 2. 设计原则

### 2.1 高信任优先
页面必须先让用户信任结果，再让用户点击购买。

### 2.2 结果不是终点
结果出现后，页面还要自然承接：
- 为什么是这个结果
- 如果更保守会怎样
- 需要买哪类产品
- 开工前还要注意什么

### 2.3 工具感而不是营销感
整体气质应更接近专业测量工具，而不是电商落地页。

### 2.4 减少机械操作
用户经常在车间、手机、带手套、站立状态下使用。交互应该少步骤、少模式切换、少精细点击。

## 3. 页面结构建议

### 3.1 首页
- Hero 区直接说明用途。
- 一个主入口卡片，直达 `River Table Planner`。
- 一个次入口卡片，进入基础体积计算。
- 一段“这个工具比普通计算器多做了什么”。
- 一段“如何测量 irregular river / void”。
- 一段“结果会输出什么”。

首页不是内容农场，不需要堆很多链接。

### 3.2 旗舰计算页
推荐信息结构如下：

1. 顶部标题与简短说明
2. 单位切换
3. 项目类型切换
4. 输入区
5. 实时结果摘要
6. 结果解释区
7. 方案对比区
8. 购买建议区
9. 常见错误
10. 项目 checklist
11. FAQ

这个顺序的目的，是把“出数字”变成“完成决策”。

## 4. 如何增加有效停留

### 4.1 不要做的事
- 不要为了拉时长故意隐藏结果。
- 不要把结果拆到第二页。
- 不要先留邮箱再看结果。
- 不要在计算途中弹出购买框。

### 4.2 应该做的模块

#### A. Why This Estimate Changed
在结果旁边展示：
- 原始体积
- waste buffer
- seepage / seal coat 加量
- 最终建议采购量

用户愿意停留，是因为他们在理解差异。

#### B. Compare Scenarios
允许用户一键比较：
- Quick vs Segment
- Normal vs Conservative
- Deep Pour vs Table Top

这类对比会自然提升停留和交互深度，而且非常贴近购买决策。

#### C. Measurement Guide
在输入区下方提供折叠式“如何测量”说明：
- 分段测量示意图
- 宽度取样频率建议
- 深度测量注意事项

#### D. Common Mistakes
围绕高风险错误写 4-6 条：
- 低估木材渗漏
- 忽略封闭层
- 忽略产品最大浇注厚度
- 只按平均宽度估算 irregular river

#### E. Project Checklist
结果后给一个简短 checklist：
- Mold sealed
- Wood sealed
- Room temperature checked
- Pour depth confirmed
- Mixing containers ready

这会让页面从“计算器”变成“开工前检查工具”。

## 5. 移动端交互建议

### 5.1 输入控件
- 数值输入应以大号数字输入框为主，而不是 stepper 为主。
- 支持数字键盘直出。
- 单位采用 segmented control。
- 项目类型采用大尺寸 pill tabs。

原因：
- 树脂项目常见输入包含小数、非整数和多段不同宽度。
- Stepper 适合数量，不适合精确尺寸。

### 5.2 分段输入
`Segment mode` 不应一次展示过多输入框。

推荐方式：
- 默认显示 3-5 段。
- 支持 “Add segment”。
- 每段用简洁卡片展示 `Width`。
- 页面底部有 sticky summary，实时汇总总体积。

### 5.3 实时计算
可以做实时计算，但实现方式要克制：

- 输入 `150-250ms debounce`
- 有稳定状态提示，不要抖动跳数
- 出现非法输入时，给局部提示，不要整页报错

### 5.4 单手操作
- 主要交互位集中在首屏和屏幕中下区域。
- 移动端 CTA 可用 sticky bottom bar，但必须在结果已经稳定可理解后出现。

## 6. 视觉系统建议

### 6.1 风格
- 工业极简
- 明亮车间环境可读
- 工具感强
- 不做消费级 SaaS 渐变风

### 6.2 颜色
推荐方向：
- 背景：`stone-50` / `zinc-50`
- 主文字：`slate-900`
- 次文字：`slate-600`
- 边框：`slate-200`
- 功能强调：偏工程感的蓝或安全绿

不要把页面做成泛电商“高转化绿按钮 + 白底卡片堆叠”的模板感。

### 6.3 字体
不建议用 `Inter` 或 `Roboto` 作为唯一主字体。

更合适的方向：
- `IBM Plex Sans`
- `Public Sans`
- `Geist`

其中 `IBM Plex Sans` 最贴近“工业、测量、精确”气质。

### 6.4 结果卡
结果卡需要强视觉锚点，但不建议做成纯黑大面积卡片。

更好的做法：
- 浅底高边框卡
- 或者深色仅用于结果数字模块本身
- 保证在强光下依然清晰

## 7. 商业模块设计

### 7.1 放置原则
Affiliate CTA 不能早于信任建立。

推荐顺序：
1. 结果
2. 结果解释
3. 购买建议

而不是：
1. 结果
2. 立刻大按钮卖货

### 7.2 CTA 文案
不建议默认使用：
- `Save 10%`
- `Best Deal`
- `Buy Now`

原因：
- 未核实优惠时可能不合规
- 营销感过强
- 降低工具可信度

更合适的文案：
- `View Deep Pour Options`
- `See Recommended Kit Sizes`
- `Check Price on Amazon`

### 7.3 双层转化结构
推荐使用：
- 主 CTA：独立站高匹配商品
- 次 CTA：Amazon fallback
- 附加文本：为什么推荐这个产品

让“推荐理由”紧贴 CTA，比把 CTA 做得更大更重要。

## 8. 关键埋点建议
- 首次输入
- 结果稳定生成
- `Quick` 切换到 `Segment`
- `How to measure` 展开
- `Why this estimate changed` 展开
- 方案对比切换
- CTA 曝光
- CTA 点击
- Checklist 互动

这些埋点比单独看 time on page 更有解释力。

## 9. 对原始 Prompt 的逐条审阅

### 9.1 Overall Style
基本正确。

修改建议：
- 保留 `Industrial Minimalist + Mobile-First Native`
- 加一条：`Tool-first, trust-first, not e-commerce-first`

### 9.2 Typography
需要改。

问题：
- `Inter / Roboto` 过于常规，缺少独特工具感。

修改建议：
- 改为 `IBM Plex Sans` first, `Public Sans` fallback。

### 9.3 Mobile-First Interaction
方向正确，但要微调。

问题：
- `steppers` 不适合精细尺寸输入。
- 完全取消按钮是可行的，但要保证稳定和可理解。

修改建议：
- 以大号 numeric inputs 为主，stepper 仅用于少数计数型场景。
- 明确 debounce 和错误态策略。

### 9.4 Visual Hammer & Monetization
需要改。

问题：
- 结果卡可以强，但不宜过黑过重。
- 购买按钮直接贴结果太像 landing page。
- `Save 10%` 类型文案过早、过营销。

修改建议：
- 结果卡后先显示解释摘要，再给 CTA。
- CTA 文案改为更中性、更可信的动作文案。

## 10. 修订版 Prompt

```md
## UI/UX Design System Prompt (Revised)

### 1. Overall Style
- Style: Industrial Minimalist + Mobile-First Native.
- Product mood: precise, trustworthy, tool-first, workshop-friendly.
- Prioritize clarity and confidence over marketing energy.
- Use a bright, high-contrast light theme that remains readable in workshop lighting.
- Avoid dark mode as the primary theme.

### 2. Visual Direction
- Background: warm stone or zinc neutrals.
- Primary text: deep slate / near-black.
- Accent: engineering blue or safety green, used sparingly.
- The UI should feel like a precision measuring tool, not a generic SaaS dashboard or e-commerce landing page.

### 3. Typography
- Prefer a more distinctive, tool-appropriate sans-serif such as IBM Plex Sans or Public Sans.
- The final result number must be the strongest visual element on the page.
- Support data-heavy reading with clean spacing, high contrast, and compact but touch-friendly labels.

### 4. Mobile-First Interaction
- Optimize for one-handed use on a phone in a workshop environment.
- Minimum touch target: 48px.
- Use large numeric inputs for measurements.
- Use segmented controls for units and project type.
- Do not rely on tiny dropdowns for critical input.
- Avoid steppers for precise dimensions; they are acceptable only for simple counters.

### 5. Calculation Behavior
- Update results in real time with a gentle debounce.
- Keep the result stable and easy to scan while users type.
- Show local inline validation, not disruptive error states.
- The experience should feel instant, but never jittery.

### 6. Result Experience
- Treat the result as the start of the decision flow, not the end.
- The result area should include:
  - final recommended volume
  - raw volume
  - buffer explanation
  - Part A / Part B split
  - layer guidance
  - cost estimate
- Allow users to compare at least two scenarios such as Quick vs Segment or Standard vs Conservative.

### 7. Post-Result Engagement
- Directly below the result, include high-relevance follow-up modules:
  - Why this estimate changed
  - How to measure correctly
  - Common mistakes
  - Compare scenarios
  - Project checklist
- These modules should increase meaningful engagement, not artificially delay conversion.

### 8. Monetization
- Do not attach aggressive sales messaging immediately below the first result number.
- Build trust first, then show recommended purchase options.
- Show product recommendations only after explaining why that product type fits the project.
- Use neutral CTA copy such as:
  - View Deep Pour Options
  - See Recommended Kit Sizes
  - Check Price on Amazon
- Avoid unverified savings language like "Save 10%" unless the discount is confirmed and compliant.

### 9. Result Card
- The result card should be visually dominant but remain readable in bright environments.
- Prefer a strong bordered card or a restrained dark inset panel rather than a large heavy black block.
- Emphasize the number, the recommendation, and the explanation hierarchy.

### 10. UX Goal
- Optimize for effective dwell time:
  users should naturally stay longer because they are understanding, comparing, and preparing to act.
- Never optimize for fake dwell time by hiding results, gating access, or splitting a simple workflow across multiple pages.
```

## 11. 最终建议
如果这个项目的 UI/UX 只有“结果很大、按钮很大”，那还是停留在普通计算器思路。

更对的方向是：
- 像一个值得信任的专业工具
- 在结果之后继续帮助用户完成决策
- 用解释、对比、checklist 带来更深浏览
- 最后再做商业转化
