---
marp: true
theme: TJ-Minimal
size: 16:9
paginate: true
math: mathjax
header: 'TONGJI UNIVERSITY | 同济大学'
footer: '© 2026 Haoyu Tang | TJ-Minimal Marp Theme'
---

<!-- _class: title -->

# TJ-Minimal Marp 主题模板
## A Minimalist Marp Theme by Haoyu Tang

---

<!-- _class: index -->
# 目录 Contents

1. 字体排版与留白 (Typography & Spacing)
2. 公式与代码高亮 (Math & Code Syntax)
3. 极简表格与引用 (Tables & Blockquotes)
4. 多列网格版型：1:1 (Two columns: 50% / 50%)
5. 多列网格版型：4:6 (Two columns: 40% / 60%)

---

<!-- _class: chapter -->

# PART 01
## 基础页面与排版展示 (Typography & Elements)

---

# 1. 字体排版与留白

在正文字体排版中，我们追求极致的**呼吸感**与**留白**。在学术汇报或专业演讲中，过多的视觉干扰往往会分散观众的注意力。因此，TJ-Minimal 移除了多余的色块与复杂的背景修饰，将整体基调聚焦在干净、纯粹的内容本身。

- **加粗文本 (Bold)**：用于强调核心理论与关键指标，对比分明，让视线第一时间捕捉重点。
- *斜体 (Italics)*：用于引用文献、外文专有名词或特定的语境提示，展现学术严谨性。
- 带有删除线的~~废弃信息~~以及干净的[同济大学官方网站链接示例](https://www.tongji.edu.cn/)。
- **中英文混排体验**：The typography preserves elegant metrics for mixed texts. You can see how English words seamlessly blend with Chinese characters without breaking the baseline. 

整个页面能保持最轻松高贵的阅读基调。适当增加的行高 (Line Height) 与精心调试的字间距，能够确保在大段文字展示时，不仅避免杂乱，反而更显专业。

---

# 2. 公式与代码高亮

在理工科的展示中，公式与代码往往是不可或缺的核心部分。启用 `math: mathjax` 之后，无论是文本中的简单行内公式，例如爱因斯坦质能方程 $E = mc^2$，还是较为复杂的傅里叶变换、统计学分布等独立分布的块级方程，都能以最标准、优雅的无衬线/衬线混合形态渲染。

$$
f(x) = \frac{1}{\sigma \sqrt{2\pi}} e^{-\frac{1}{2}\left(\frac{x-\mu}{\sigma}\right)^2}
$$

对于计算机科学以及数据分析等相关专业的演示，代码块同样继承了主题清淡柔和的色调属性。带有圆角矩形的容器和护眼的语法高亮，使长时间阅读代码不造成视觉疲劳：

```python
def generate_distribution(mu=0, sigma=0.1, size=1000):
    # 此函数用于生成一个正态分布随机数例以作代码排版演示
    # 可以观察到代码块具有舒适的内补白（Padding）与圆角设计
    import numpy as np
    return np.random.normal(mu, sigma, size)
```

---

# 3. 极简表格与引用

在展示结构化数据时，我们彻底抛除了沉重的背景填色与冗余的纵向分割线。数据本身才应当是视觉的焦点。利用恰到好处的加粗线条，我们仅仅突出了表格的上下层次与内容边界，让数据呈现天然的阵列感。

| 核心设计元素 (Element) | 排版与视觉风格 (Design Style / Guidelines) | 使用强调色 | 视觉克制层级 |
|-----------------------|-------------------------------------------|----------|-------------|
| **表头 (Headers)**    | 顶部与底部双粗线条控制，提供强有力的边界感      | 否 (No)  | 高 (High)   |
| **主体数据列 (Rows)**   | 极细单根浅色水平分割线，弱化视觉隔阂，保证连贯   | 否 (No)  | 中 (Medium) |
| **底部边缘 (Footer)**   | 底部加粗横线完美收尾，形成完美的视觉闭环        | 否 (No)  | 高 (High)   |

> 极简引用块采用细长的同济蓝色（或者您自定义的主题强调色）作为左侧边界约束。
> 当您需要引用名人名言、关键结论或是大段摘抄文献时，这种轻量级的引用设计既能明确地跟正文区分开来，又不会破坏页面的整体留白比例。
> (Quotes use a thin accent color bound on the left border to distinguish them gracefully.)

---

<!-- _class: chapter -->

# PART 02
## 多栏网格布局 (Grid Layouts)

---

<!-- _class: two-cols -->

# 4. 版式引擎：经典的等分网格 (two-cols)

<div class="ldiv">

### 左侧：文字大纲与详细陈述
使用 `two-cols` 类可以将内容精准且稳固地按 50%:50% 比例切分为结构对称的左右半场。所有的核心标题、列表与段落元素都将自动对焦于顶部区域。

- 这种经典的居中劈分设计迎合了大多数人在日常演示文稿时的常规阅读习惯。
- 特别适合大段的条文概念说明配合旁边约束得当的高清图片，以此来辅助听众理解抽象概念。
- 文本在左半场即使折行，也会自动遵守设定的网格系统，绝不发生越界侵入右侧区域的排版事故。此设计充分利用了宽屏幕的横向空间。

</div>

<div class="rimg">

![w:400](https://picsum.photos/id/1015/600/400)

</div>

---

<!-- _class: two-cols-46 -->

# 5. 版式引擎：4与6分配比例 (two-cols-46)

<div class="ldiv">

当左半场的内容仅为寥寥数语的核心点缀或关键结论时，我们可以采用这种更加灵活的不对称设计。

> 对于需要极高表现力、复杂数据展示或大量推导步骤的区域，我们果断将 60% 的巨幅空间留给右侧。这种非对称的张力，让版面更加灵动。

</div>

<div class="rdiv">

### 扩展后的右侧专属展示区

在 60% 的充裕空间下，即使是那些最为冗长的大型偏微分等式、复杂的网络架构图、甚至是有着多个维度的宽幅统计表格，都将不再显得拥堵与局促。例如麦克斯韦方程组的积分形式：
$$
\oint_{\partial \Sigma} \mathbf{E} \cdot \mathrm{d}\boldsymbol{l} = - \int_{\Sigma} \frac{\partial \mathbf{B}}{\partial t} \cdot \mathrm{d}\mathbf{A}
$$

这不仅避免了对多行内容的过度挤压，同时也能确保任何置入的学术配图、图表分析拥有完美的留白与清晰的边界，从而提升演讲展示时的专业度。

</div>

---

<!-- _class: two-cols-46 -->

# 6. 版式引擎：4:6 满载压力排版演示

<div class="ldiv">

本页用于测试在 **极高信息密度** 下，两侧网格布局的稳定性与防溢界能力。

- **稳固边界**：即使左侧文字加入了多维度的长条目说明并包含大量标点折行，整体网格依然能够稳稳锁住这 40% 的边界范围。
- **无界边框**：因为去除了传统版式里冗杂的表格框线和色块，大量的留白反而成了分隔两边内容最好的“隐形墙”。
- **核心建议**：在学术工作汇报中，由于信息极其密集，强烈建议将左半场留给“大纲、结论、核心准则”，将大型推导、复杂数据或是高密图表统统装载到右侧。

</div>

<div class="rdiv">

### 右侧：高密度学术混合内容展示区

通过适当压缩行距和规整的网格引擎，在右侧您完全可以在一屏内塞下一个复杂物理公式、一个对比说明表格以及一段 Python 实验代码。

$$
\mathcal{L} = -\frac{1}{4}F_{\mu\nu}F^{\mu\nu} + i\bar{\psi}\not\!\!D\psi + |D_\mu\phi|^2 - V(\phi)
$$

| 模型指标 (Metric) | 推理精度 (Acc) | 数据耗时 (Time) | 显存 (Mem) |
|-----------------|--------------|---------------|-----------|
| Baseline Model  | 88.5%        | 1.2s          | 2.4GB     |
| **Our Method**  | **94.2%**    | **0.8s**      | **1.8GB** |

```python
# 即使在插入带边框的表格与大型公式后，依然有空间容纳代码块
def optimize_model(params, learning_rate=1e-3):
    return {"status": "success", "loss": params * learning_rate}
```

</div>

---

<!-- _class: ending -->

# Q&A
## Thanks for listening

