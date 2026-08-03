# 智谱AI（Zhipu AI）设计规范

> **品牌主色**: `#3B82F6`（学术蓝绿）| **平台**: Web | **关键词**: 学术蓝绿/知识引擎/国产大模型

---

## 一、设计价值观与原则

1. **学术严谨**：界面设计传递知识引擎的专业与权威，信息呈现结构化
2. **知识引擎**：以知识图谱为核心，回答有据可查、来源可追溯
3. **智能普惠**：GLM大模型能力人人可用，交互自然直觉
4. **开放协作**：开源精神驱动，界面支持多模型切换与对比

---

## 二、配色体系

### 品牌主色色板（学术蓝绿 #3B82F6）

| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | `#EFF6FF` | 浅底背景、选中高亮 |
| 100 | `#DBEAFE` | 标签底色、悬浮提示 |
| 200 | `#BFDBFE` | 次级图标浅色 |
| 300 | `#93C5FD` | 辅助强调 |
| 400 | `#60A5FA` | 悬停态 |
| 500 | `#3B82F6` | **品牌主色**，主按钮、链接 |
| 600 | `#2563EB` | 按压态 |
| 700 | `#1D4ED8` | 深色强调 |
| 800 | `#1E40AF` | 暗色模式主色 |
| 900 | `#1E3A8A` | 极深背景 |

### 功能色

| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | `#10B981` | 模型加载成功、操作完成 |
| 警告 | `#F59E0B` | Token不足提示 |
| 错误 | `#EF4444` | 请求失败、参数错误 |
| 信息 | `#3B82F6` | 与品牌色统一 |

### 中性色

| 名称 | 色值 | 用途 |
|------|------|------|
| 标题 | `#111827` | 一级标题 |
| 正文 | `#374151` | 正文内容 |
| 次级 | `#6B7280` | 辅助说明 |
| 占位 | `#9CA3AF` | 占位文字 |
| 分割 | `#E5E7EB` | 分割线、边框 |
| 浅底 | `#F9FAFB` | 页面底色 |
| 卡片 | `#FFFFFF` | 卡片底色 |

### 渐变色

| 名称 | 值 | 用途 |
|------|-----|------|
| 品牌渐变 | `linear-gradient(135deg, #3B82F6, #60A5FA)` | Hero区域 |
| 知识渐变 | `linear-gradient(90deg, #3B82F6, #10B981)` | 知识图谱装饰 |
| 学术渐变 | `linear-gradient(180deg, #EFF6FF, #FFFFFF)` | 内容区背景 |

---

## 三、字体排版体系

### 字体家族

- **主字体**: `'Noto Sans SC', 'PingFang SC', -apple-system, BlinkMacSystemFont, sans-serif`
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
| Micro | 11px | 16px | 400 | 标签、参数 |

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
| 主要按钮 | 36px | 8px | `#3B82F6` | `#FFFFFF` | 0 16px |
| 次要按钮 | 36px | 8px | `#EFF6FF` | `#3B82F6` | 0 16px |
| 文字按钮 | 32px | 4px | transparent | `#3B82F6` | 0 8px |
| 模型切换 | 32px | 6px | `#F9FAFB` | `#374151` | 0 12px，边框1px #E5E7EB |

### 卡片

| 类型 | 圆角 | 阴影 | 内边距 | 背景 |
|------|------|------|--------|------|
| 对话卡片 | 12px | none | 16px | `#F9FAFB` |
| 模型卡片 | 12px | `0 1px 3px rgba(0,0,0,0.06)` | 20px | `#FFFFFF` |
| 知识卡片 | 8px | none | 12px 16px | `#EFF6FF`，左侧3px #3B82F6 |

### 导航栏

- 高度：56px；背景：`#FFFFFF`；底部边框：1px solid `#E5E7EB`
- 左侧Logo+模型选择器，中间对话标题，右侧API文档+用户

### 弹窗

- 圆角：12px；遮罩：`rgba(0,0,0,0.4)`；背景：`#FFFFFF`
- 标题区：内边距20px 24px，字号16px，字重500

### 输入框

- 高度：40px；圆角：8px；背景：`#FFFFFF`；边框：1px solid `#E5E7EB`
- 聚焦边框：1px solid `#3B82F6`；聚焦阴影：`0 0 0 3px rgba(59,130,246,0.1)`

