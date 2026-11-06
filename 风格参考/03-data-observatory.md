---
name: "Data Observatory / 数据观测站"
id: "data-observatory"
version: "1.0"
purpose: "统计、科研、AI 与数据洞察类中文竖屏视频"
preferred_format: "9:16"
resolution: "1080x1920"
best_for:
  - "统计学、研究方法与科研"
  - "AI、数据科学与技术概念"
  - "数字趋势与因果关系"
avoid_for:
  - "儿童内容"
  - "生活方式与温暖人物故事"
colors:
  canvas: "#08131D"
  surface: "#102432"
  surface_high: "#183446"
  ink: "#F0F6F7"
  muted: "#91A8B7"
  primary: "#58D8BB"
  primary_soft: "#173F3B"
  secondary: "#FFB25B"
  secondary_soft: "#4A3521"
  grid: "#244354"
  danger: "#FF6B6B"
typography:
  display: "Noto Sans SC, Microsoft YaHei, sans-serif"
  body: "Noto Sans SC, Microsoft YaHei, sans-serif"
  data: "Bahnschrift, DIN Alternate, Consolas, monospace"
  hero: "112px–150px / 700"
  scene_title: "74px–94px / 700"
  section_title: "48px–60px / 700"
  body_copy: "30px–36px / 400–600"
  data_number: "92px–168px / 600"
  metadata: "21px–25px / 600"
spacing:
  frame_padding: "54px–64px horizontal / 52px–66px vertical"
  panel_gap: "16px–26px"
  section_gap: "28px–44px"
components:
  card_radius: "10px–16px"
  border: "2px solid"
  structural_rule: "2px solid"
  depth: "solid tonal layers; localized glow only"
density:
  content_fill_target: "70%–86%"
  max_unintentional_blank_area: "16%"
  stable_reading_time: "2.3s minimum"
motion:
  energy: "focused"
  fast: "0.28s"
  standard: "0.48s"
  slow: "0.88s"
  stagger: "0.04s–0.07s"
  travel: "20px–40px"
  transition: "scan gate"
---

# 数据观测站

## 1. 核心概念

画面像一座面向数据的夜间观测站：每个场景先捕获一个信号，再放大、比较并得出结论。薄荷绿代表可信信号与成立关系，琥珀色代表解释、变量和需要注意的条件，红色只用于错误或风险。

科技感来自数据尺度、轨迹和观测逻辑，不来自满屏霓虹或虚假的仪表盘。

## 2. 视觉语法

- 深蓝黑画布贯穿全部场景，使用局部实色层次，不用全屏线性渐变。
- 每幕选用 2–4 个观测元素：坐标轴、采样点、刻度环、扫描线、数据轨迹、窗口编号。
- 主数据必须足够大，图形与文字共同承担信息，不以装饰性代码填空。
- 面板宽度和高度按信息权重变化，不做均匀 dashboard 网格。
- 局部辉光只用于主数据和选中轨迹，环境亮度不得降低文字对比。

## 3. 色彩语义

- Primary 薄荷绿：有效信号、主要数据、已验证关系。
- Secondary 琥珀色：条件变量、解释、比较对象和提醒。
- Danger 红色：错误、偏差、风险；一条视频中应极少使用。
- Surface 与 Surface High 负责深色层次，不能用透明玻璃卡替代。
- 每幕至少有一处全饱和主色焦点，避免低透明度导致压缩后消失。

## 4. 中文排版

- 中文标题采用高字重黑体，数字使用窄体或等宽字体。
- 主数据 92–168px，单位 28–40px；数字和单位必须基线对齐。
- 正文 30–36px，行高 1.35–1.5，每段最多三行。
- 元数据可以使用英文大写，但只放真实栏目词，如 SAMPLE、TREND、RESULT。
- 不使用伪代码、随机十六进制或没有意义的数字串装饰画面。

## 5. 构图规则

- 首读是数据或问题，次读是图形关系，最后读解释或结论。
- 优先使用 40/60 分屏、上方数据带加下方图形、中央大数字加边缘读数。
- 图表必须简化为一个观点：一个趋势、一个差异或一个关系。
- 坐标、网格和刻度应与主图形对齐，不得漂浮。
- 黑底场景仍需覆盖 70% 以上视觉面积，不能只在中心放一张小卡片。

## 6. 核心组件

### 信号读数

- 大数字、短结论和一条微型趋势线组成同一组。
- 薄荷绿用于数字，琥珀色用于条件或对比。

### 关系轨迹

- 由 3–6 个节点连接成曲线或折线。
- 每个节点只保留短标签，解释统一放在独立区域。

### 学科雷达

- 用环形刻度或放射线表示多个学科的连接，但不伪造量化分值。
- 若没有真实数据，只表达“关联”而不是强弱排名。

### 结论舱

- 使用高层级实色面板承载一句结论。
- 结论下方最多一条条件说明，避免变成长文本卡片。

## 7. 动效方向

- 先出现扫描门或坐标轴，再让采样点、轨迹和数字依次锁定。
- 数字允许短促计数，但必须从真实起点到真实终点，并可确定复现。
- 轨迹用 SVG 绘制或缩放揭示，数据点在轨迹到达时点亮。
- 环境层仅做缓慢水平扫描或低幅呼吸，不做随机粒子。
- 转场使用一条横向扫描门或局部黑场遮盖，不使用大面积闪白。

## 8. 推荐场景

- 首屏问题：一个巨大问号或数字，扫描线定位主题。
- 数据证据：趋势线与核心数字同步建立。
- 跨学科连接：学科节点围绕统计或研究方法形成关系图。
- 结论：信号汇聚成一句明确判断，并显示适用条件。

## 9. 禁止项

- 禁止紫蓝渐变、满屏粒子、赛博朋克霓虹和透明玻璃面板。
- 禁止虚构精确数值和没有来源的增长百分比。
- 禁止为了科技感放置不可读的小字。
- 禁止同时展示多个复杂图表。
- 禁止让辉光穿过正文或降低对比度。

## 10. 执行检查

- [ ] 每个图形都对应真实内容关系。
- [ ] 主数据、图形、解释形成明确阅读顺序。
- [ ] 薄荷绿与琥珀色语义没有互换。
- [ ] 中文正文至少 30px，元数据至少 21px。
- [ ] 没有伪数据、随机粒子和无意义代码。
- [ ] 动画可寻址，并保留至少 2.3 秒稳定阅读时间。
