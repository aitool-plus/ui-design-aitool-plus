# MiniMax 设计规范

> **品牌主色**: `#6B21A8`（创意紫红）| **平台**: Web | **关键词**: 创意紫红/多模态/角色AI

---

## 一、设计价值观与原则

1. **创意无限**：紫红色传递创意与想象，激发用户创造角色与内容
2. **角色扮演**：AI角色人格化，每个角色有独特视觉标识与交互风格
3. **多模态融合**：文本、语音、图像、视频多模态无缝切换
4. **沉浸体验**：角色对话沉浸式体验，界面服务于故事与情感

---

## 二、配色体系

### 品牌主色色板（创意紫红 #6B21A8）

| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | `#F5F0FF` | 浅底背景 |
| 100 | `#EDE5FF` | 标签底色 |
| 200 | `#D9C7FF` | 图标浅色态 |
| 300 | `#C4A8FF` | 辅助强调 |
| 400 | `#A855F7` | 悬停态 |
| 500 | `#6B21A8` | **品牌主色**，主按钮、链接 |
| 600 | `#581C87` | 按压态 |
| 700 | `#45166B` | 深色强调 |
| 800 | `#331050` | 暗色模式主色 |
| 900 | `#1E0A33` | 极深背景 |

### 功能色

| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | `#10B981` | 生成完成 |
| 警告 | `#F59E0B` | 内容审核提示 |
| 错误 | `#EF4444` | 生成失败 |
| 信息 | `#6B21A8` | 与品牌色统一 |
| 角色标识 | `#EC4899` | 角色卡片装饰 |

### 中性色

| 名称 | 色值 | 用途 |
|------|------|------|
| 标题 | `#1A1A2E` | 一级标题 |
| 正文 | `#374151` | 正文内容 |
| 次级 | `#6B7280` | 辅助说明 |
| 占位 | `#9CA3AF` | 占位文字 |
| 分割 | `#E5E7EB` | 分割线 |
| 浅底 | `#FAFAFE` | 页面底色 |
| 卡片 | `#FFFFFF` | 卡片底色 |

### 渐变色

| 名称 | 值 | 用途 |
|------|-----|------|
| 品牌渐变 | `linear-gradient(135deg, #6B21A8, #A855F7)` | Hero区域 |
| 创意渐变 | `linear-gradient(90deg, #6B21A8, #EC4899)` | 角色卡片装饰 |
| 梦幻渐变 | `linear-gradient(135deg, #6B21A8, #3B82F6, #10B981)` | 多模态展示 |

---

## 三、字体排版体系

### 字体家族

- **主字体**: `'Noto Sans SC', 'PingFang SC', -apple-system, sans-serif`
- **代码字体**: `'JetBrains Mono', 'Fira Code', Consolas, monospace`

### 字号阶梯

| 层级 | 字号 | 行高 | 字重 | 用途 |
|------|------|------|------|------|
| H1 | 24px | 32px | 600 | 页面标题 |
| H2 | 20px | 28px | 600 | 模块标题 |
| H3 | 16px | 24px | 500 | 卡片标题 |
| Body | 14px | 22px | 400 | 正文内容 |
| Code | 13px | 20px | 400 | 代码块 |
| Caption | 12px | 18px | 400 | 辅助说明 |

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
| 主要按钮 | 36px | 8px | `#6B21A8` | `#FFFFFF` | 0 16px |
| 次要按钮 | 36px | 8px | `#F5F0FF` | `#6B21A8` | 0 16px |
| 角色按钮 | 40px | 20px | `linear-gradient(135deg, #6B21A8, #EC4899)` | `#FFFFFF` | 0 20px |
| 文字按钮 | 32px | 4px | transparent | `#6B21A8` | 0 8px |

### 卡片

| 类型 | 圆角 | 阴影 | 内边距 | 背景 |
|------|------|------|--------|------|
| 对话卡片 | 16px | none | 16px | `#FAFAFE` |
| 角色卡片 | 16px | `0 4px 16px rgba(107,33,168,0.1)` | 20px | `#FFFFFF` |
| 创意卡片 | 12px | `0 2px 8px rgba(0,0,0,0.06)` | 16px | `#FFFFFF` |

### 导航栏

- 高度：56px；背景：`#FFFFFF`；底部边框：1px solid `#E5E7EB`
- 左侧Logo，中间角色/对话切换，右侧创建+用户

### 弹窗

- 圆角：16px；遮罩：`rgba(0,0,0,0.5)`；背景：`#FFFFFF`

### 输入框

- 高度：44px；圆角：22px；背景：`#FAFAFE`；边框：1px solid `#E5E7EB`
- 聚焦边框：1px solid `#6B21A8`；聚焦阴影：`0 0 0 3px rgba(107,33,168,0.12)`

