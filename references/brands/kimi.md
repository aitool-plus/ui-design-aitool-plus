# Kimi / Moonshot AI 设计规范

> **品牌主色**: `#4F6BED`（长文蓝）| **平台**: Web | **关键词**: 长文蓝/智能阅读/上下文理解

---

## 一、设计价值观与原则

1. **长文友好**：超长上下文能力映射为沉浸阅读体验，排版舒适、层次清晰
2. **智能辅助**：AI作为阅读伙伴而非工具，界面温和引导而非强势干预
3. **信息密度**：在有限空间内高效呈现长文本，可折叠、可跳转、可摘要
4. **阅读沉浸**：减少视觉噪音，让用户专注于内容本身

---

## 二、配色体系

### 品牌主色色板（长文蓝 #4F6BED）

| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | `#EEF1FF` | 浅底高亮、选中态 |
| 100 | `#D5DCFF` | 标签背景 |
| 200 | `#ABB9FF` | 图标浅色态 |
| 300 | `#8196FF` | 辅助强调 |
| 400 | `#6780FF` | 悬停态 |
| 500 | `#4F6BED` | **品牌主色**，主按钮、链接 |
| 600 | `#3D56D4` | 按压态 |
| 700 | `#2E42A8` | 深色强调 |
| 800 | `#1F2D75` | 暗色模式主色 |
| 900 | `#121945` | 极深背景 |

### 功能色

| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | `#22C55E` | 文件解析成功、发送成功 |
| 警告 | `#EAB308` | 文件过大提示 |
| 错误 | `#EF4444` | 解析失败、网络错误 |
| 信息 | `#4F6BED` | 与品牌色统一 |

### 中性色

| 名称 | 色值 | 用途 |
|------|------|------|
| 标题 | `#1E293B` | 一级标题 |
| 正文 | `#334155` | 正文内容 |
| 次级 | `#64748B` | 辅助说明 |
| 占位 | `#94A3B8` | 占位文字 |
| 分割 | `#E2E8F0` | 分割线 |
| 浅底 | `#F8FAFC` | 页面底色 |
| 卡片 | `#FFFFFF` | 卡片底色 |
| 深面 | `#1E293B` | 暗色卡片 |

### 渐变色

| 名称 | 值 | 用途 |
|------|-----|------|
| 品牌渐变 | `linear-gradient(135deg, #4F6BED, #8196FF)` | Hero区域 |
| 阅读渐变 | `linear-gradient(180deg, #F8FAFC, #EEF1FF)` | 阅读区背景 |
| 文件渐变 | `linear-gradient(135deg, #4F6BED, #22C55E)` | 文件上传成功 |

---

## 三、字体排版体系

### 字体家族

- **主字体**: `'Noto Sans SC', 'PingFang SC', -apple-system, sans-serif`
- **阅读字体**: `'Noto Serif SC', 'Source Han Serif SC', Georgia, serif`
- **代码字体**: `'JetBrains Mono', 'Fira Code', Consolas, monospace`

### 字号阶梯

| 层级 | 字号 | 行高 | 字重 | 用途 |
|------|------|------|------|------|
| H1 | 24px | 36px | 600 | 页面标题 |
| H2 | 20px | 30px | 600 | 模块标题 |
| H3 | 16px | 24px | 500 | 卡片标题 |
| Body | 15px | 26px | 400 | 正文（阅读优化行高） |
| Code | 13px | 20px | 400 | 代码块 |
| Caption | 12px | 18px | 400 | 辅助说明 |
| Micro | 11px | 16px | 400 | 页码、字数统计 |

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
| 主要按钮 | 36px | 8px | `#4F6BED` | `#FFFFFF` | 0 16px |
| 次要按钮 | 36px | 8px | `#EEF1FF` | `#4F6BED` | 0 16px |
| 文字按钮 | 32px | 4px | transparent | `#4F6BED` | 0 8px |
| 发送按钮 | 36px | 8px | `#4F6BED` | `#FFFFFF` | 0 12px |

### 卡片

| 类型 | 圆角 | 阴影 | 内边距 | 背景 |
|------|------|------|--------|------|
| 对话卡片 | 16px | none | 16px | `#F8FAFC` |
| 文件卡片 | 12px | `0 1px 3px rgba(0,0,0,0.06)` | 16px | `#FFFFFF` |
| 摘要卡片 | 8px | none | 12px 16px | `#EEF1FF`，左侧3px #4F6BED |

### 导航栏

- 高度：56px；背景：`#FFFFFF`；底部边框：1px solid `#E2E8F0`
- 左侧Logo，中间对话标题，右侧文件入口+设置

### 弹窗

- 圆角：12px；遮罩：`rgba(0,0,0,0.4)`；背景：`#FFFFFF`
- 标题区：内边距20px 24px，字号16px，字重500
- 内容区：内边距16px 24px，字号14px

### 输入框

- 高度：44px；圆角：12px；背景：`#F8FAFC`；边框：1px solid `#E2E8F0`
- 聚焦边框：1px solid `#4F6BED`；聚焦阴影：`0 0 0 3px rgba(79,107,237,0.12)`
- 支持多行输入，最大高度200px自动滚动

