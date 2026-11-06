---
name: "Academic Blueprint / 学术蓝图"
id: "academic-blueprint"
version: "2.0"
purpose: "中文教育信息、路径规划与课程决策视频"
preferred_format: "9:16"
resolution: "1080x1920"
best_for:
  - "AP 选课与升学规划"
  - "学习路径、步骤与分类"
  - "课程地图和知识结构"
avoid_for:
  - "情绪故事"
  - "生活方式与软性品牌"
colors:
  canvas: "#F3F6FA"
  paper: "#FFFFFF"
  ink: "#10233F"
  muted: "#58708D"
  primary: "#245FD3"
  primary_deep: "#153F91"
  primary_soft: "#E1EAFF"
  secondary: "#F07A42"
  secondary_soft: "#FFF0E7"
  grid: "#CBD8E9"
  edge: "#91A9C8"
typography:
  display: "Noto Sans SC, Microsoft YaHei, sans-serif"
  body: "Noto Sans SC, Microsoft YaHei, sans-serif"
  data: "Space Mono, Consolas, monospace"
  hero: "108px–136px / 800"
  scene_title: "76px–94px / 700"
  section_title: "50px–62px / 700"
  item_title: "36px–44px / 700"
  body_copy: "31px–36px / 400–600"
  label: "23px–27px / 700"
spacing:
  frame_padding: "56px–64px horizontal / 54px–68px vertical"
  content_gap: "14px–28px"
  section_gap: "30px–52px"
components:
  card_radius: "18px"
  pill_radius: "999px"
  border: "2px solid"
  structural_rule: "3px solid"
  depth: "flat; no blur shadow"
density:
  content_fill_target: "72%–86%"
  max_unintentional_blank_area: "18%"
  stable_reading_time: "2.4s minimum"
motion:
  energy: "measured"
  fast: "0.30s"
  standard: "0.50s"
  slow: "0.82s"
  stagger: "0.045s–0.065s"
  travel: "24px–46px"
  transition: "two-panel blueprint wipe"
---

# 学术蓝图

## 1. 核心概念

把复杂内容变成一张正在被绘制、定位和确认的学习地图。蓝色负责主路径与确定结论，橙色负责补充、提醒和下一步；网格、坐标、节点和编号共同建立阅读方向。

画面要像“专业信息图正在组装”，而不是网页卡片列表。所有结构线都有信息功能：连接、分组、标记进度或提示顺序。

## 2. 视觉语法

- 冷白纸面贯穿全部场景，不切换纯黑背景。
- 每幕使用 2–4 个结构元素：坐标网格、路线、节点、刻度、章节大号或边缘索引。
- 主要内容用不对称布局，优先左侧路线配右侧内容、顶部坐标配下方条目。
- 卡片与路线必须产生关系；不允许孤立的等宽卡片矩阵。
- 前景用少量等宽英文索引、页码和状态词增加完成度。

## 3. 色彩语义

- Primary：核心课程、主结论、已锁定状态、关键数字。
- Secondary：补充课程、限制条件、转折和行动提醒。
- Ink：标题和正文；Muted 仅用于解释性次级信息。
- 一幕只建立一个主色焦点和一个辅色提示，不临时引入第三种高饱和色。
- 浅色画布必须用 2–3px 实线和足够实的网格增强视频压缩后的清晰度。

## 4. 中文排版

- 主标题宽度占画面 64%–84%，最多三行，行高 1.06–1.14。
- 正文每行建议 13–18 个汉字；超过三行时拆成条目或拆场景。
- 标题用 700–800，正文用 400–600，重点词用 700。
- AP、STEM、编号和数据使用等宽字体，中文不使用等宽字体排长句。
- 不使用渐变文字、描边正文或极细字重。

## 5. 构图规则

- 首读：主标题、主数字或核心结论。
- 次读：路径节点、分组标题或对比关系。
- 收束：底部结论条、页码或下一步。
- 内容区域覆盖画面的 72%–86%；空白必须由网格、路线或大号章节数字组织。
- 页脚只放状态、页码和极短说明，不承载关键结论。

## 6. 核心组件

### 路线站点

- 左侧节点直径 64–82px，右侧内容容器与路线保持 28–42px 间距。
- 每个站点最多两层语义：核心与补充。
- 标题 36–44px，说明 31–35px；长内容换行但不压缩字号。

### 数字结论

- 80–132px 等宽数字配 38–48px 结论。
- 数字与解释形成一个组合，不能把说明孤立放在最底部。

### 锁定提示

- 使用浅橙底或 6px 橙色结构线。
- 只承载限制条件、决定动作或最后结论。

## 7. 动效方向

- 网格或主路径先建立，标题随后锁定，信息站点按阅读方向依次出现。
- 路线使用 scaleX 或 scaleY 绘制；节点用短距离位移加轻微缩放。
- 卡片进入方向要跟随路线，不统一从底部淡入。
- 背景只做单一、低幅度漂移或呼吸；不做持续旋转和弹跳。
- 场景转场使用蓝色与橙色实色板错峰覆盖，完成后立刻进入下一幕结构。

## 8. 推荐场景

- 首屏钩子：超大标题、被否定的误区、路径锁定正确方向。
- 分类地图：四到五个站点沿纵向轨道装配。
- 对比说明：蓝色核心列与橙色补充列形成主次。
- 三步总结：路径折叠为 1—2—3，最后一步用橙色提示。

## 9. 禁止项

- 禁止玻璃拟态、模糊阴影、霓虹、渐变文字和无语义装饰图标。
- 禁止所有卡片等大、等距、同方向进入。
- 禁止正文小于 31px 来补偿信息过多。
- 禁止让背景网格比内容更醒目。
- 禁止把原始表格直接缩小呈现。

## 10. 执行检查

- [ ] 蓝色与橙色语义始终一致。
- [ ] 每幕至少有标题与路径两个焦点。
- [ ] 正文至少 31px，标签至少 23px。
- [ ] 路线、节点和卡片存在明确连接关系。
- [ ] 至少保留 2.4 秒稳定阅读区间。
- [ ] 动画已注册为暂停且可寻址的时间线。
- [ ] 无随机值、无限循环和渲染时网络请求。