### AI对话组件

| 组件 | 规格 |
|------|------|
| 用户气泡 | 背景`#3B82F6`，文字`#FFFFFF`，圆角16px 16px 4px 16px，内边距12px 16px |
| AI气泡 | 背景`#F9FAFB`，文字`#374151`，圆角16px 16px 16px 4px，内边距12px 16px |
| 知识引用 | 背景`#EFF6FF`，左侧3px `#3B82F6`，圆角0 8px 8px 0，内边距12px 16px |
| 代码块 | 背景`#1E293B`，文字`#E2E8F0`，圆角8px，字号13px，行高20px，内边距16px |
| Markdown标题 | H1 18px/600，H2 16px/500，H3 14px/500 |
| Markdown代码 | 背景`#EFF6FF`，文字`#3B82F6`，圆角4px，内边距2px 6px，字号13px |

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
| 弹窗出现 | 250ms | ease-out | 从中心缩放 |
| AI流式输出 | 28ms/字 | linear | 逐Token输出 |
| 模型切换 | 300ms | ease-in-out | 淡入淡出 |
| 知识引用展开 | 250ms | ease-out | 高度动画 |

---

## 七、暗色模式规范

| 元素 | 亮色值 | 暗色值 |
|------|--------|--------|
| 页面背景 | `#F9FAFB` | `#0F172A` |
| 卡片背景 | `#FFFFFF` | `#1E293B` |
| 主色 | `#3B82F6` | `#60A5FA` |
| 标题文字 | `#111827` | `#F1F5F9` |
| 正文文字 | `#374151` | `#CBD5E1` |
| 次级文字 | `#6B7280` | `#94A3B8` |
| 分割线 | `#E5E7EB` | `#334155` |
| AI气泡 | `#F9FAFB` | `#1E293B` |
| 用户气泡 | `#3B82F6` | `#60A5FA` |
| 代码块 | `#1E293B` | `#0F172A` |

---

## 八、设计禁忌（Do's and Don'ts）

### Do

- 知识引用使用左侧竖线+浅蓝底清晰标注来源
- 模型切换器始终可见，支持快速切换GLM系列
- 代码块提供语言标识和复制功能
- 学术场景使用结构化排版（有序列表、表格）

### Don't

- 禁止知识引用无来源标注
- 禁止模型切换隐藏在深层菜单
- 禁止AI回复缺少引用溯源能力
- 禁止正文使用`#9CA3AF`以下色值

---

## 九、CSS变量快速参考

```css
:root {
  --zhipu-primary: #3B82F6;
  --zhipu-primary-50: #EFF6FF;
  --zhipu-primary-100: #DBEAFE;
  --zhipu-primary-200: #BFDBFE;
  --zhipu-primary-300: #93C5FD;
  --zhipu-primary-400: #60A5FA;
  --zhipu-primary-500: #3B82F6;
  --zhipu-primary-600: #2563EB;
  --zhipu-primary-700: #1D4ED8;
  --zhipu-primary-800: #1E40AF;
  --zhipu-primary-900: #1E3A8A;
  --zhipu-success: #10B981;
  --zhipu-warning: #F59E0B;
  --zhipu-error: #EF4444;
  --zhipu-text-title: #111827;
  --zhipu-text-body: #374151;
  --zhipu-text-secondary: #6B7280;
  --zhipu-text-placeholder: #9CA3AF;
  --zhipu-border: #E5E7EB;
  --zhipu-bg-page: #F9FAFB;
  --zhipu-bg-card: #FFFFFF;
  --zhipu-spacing-xs: 4px;
  --zhipu-spacing-sm: 8px;
  --zhipu-spacing-md: 12px;
  --zhipu-spacing-lg: 16px;
  --zhipu-spacing-xl: 24px;
  --zhipu-spacing-2xl: 32px;
  --zhipu-spacing-3xl: 48px;
  --zhipu-radius-sm: 4px;
  --zhipu-radius-md: 8px;
  --zhipu-radius-lg: 12px;
  --zhipu-radius-xl: 16px;
  --zhipu-radius-full: 9999px;
  --zhipu-font-family: 'Noto Sans SC', 'PingFang SC', -apple-system, sans-serif;
  --zhipu-font-mono: 'JetBrains Mono', 'Fira Code', Consolas, monospace;
}
```
