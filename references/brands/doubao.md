# 豆包（Doubao）设计规范

> **品牌主色**: `#FF6B2B`（活力橙）| **平台**: Web | **关键词**: 活力橙/字节系AI/创意工具

---

## 一、设计价值观与原则

1. **活力创意**：橙色传递年轻活力，激发用户创造力与探索欲
2. **字节基因**：继承字节跳动设计语言，内容优先、算法驱动
3. **轻松上手**：零门槛AI体验，对话即用、无需学习
4. **趣味交互**：表情、语音、图片多模态趣味交互，AI也有温度

---

## 二、配色体系

### 品牌主色色板（活力橙 #FF6B2B）

| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | `#FFF4ED` | 浅底背景、标记高亮 |
| 100 | `#FFE6D5` | 标签底色 |
| 200 | `#FECCAA` | 图标浅色态 |
| 300 | `#FDA97A` | 辅助强调 |
| 400 | `#FC8C4F` | 悬停态 |
| 500 | `#FF6B2B` | **品牌主色**，主按钮、链接 |
| 600 | `#E55A1B` | 按压态 |
| 700 | `#BF4510` | 深色强调 |
| 800 | `#8A320C` | 暗色模式主色 |
| 900 | `#551E07` | 极深背景 |

### 功能色

| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | `#22C55E` | 发送成功、操作完成 |
| 警告 | `#F59E0B` | 提醒注意 |
| 错误 | `#EF4444` | 发送失败 |
| 信息 | `#3B82F6` | 引导提示 |

### 中性色

| 名称 | 色值 | 用途 |
|------|------|------|
| 标题 | `#1A1A1A` | 一级标题 |
| 正文 | `#333333` | 正文内容 |
| 次级 | `#666666` | 辅助说明 |
| 占位 | `#999999` | 占位文字 |
| 分割 | `#EEEEEE` | 分割线 |
| 浅底 | `#F7F7F7` | 页面底色 |
| 卡片 | `#FFFFFF` | 卡片底色 |

### 渐变色

| 名称 | 值 | 用途 |
|------|-----|------|
| 品牌渐变 | `linear-gradient(135deg, #FF6B2B, #FC8C4F)` | Hero区域、主按钮 |
| 活力渐变 | `linear-gradient(90deg, #FF6B2B, #FF2D87)` | 创意功能装饰 |
| 暖阳渐变 | `linear-gradient(180deg, #FFF4ED, #FFFFFF)` | 内容区背景 |

---

## 三、字体排版体系

### 字体家族

- **主字体**: `'PingFang SC', 'Noto Sans SC', 'Helvetica Neue', sans-serif`
- **代码字体**: `'JetBrains Mono', 'Fira Code', Consolas, monospace`

### 字号阶梯

| 层级 | 字号 | 行高 | 字重 | 用途 |
|------|------|------|------|------|
| H1 | 22px | 30px | 600 | 页面标题 |
| H2 | 18px | 26px | 600 | 模块标题 |
| H3 | 16px | 24px | 500 | 卡片标题 |
| Body | 14px | 22px | 400 | 正文内容 |
| Code | 13px | 20px | 400 | 代码块 |
| Caption | 12px | 18px | 400 | 辅助说明 |
| Micro | 11px | 16px | 400 | 标签 |

### 字重体系

| 字重 | 值 | 用途 |
|------|-----|------|
| Regular | 400 | 正文、代码 |
| Medium | 500 | 小标题、按钮 |
| Semibold | 600 | 标题、强调 |

---

## 四、组件设计规范

### 按钮

| 类型 | 高度 | 圆角 | 背景 | 文字色 | 内边距 |
|------|------|------|------|--------|--------|
| 主要按钮 | 40px | 20px | `#FF6B2B` | `#FFFFFF` | 0 20px |
| 次要按钮 | 40px | 20px | `#FFF4ED` | `#FF6B2B` | 0 20px |
| 文字按钮 | 32px | 4px | transparent | `#FF6B2B` | 0 8px |
| 表情按钮 | 36px | 18px | `#F7F7F7` | `#666666` | 0 12px |

### 卡片

| 类型 | 圆角 | 阴影 | 内边距 | 背景 |
|------|------|------|--------|------|
| 对话卡片 | 16px | none | 16px | `#F7F7F7` |
| 功能卡片 | 12px | `0 2px 8px rgba(0,0,0,0.06)` | 16px | `#FFFFFF` |
| 角色卡片 | 16px | `0 4px 12px rgba(0,0,0,0.08)` | 20px | `#FFFFFF` |

### 导航栏

- 高度：52px；背景：`#FFFFFF`；底部边框：1px solid `#EEEEEE`
- 左侧Logo，中间角色切换，右侧设置+用户

### 弹窗

- 圆角：16px；遮罩：`rgba(0,0,0,0.4)`；背景：`#FFFFFF`
- 标题区：内边距20px 24px，字号16px，字重500

### 输入框

- 高度：44px；圆角：22px；背景：`#F7F7F7`；边框：none
- 聚焦背景：`#FFFFFF`；聚焦边框：1px solid `#FF6B2B`
- 支持表情选择器、语音输入、图片上传

### AI对话组件

