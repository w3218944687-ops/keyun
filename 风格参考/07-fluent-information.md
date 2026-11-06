---
name: "微软流动信息 / Microsoft Fluent Information"
id: "fluent-information"
version: "1.0"
last_updated: "2026-10-05"
best_for:
  - "步骤流程、操作指引"
  - "对比说明、功能矩阵"
  - "系统性知识、架构图解"
avoid_for:
  - "情感化表达、故事性内容"
  - "需要大量手绘感装饰的场景"
colors:
  background: "#F5F5F5"
  surface: "#FFFFFF"
  surface_raised: "#F0F0F0"
  border: "rgba(0,0,0,0.08)"
  border_strong: "rgba(0,0,0,0.14)"
  ink: "#1B1B1B"
  muted: "#616161"
  accent_blue: "#0078D4"
  accent_teal: "#038387"
  accent_orange: "#D83B01"
  accent_green: "#107C10"
  shadow_card: "0 2px 4px rgba(0,0,0,0.07), 0 8px 20px rgba(0,0,0,0.06)"
  shadow_float: "0 8px 24px rgba(0,0,0,0.12), 0 2px 6px rgba(0,0,0,0.08)"
typography:
  display: "Segoe UI Variable, SF Pro Display, Noto Sans SC, sans-serif"
  body: "Segoe UI, SF Pro Text, Noto Sans SC, sans-serif"
  mono: "Cascadia Code, SF Mono, Consolas, monospace"
  hero: "112px–148px / 600–700"
  title: "68px–84px / 600"
  subtitle: "40px–52px / 400–600"
  body: "32px–40px / 400"
  label: "24px–30px / 600"
radius:
  component: "6px"
  card: "12px"
  pill: "999px"
elevation:
  base: "0"
  card: "shadow_card"
  float: "shadow_float"
spacing:
  unit: "4px"
  card_padding: "40px–56px"
  section_gap: "48px–64px"
motion:
  enter: "0.25s cubic-bezier(0.45, 0, 0.15, 1)"
  micro: "0.15s ease"
  stagger: "0.04s"
  travel: "16px–24px"
---

# 微软流动信息风格

## 1. 核心概念

Fluent Design 的核心是「让信息系统有结构感、有层次感，但不沉重」。浅色背景、清晰分层、一致的卡片系统、恰当的留白、蓝色作为唯一主色。这个风格视觉上克制、可信，适合需要「让人信任」和「能快速扫读」的内容。

与磨砂玻璃的区别：Fluent Information 是浅色系、有墨色文字、用边框和轻微阴影建立层次，不依赖透明度和模糊。

## 2. 背景与层次

层次靠颜色和阴影而非模糊：

| 层级 | 颜色 | 阴影 | 边框 |
|---|---|---|---|
| 页面底 | `#F5F5F5` | 无 | 无 |
| 卡片 | `#FFFFFF` | shadow_card | 1px `rgba(0,0,0,0.08)` |
| 浮起/弹出 | `#FFFFFF` | shadow_float | 1px `rgba(0,0,0,0.12)` |
| 强调区 | `#EBF4FF`（蓝色软化） | 无 | 2px `#0078D4` 左侧线 |

## 3. 颜色语义

- `#0078D4`（Fluent 蓝）：主要行动点、激活状态、主链接、核心进度。
- `#D83B01`（橙红）：警告、限制条件、注意。
- `#107C10`（绿）：完成、通过、正向结果。
- `#038387`（蓝绿）：补充性分支、次要数据系列。
- **禁止**：同时使用超过 2 个语义色、随机彩色标签、彩色渐变标题。

## 4. 组件系统

### 信息卡
白色圆角卡，12px 圆角，2px `rgba(0,0,0,0.08)` 边框，`shadow_card`。卡内顶部可以有 `#0078D4` 左侧强调线（3px），表示主内容。标题 40px 600，正文 32px 400。

### 状态徽章
Pill 形，`border-radius: 999px`，4px 8px 内距。根据语义用对应颜色：激活=蓝软底+蓝字，注意=橙软底+橙字，完成=绿软底+绿字。字号 24–28px，600 weight。

### 步骤节点
圆形，48–64px 直径，蓝色填充，白色数字，step 之间用 `2px dashed #CBD5E0` 连线。已完成的节点改为绿色；当前节点可以有 4px 蓝色外环。

### 数据图表
坐标轴 `#E0E0E0`，数据系列用 `#0078D4` 为主色，第二系列用 `#038387`，不超过三个系列。标签直接放在数据附近，不用图例遮挡画面。

## 5. 构图规则

- 左对齐为主，标题和正文严格对齐；居中布局只用于少于三行的大标题场景。
- 信息按「主结论 → 解释层 → 细节层」纵向排列。
- 不在一张卡里塞三层不同层级的内容；信息过多时拆卡，而不是压缩字号。
- 标题右侧或左上角可以放语义标签（学科、状态），但标签不能比标题更抢眼。
- 封面：白色或极浅灰底，超大标题，蓝色单词或短语做视觉焦点，底部一行副标题。

## 6. 动效方向

- 卡片入场：`opacity 0→1 + translateY(12px→0)`，0.25s。
- 步骤节点依次出现，错峰 0.04s，按从上到下或从左到右阅读方向。
- 数据图：bar 从底部 `scaleY(0→1)`，折线逐段 `strokeDashoffset` 绘制。
- 场景切换：当前页右移退出（`translateX(0→-40px) + opacity 0`），新页从右侧进入（`translateX(40px→0) + opacity 0→1`），0.25s。

## 7. 禁止项

- 禁止深色背景（这是浅色系风格）。
- 禁止超过 2 种不同重量的阴影混用。
- 禁止彩色背景卡片（语义色只用于边框、徽章、图标，不铺满卡片背景）。
- 禁止超过 3 个不同圆角值。
- 禁止无语义的纯装饰图形和随机放置的图标。
- 禁止左右两列等宽的卡片网格（Fluent 的视觉节奏更喜欢不对称宽度）。

## 8. 执行检查

- [ ] 所有卡片圆角统一为 12px。
- [ ] 阴影值只来自 shadow_card 和 shadow_float 两档。
- [ ] 蓝色只出现在交互元素、数据和强调线，不出现在背景色块。
- [ ] 文字颜色满足 WCAG AA（正文 #1B1B1B 在白底上轻松通过）。
- [ ] 步骤节点和连线在同一坐标容器里，移动不会错位。
