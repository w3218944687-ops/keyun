---
name: "磨砂玻璃 / Frosted Glass Studio"
id: "frosted-glass-studio"
version: "1.0"
last_updated: "2026-10-05"
best_for:
  - "产品介绍、工具测评"
  - "数字工具与 App 推荐"
  - "清单型、对比型内容"
avoid_for:
  - "学术路径、课程规划"
  - "数据图表主导的内容"
colors:
  base_dark: "oklch(14% 0.01 250)"
  surface: "oklch(22% 0.015 250 / 0.72)"
  elevated: "oklch(30% 0.018 250 / 0.56)"
  stroke: "oklch(100% 0 0 / 0.12)"
  text_primary: "oklch(97% 0 0)"
  text_secondary: "oklch(75% 0.01 250)"
  accent: "oklch(72% 0.18 230)"
  accent_warm: "oklch(76% 0.17 55)"
  gradient_cover: "linear-gradient(160deg, oklch(18% 0.025 260), oklch(12% 0.015 290))"
typography:
  hero: "120px–160px / 800, line-height 0.98"
  scene_title: "72px–88px / 700"
  label: "26px–32px / 600, letter-spacing 0.06em"
  body: "32px–38px / 400–500"
  mono: "Space Mono, Consolas, monospace"
blur:
  card: "backdrop-filter: blur(24px) saturate(1.4)"
  elevated: "backdrop-filter: blur(40px) saturate(1.6)"
borders:
  card: "1px solid oklch(100% 0 0 / 0.10)"
  elevated: "1px solid oklch(100% 0 0 / 0.18)"
  inner_top: "1px solid oklch(100% 0 0 / 0.28)"
depth:
  card_shadow: "0 8px 32px oklch(0% 0 0 / 0.45)"
  elevated_shadow: "0 20px 60px oklch(0% 0 0 / 0.55)"
motion:
  enter: "0.40s cubic-bezier(0.22, 1, 0.36, 1)"
  micro: "0.18s ease"
  blur_reveal: "backdrop-filter from 0 to target over 0.5s"
  stagger: "0.06s"
---

# 磨砂玻璃风格

## 1. 核心概念

深色渐变背景，透明度层叠。卡片本身是「悬浮在背景之上的毛玻璃」，而不是白色方块。背景可以是深蓝、深紫，或带轻微纹理的纯黑。卡片和背景之间的关系让人感觉「背景透进来了一点点」。

这个风格的重点是：用「深色 + 透明层」替代「白底 + 阴影」，用「模糊 + 边框高光」替代「卡片投影」。

## 2. 背景系统

- 底层：一个饱和度极低的深色纯色面，约 `oklch(12–18% 0.015–0.025 240–270)`。
- 中层：可以叠一个低不透明度的径向渐变光团（蓝色或紫色），暗示光源，不是纯装饰。
- 顶层：所有内容卡片放在这一层，用 `backdrop-filter: blur()` 从底层取模糊。
- 背景不做图片、不做纹理噪点、不做彩色渐变墙。
- 背景最多两个「光点」，否则背景会比内容更抢眼。

## 3. 卡片系统

卡片的视觉层次靠**透明度**而不是颜色区分：

| 层级 | 表面颜色 | 模糊量 | 边框 |
|---|---|---|---|
| 基础卡 | 22% 明度 / 72% 透明 | blur(24px) | 10% 白色描边 |
| 浮起卡 | 30% 明度 / 56% 透明 | blur(40px) | 18% 白色描边 |
| 顶层提示 | 36% 明度 / 50% 透明 | blur(52px) | 28% 白色描边 + 顶部内发光 |

顶部内高光（`box-shadow: inset 0 1px 0 oklch(100% 0 0 / 0.30)`）是玻璃质感最重要的细节。

## 4. 颜色语义

- **蓝色 accent（#245FD3 同亮度 OKLCH 等价）**：主结论、核心标签、主交互。
- **暖橙 accent**：注意事项、价格、限制条件、下一步行动。
- **白色文字**：主标题和正文，两个亮度级别（97% 和 75%）。
- **禁止**：彩虹渐变文字、霓虹发光、多余的多色配色。

## 5. 构图规则

- 竖屏 1080×1920，和 Academic Blueprint 相同的安全区（左右 64px，顶 120px，底 250px）。
- 主内容区应覆盖 72–86%。深色版面的「空白」会比浅色版面显得更重，需要背景光团或轻微纹理填补。
- 封面：大字居中 + 背景光点，不需要底部介绍。
- 卡片之间不要用阴影分隔，用 4–8px 间距，靠视觉深度区分。

## 6. 动效方向

- 卡片入场：`opacity 0→1 + translateY(28px→0)` + 同时 `backdrop-filter blur(0→24px)`，约 0.4s。
- 背景光团：非常低幅度的缓慢漂移（0.03×宽度，8–12 秒周期），或完全静止。
- 不做大幅度背景动画，不做粒子效果，不做常驻渐变循环。
- 每次场景切换：当前页 `opacity 0 + scale(0.97)` 离场，新页 `opacity 0 + scale(1.03→1)` 入场，0.3s。

## 7. 禁止项

- 禁止纯黑 `#000` 或纯白 `#fff` 作为主色，会丢失玻璃层次。
- 禁止 `blur()` 过大（>60px）导致背景完全消失。
- 禁止每张卡片都用不同颜色，破坏统一深色基调。
- 禁止超过 2 层叠加的 `backdrop-filter`，会导致渲染卡顿。
- 禁止白底卡片、实心彩色卡片作为主信息容器。

## 8. 执行检查

- [ ] 背景深色底是否一致，没有白色意外出现。
- [ ] `backdrop-filter` 有真实内容在下方可模糊，否则会是纯色块。
- [ ] 卡片顶部内高光存在。
- [ ] 文字对比度满足 WCAG AA（深色背景上白字 4.5:1+）。
- [ ] 帧渲染时 `backdrop-filter` 需要允许硬件加速，Playwright 截图已确认正常渲染。
