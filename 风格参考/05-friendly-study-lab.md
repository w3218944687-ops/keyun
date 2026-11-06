---
name: "Friendly Study Lab / 友好学习实验室"
id: "friendly-study-lab"
version: "1.0"
purpose: "面向学生和家长的温暖、清晰、易接近的中文学习视频"
preferred_format: "9:16"
resolution: "1080x1920"
best_for:
  - "学习方法与入门科普"
  - "学生和家长沟通"
  - "步骤、习惯与轻量课程建议"
avoid_for:
  - "金融和危机内容"
  - "严肃新闻与强科技主题"
colors:
  canvas: "#FFF6E9"
  paper: "#FFFFFF"
  ink: "#302C35"
  muted: "#706875"
  primary: "#279F90"
  primary_soft: "#DDF3EE"
  secondary: "#EE6A69"
  secondary_soft: "#FFE2DE"
  accent: "#F2C14E"
  accent_soft: "#FFF0B8"
  sky: "#82BDEB"
  outline: "#3D3742"
typography:
  display: "Noto Sans SC, Microsoft YaHei, sans-serif"
  body: "Noto Sans SC, Microsoft YaHei, sans-serif"
  data: "Nunito Sans, Arial, sans-serif"
  hero: "104px–136px / 800"
  scene_title: "74px–92px / 800"
  section_title: "48px–62px / 700"
  item_title: "36px–44px / 700"
  body_copy: "31px–37px / 400–600"
  label: "24px–28px / 700"
spacing:
  frame_padding: "54px–66px horizontal / 54px–70px vertical"
  card_gap: "16px–26px"
  section_gap: "28px–48px"
components:
  card_radius: "24px–36px"
  pill_radius: "999px"
  border: "3px solid"
  hard_shadow: "5px 6px 0 rgba(61,55,66,0.16)"
  depth: "soft color layers; no blur shadow"
density:
  content_fill_target: "68%–84%"
  max_unintentional_blank_area: "18%"
  stable_reading_time: "2.5s minimum"
motion:
  energy: "friendly"
  fast: "0.32s"
  standard: "0.54s"
  slow: "0.86s"
  stagger: "0.055s–0.085s"
  travel: "20px–38px"
  transition: "notebook tab slide"
---

# 友好学习实验室

## 1. 核心概念

把学习内容呈现成一本正在整理的个人学习手册。圆角纸片、柔和实色、手绘式连接线和清楚的步骤标签降低距离感，让学生愿意看、家长也能快速理解。

亲和不等于幼稚。装饰采用简化文具和实验符号，避免卡通人物、表情包和过多糖果色。

## 2. 视觉语法

- 暖白画布贯穿全片，内容区域使用白色或浅色纸片。
- 每幕选择 2–3 个手册元素：页签、便签、勾选框、连接线、圆点、简化图标。
- 组件可有不同大小和轻微错位，但标题与正文保持稳固基线。
- 线条具有轻微手绘感，粗细保持 3–5px，不能过度抖动。
- 一幕最多出现三种彩色，其中只有一种承担主焦点。

## 3. 色彩语义

- Primary 青绿：正确方法、已完成、可执行步骤。
- Secondary 珊瑚红：容易忽略、需要调整、重要提醒。
- Accent 黄色：鼓励、短提示和轻量高亮。
- Sky 天蓝：分类辅助或例子，不承担关键结论。
- 文字始终用 Ink，不用彩色正文大段排版。

## 4. 中文排版

- 标题使用圆润但不过度卡通的黑体，字重 700–800。
- 主标题 104–136px，最多三行；关键词可以放进彩色胶囊，但每行最多一个。
- 正文 31–37px，行高 1.4–1.55，语气直接、句子短。
- 标签 24–28px，用 2–5 个字表达状态。
- 编号可以是圆形贴纸，数字与中文标题保持明显尺寸差。

## 5. 构图规则

- 首读是问题或方法名，次读是步骤卡，最后读提醒或鼓励。
- 优先使用上标题加下方路径、左右错位便签、主卡配小提醒。
- 卡片不做完全等宽等高；主步骤更大，补充提示更小。
- 空白区域用页签、连接线或大号浅色图形组织，不堆装饰小图标。
- 关键内容留在 60px 安全区内，底部平台 UI 可能遮挡的区域只放页码或非关键装饰。

## 6. 核心组件

### 学习步骤卡

- 编号贴纸、短标题和一句解释组成一张卡。
- 青绿表示建议动作，珊瑚红表示需要避免或修正的动作。

### 勾选清单

- 每幕最多四项，每项控制在一至两行。
- 勾选动画只播放一次，完成后保留稳定状态。

### 小提醒便签

- 黄色或浅珊瑚底，使用 3px 描边和短标题。
- 只承载一句提醒，不承担正文段落。

### 例子卡

- 例子与规则使用不同底色和明显的 例子 标签。
- 图标只用于帮助识别，不取代文字含义。

## 7. 动效方向

- 页签先滑入，标题随后落位，步骤卡沿连接线依次出现。
- 卡片可以有轻微 0.98 到 1 的缩放，但不做夸张弹跳。
- 勾选、下划线和连接线使用一次性绘制动画。
- 背景装饰只做共享的低幅呼吸或漂移，不给每个图标单独循环。
- 转场使用页面页签或纸片横向滑动，保持温和但不拖沓。

## 8. 推荐场景

- 首屏：一个学习问题加一句减压式解释。
- 三步方法：三张错位步骤卡沿路径展开。
- 常见误区：珊瑚提醒卡配青绿修正卡。
- 结尾：勾选清单收束成一句可执行行动。

## 9. 禁止项

- 禁止过多卡通贴纸、emoji 和无关插画。
- 禁止粉彩低对比文字。
- 禁止所有卡片等大并平均排列。
- 禁止柔焦、玻璃拟态和大片模糊阴影。
- 禁止把亲和风格做成低幼儿童界面。

## 10. 执行检查

- [ ] 主焦点颜色每幕只有一种。
- [ ] 装饰不超过三类，且服务阅读路径。
- [ ] 正文至少 31px，标签至少 24px。
- [ ] 主步骤和补充提示有明显尺寸差。
- [ ] 没有低对比粉彩文字和幼稚装饰。
- [ ] 动效可寻址，稳定阅读至少 2.5 秒。