### AI对话组件

| 组件 | 规格 |
|------|------|
| 用户气泡 | 背景`#4F6BED`，文字`#FFFFFF`，圆角16px 16px 4px 16px，内边距12px 16px |
| AI气泡 | 背景`#F8FAFC`，文字`#334155`，圆角16px 16px 16px 4px，内边距12px 16px |
| 引用块 | 背景`#EEF1FF`，左侧3px `#4F6BED`，圆角0 8px 8px 0，内边距12px 16px |
| 代码块 | 背景`#1E293B`，文字`#E2E8F0`，圆角8px，字号13px，行高20px，内边距16px |
| 文件预览 | 背景`#FFFFFF`，边框1px `#E2E8F0`，圆角8px，最大高度400px可滚动 |
| Markdown标题 | H1 18px/600，H2 16px/500，H3 14px/500 |
| Markdown代码 | 背景`#F1F5F9`，文字`#4F6BED`，圆角4px，内边距2px 6px，字号13px |
| Markdown链接 | 色`#4F6BED`，悬停下划线 |

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
| md | 8px | 按钮、输入框 |
| lg | 12px | 卡片、弹窗 |
| xl | 16px | 对话气泡 |
| full | 9999px | 头像 |

---

## 六、动效规范

| 场景 | 时长 | 缓动 | 说明 |
|------|------|------|------|
| 按钮悬停 | 150ms | ease | 背景色过渡 |
| 弹窗出现 | 250ms | ease-out | 从底部滑入 |
| AI流式输出 | 28ms/字 | linear | 逐字输出 |
| 文件解析进度 | 500ms | ease-in-out | 进度条动画 |
| 引用折叠展开 | 300ms | ease-out | 高度动画 |
| 摘要生成 | 200ms | ease | 淡入效果 |

---

## 七、暗色模式规范

| 元素 | 亮色值 | 暗色值 |
|------|--------|--------|
| 页面背景 | `#F8FAFC` | `#0F172A` |
| 卡片背景 | `#FFFFFF` | `#1E293B` |
| 主色 | `#4F6BED` | `#6780FF` |
| 标题文字 | `#1E293B` | `#F1F5F9` |
| 正文文字 | `#334155` | `#CBD5E1` |
| 次级文字 | `#64748B` | `#94A3B8` |
| 分割线 | `#E2E8F0` | `#334155` |
| AI气泡 | `#F8FAFC` | `#1E293B` |
| 用户气泡 | `#4F6BED` | `#6780FF` |
| 代码块 | `#1E293B` | `#0F172A` |
| 引用块 | `#EEF1FF` | `#1C2A5E` |

---

## 八、设计禁忌（Do's and Don'ts）

### Do

- 正文使用15px+26px行高，优化长文阅读体验
- 引用内容使用左侧竖线+浅蓝底区分
- 文件预览支持滚动，不截断内容
- 代码块提供语言标识和一键复制
- 摘要卡片使用品牌色浅底突出

### Don't

- 禁止正文行高低于1.6（长文阅读不适）
- 禁止AI回复缺少Markdown渲染能力
- 禁止引用块无视觉区分（与正文混淆）
- 禁止文件预览截断无滚动提示
- 禁止代码块无语法高亮

---

## 九、CSS变量快速参考

```css
:root {
  --kimi-primary: #4F6BED;
  --kimi-primary-50: #EEF1FF;
  --kimi-primary-100: #D5DCFF;
  --kimi-primary-200: #ABB9FF;
  --kimi-primary-300: #8196FF;
  --kimi-primary-400: #6780FF;
  --kimi-primary-500: #4F6BED;
  --kimi-primary-600: #3D56D4;
  --kimi-primary-700: #2E42A8;
  --kimi-primary-800: #1F2D75;
  --kimi-primary-900: #121945;
  --kimi-success: #22C55E;
  --kimi-warning: #EAB308;
  --kimi-error: #EF4444;
  --kimi-text-title: #1E293B;
  --kimi-text-body: #334155;
  --kimi-text-secondary: #64748B;
  --kimi-text-placeholder: #94A3B8;
  --kimi-border: #E2E8F0;
  --kimi-bg-page: #F8FAFC;
  --kimi-bg-card: #FFFFFF;
  --kimi-spacing-xs: 4px;
  --kimi-spacing-sm: 8px;
  --kimi-spacing-md: 12px;
  --kimi-spacing-lg: 16px;
  --kimi-spacing-xl: 24px;
  --kimi-spacing-2xl: 32px;
  --kimi-spacing-3xl: 48px;
  --kimi-radius-sm: 4px;
  --kimi-radius-md: 8px;
  --kimi-radius-lg: 12px;
  --kimi-radius-xl: 16px;
  --kimi-radius-full: 9999px;
  --kimi-font-family: 'Noto Sans SC', 'PingFang SC', -apple-system, sans-serif;
  --kimi-font-serif: 'Noto Serif SC', 'Source Han Serif SC', Georgia, serif;
  --kimi-font-mono: 'JetBrains Mono', 'Fira Code', Consolas, monospace;
}
```