| 组件 | 规格 |
|------|------|
| 用户气泡 | 背景`#FF6B2B`，文字`#FFFFFF`，圆角18px 18px 4px 18px，内边距12px 16px |
| AI气泡 | 背景`#F7F7F7`，文字`#333333`，圆角18px 18px 18px 4px，内边距12px 16px |
| 角色标签 | 背景`#FFF4ED`，文字`#FF6B2B`，圆角12px，内边距4px 10px，字号12px |
| 代码块 | 背景`#1E1E1E`，文字`#D4D4D4`，圆角12px，字号13px，行高20px，内边距16px |
| Markdown标题 | H1 18px/600，H2 16px/500，H3 14px/500 |
| Markdown代码 | 背景`#FFF4ED`，文字`#E55A1B`，圆角4px，内边距2px 6px，字号13px |

---

## 五、间距与圆角体系

### 间距阶梯（4px基准）

| Token | 值 | 用途 |
|-------|-----|------|
| xs | 4px | 图标与文字间距 |
| sm | 8px | 紧凑元素间距 |
| md | 12px | 组件内部间距 |
| lg | 16px | 卡片内边距 |
| xl | 24px | 模块间距 |
| 2xl | 32px | 区块间距 |
| 3xl | 48px | 大区块间距 |

### 圆角阶梯

| Token | 值 | 用途 |
|-------|-----|------|
| none | 0px | 表格 |
| sm | 4px | 标签 |
| md | 8px | 按钮 |
| lg | 12px | 卡片、代码块 |
| xl | 16px | 对话气泡、弹窗 |
| pill | 20px | 主按钮、输入框 |
| full | 9999px | 头像 |

---

## 六、动效规范

| 场景 | 时长 | 缓动 | 说明 |
|------|------|------|------|
| 按钮悬停 | 150ms | ease | 背景色过渡 |
| 弹窗出现 | 250ms | ease-out | 从底部弹起 |
| AI流式输出 | 25ms/字 | linear | 逐字输出 |
| 角色切换 | 300ms | ease-in-out | 淡入淡出+缩放 |
| 表情弹出 | 200ms | ease-out | 从底部滑入 |
| 发送动画 | 300ms | ease | 气泡飞出效果 |

---

## 七、暗色模式规范

| 元素 | 亮色值 | 暗色值 |
|------|--------|--------|
| 页面背景 | `#F7F7F7` | `#0F0F0F` |
| 卡片背景 | `#FFFFFF` | `#1A1A1A` |
| 主色 | `#FF6B2B` | `#FC8C4F` |
| 标题文字 | `#1A1A1A` | `#F0F0F0` |
| 正文文字 | `#333333` | `#CCCCCC` |
| 次级文字 | `#666666` | `#888888` |
| 分割线 | `#EEEEEE` | `#2A2A2A` |
| AI气泡 | `#F7F7F7` | `#1A1A1A` |
| 用户气泡 | `#FF6B2B` | `#FC8C4F` |
| 代码块 | `#1E1E1E` | `#0A0A0A` |

---

## 八、设计禁忌（Do's and Don'ts）

### Do

- 使用圆角药丸形按钮和输入框，传递友好感
- AI角色使用头像+名称标签，增强人格化
- 输入框支持表情、语音、图片多模态入口
- 橙色`#FF6B2B`作为唯一品牌强调色

### Don't

- 禁止使用方形按钮（与活力调性不符）
- 禁止AI角色无头像和名称（缺乏人格化）
- 禁止输入框缺少多模态入口
- 禁止橙色与红色同时大面积使用（色彩冲突）

---

## 九、CSS变量快速参考

```css
:root {
  --doubao-primary: #FF6B2B;
  --doubao-primary-50: #FFF4ED;
  --doubao-primary-100: #FFE6D5;
  --doubao-primary-200: #FECCAA;
  --doubao-primary-300: #FDA97A;
  --doubao-primary-400: #FC8C4F;
  --doubao-primary-500: #FF6B2B;
  --doubao-primary-600: #E55A1B;
  --doubao-primary-700: #BF4510;
  --doubao-primary-800: #8A320C;
  --doubao-primary-900: #551E07;
  --doubao-success: #22C55E;
  --doubao-warning: #F59E0B;
  --doubao-error: #EF4444;
  --doubao-info: #3B82F6;
  --doubao-text-title: #1A1A1A;
  --doubao-text-body: #333333;
  --doubao-text-secondary: #666666;
  --doubao-text-placeholder: #999999;
  --doubao-border: #EEEEEE;
  --doubao-bg-page: #F7F7F7;
  --doubao-bg-card: #FFFFFF;
  --doubao-spacing-xs: 4px;
  --doubao-spacing-sm: 8px;
  --doubao-spacing-md: 12px;
  --doubao-spacing-lg: 16px;
  --doubao-spacing-xl: 24px;
  --doubao-spacing-2xl: 32px;
  --doubao-spacing-3xl: 48px;
  --doubao-radius-sm: 4px;
  --doubao-radius-md: 8px;
  --doubao-radius-lg: 12px;
  --doubao-radius-xl: 16px;
  --doubao-radius-pill: 20px;
  --doubao-radius-full: 9999px;
  --doubao-font-family: 'PingFang SC', 'Noto Sans SC', 'Helvetica Neue', sans-serif;
  --doubao-font-mono: 'JetBrains Mono', 'Fira Code', Consolas, monospace;
}
```