### AI对话组件

| 组件 | 规格 |
|------|------|
| 用户气泡 | 背景`#6B21A8`，文字`#FFFFFF`，圆径18px 18px 4px 18px，内边距12px 16px |
| AI气泡 | 背景`#FAFAFE`，文字`#374151`，圆角18px 18px 18px 4px，内边距12px 16px |
| 角色名称 | 背景`#F5F0FF`，文字`#6B21A8`，圆角12px，内边距4px 10px，字号12px |
| 代码块 | 背景`#1E1E2E`，文字`#E2E8F0`，圆角8px，字号13px，行高20px，内边距16px |
| Markdown标题 | H1 18px/600，H2 16px/500，H3 14px/500 |
| Markdown代码 | 背景`#F5F0FF`，文字`#581C87`，圆角4px，内边距2px 6px，字号13px |

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
| sm | 4px | 标签 |
| md | 8px | 按钮、代码块 |
| lg | 12px | 卡片 |
| xl | 16px | 对话气泡、弹窗 |
| pill | 20px | 角色按钮 |
| full | 9999px | 头像 |

---

## 六、动效规范

| 场景 | 时长 | 缓动 | 说明 |
|------|------|------|------|
| 按钮悬停 | 150ms | ease | 背景色过渡 |
| 弹窗出现 | 250ms | ease-out | 从底部弹起 |
| AI流式输出 | 25ms/字 | linear | 逐字输出 |
| 角色切换 | 400ms | ease-in-out | 淡入淡出+缩放 |
| 角色卡片悬停 | 200ms | ease | 微上浮+阴影增强 |

---

## 七、暗色模式规范

| 元素 | 亮色值 | 暗色值 |
|------|--------|--------|
| 页面背景 | `#FAFAFE` | `#0F0A1A` |
| 卡片背景 | `#FFFFFF` | `#1A1A2E` |
| 主色 | `#6B21A8` | `#A855F7` |
| 标题文字 | `#1A1A2E` | `#F1F5F9` |
| 正文文字 | `#374151` | `#CBD5E1` |
| 次级文字 | `#6B7280` | `#94A3B8` |
| 分割线 | `#E5E7EB` | `#2D2D44` |
| AI气泡 | `#FAFAFE` | `#1A1A2E` |
| 用户气泡 | `#6B21A8` | `#A855F7` |
| 代码块 | `#1E1E2E` | `#0F0A1A` |

---

## 八、设计禁忌（Do's and Don'ts）

### Do

- 角色卡片使用渐变装饰突出个性
- 角色名称标签始终可见，区分角色身份
- 对话气泡使用较大圆角，传递柔和感
- 暗色模式使用深紫底色而非纯黑

### Don't

- 禁止角色卡片无视觉个性区分
- 禁止AI回复缺少角色名称标签
- 禁止暗色模式使用纯黑底色
- 禁止紫红与粉色同时作为主强调色

---

## 九、CSS变量快速参考

```css
:root {
  --minimax-primary: #6B21A8;
  --minimax-primary-50: #F5F0FF;
  --minimax-primary-100: #EDE5FF;
  --minimax-primary-200: #D9C7FF;
  --minimax-primary-300: #C4A8FF;
  --minimax-primary-400: #A855F7;
  --minimax-primary-500: #6B21A8;
  --minimax-primary-600: #581C87;
  --minimax-primary-700: #45166B;
  --minimax-primary-800: #331050;
  --minimax-primary-900: #1E0A33;
  --minimax-success: #10B981;
  --minimax-warning: #F59E0B;
  --minimax-error: #EF4444;
  --minimax-character: #EC4899;
  --minimax-text-title: #1A1A2E;
  --minimax-text-body: #374151;
  --minimax-text-secondary: #6B7280;
  --minimax-text-placeholder: #9CA3AF;
  --minimax-border: #E5E7EB;
  --minimax-bg-page: #FAFAFE;
  --minimax-bg-card: #FFFFFF;
  --minimax-spacing-xs: 4px;
  --minimax-spacing-sm: 8px;
  --minimax-spacing-md: 12px;
  --minimax-spacing-lg: 16px;
  --minimax-spacing-xl: 24px;
  --minimax-spacing-2xl: 32px;
  --minimax-spacing-3xl: 48px;
  --minimax-radius-sm: 4px;
  --minimax-radius-md: 8px;
  --minimax-radius-lg: 12px;
  --minimax-radius-xl: 16px;
  --minimax-radius-pill: 20px;
  --minimax-radius-full: 9999px;
  --minimax-font-family: 'Noto Sans SC', 'PingFang SC', -apple-system, sans-serif;
  --minimax-font-mono: 'JetBrains Mono', 'Fira Code', Consolas, monospace;
}
```
