# DeepSeek 设计规范

> **品牌主色**: `#4D6BFE`（深度蓝紫）| **平台**: Web | **关键词**: 深度蓝紫/开源推理/暗色科技

---

## 一、设计价值观与原则

1. **深度思考**：界面克制留白，引导用户专注推理与思考过程
2. **开源透明**：设计语言开放清晰，组件状态可感知、可预期
3. **暗色优先**：深色界面降低视觉疲劳，长时间对话舒适
4. **极简交互**：去除冗余装饰，内容即界面，对话即核心

---

## 二、配色体系

### 品牌主色色板（深度蓝紫 #4D6BFE）

| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | `#EEF0FF` | 极浅底色、标记高亮 |
| 100 | `#D5DAFF` | 次级高亮背景 |
| 200 | `#ABB4FF` | 图标浅色态 |
| 300 | `#818EFF` | 辅助强调 |
| 400 | `#677AFF` | 悬停态 |
| 500 | `#4D6BFE` | **品牌主色**，主按钮、链接 |
| 600 | `#3B55E0` | 按压态 |
| 700 | `#2A3FB5` | 深色强调 |
| 800 | `#1C2A80` | 暗色模式主色 |
| 900 | `#0F1850` | 极深背景 |

### 功能色

| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | `#10B981` | 代码运行成功、连接正常 |
| 警告 | `#F59E0B` | Token即将耗尽 |
| 错误 | `#EF4444` | 运行错误、请求失败 |
| 信息 | `#4D6BFE` | 与品牌色统一，引导提示 |

### 中性色（暗色优先）

| 名称 | 色值 | 用途 |
|------|------|------|
| 标题 | `#F1F5F9` | 一级标题 |
| 正文 | `#CBD5E1` | 正文内容 |
| 次级 | `#94A3B8` | 辅助说明、时间戳 |
| 占位 | `#64748B` | 占位文字 |
| 分割 | `#334155` | 分割线、边框 |
| 表面 | `#1E293B` | 卡片、弹窗底色 |
| 深底 | `#0F172A` | 页面底色 |
| 极深 | `#020617` | 代码块背景 |

### 渐变色

| 名称 | 值 | 用途 |
|------|-----|------|
| 品牌渐变 | `linear-gradient(135deg, #4D6BFE, #818EFF)` | Hero区域、Logo光晕 |
| 推理渐变 | `linear-gradient(90deg, #4D6BFE, #10B981)` | 思考链路指示 |
| 深空渐变 | `linear-gradient(180deg, #0F172A, #1E293B)` | 页面背景 |

---

## 三、字体排版体系

### 字体家族

- **主字体**: `Inter, -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif`
- **中文字体**: `'Noto Sans SC', 'PingFang SC', 'Microsoft YaHei', sans-serif`
- **代码字体**: `'JetBrains Mono', 'Fira Code', 'Cascadia Code', monospace`

### 字号阶梯

| 层级 | 字号 | 行高 | 字重 | 用途 |
|------|------|------|------|------|
| H1 | 24px | 32px | 600 | 页面标题 |
| H2 | 20px | 28px | 600 | 模块标题 |
| H3 | 16px | 24px | 500 | 卡片标题 |
| Body | 14px | 22px | 400 | 正文、对话内容 |
| Code | 13px | 20px | 400 | 代码块内容 |
| Caption | 12px | 18px | 400 | 辅助说明 |
| Micro | 11px | 16px | 400 | Token计数、标签 |

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
| 主要按钮 | 36px | 8px | `#4D6BFE` | `#FFFFFF` | 0 16px |
| 次要按钮 | 36px | 8px | `#1E293B` | `#4D6BFE` | 0 16px，边框1px #4D6BFE |
| 幽灵按钮 | 32px | 6px | transparent | `#CBD5E1` | 0 12px |
| 图标按钮 | 32px | 6px | `#1E293B` | `#94A3B8` | 8px |

### 卡片

| 类型 | 圆角 | 阴影 | 内边距 | 背景 |
|------|------|------|--------|------|
| 对话卡片 | 12px | none | 16px | `#1E293B` |
| 功能卡片 | 8px | `0 1px 3px rgba(0,0,0,0.3)` | 20px | `#1E293B` |
| 代码卡片 | 8px | none | 0 | `#020617` |

### 导航栏

- 高度：52px；背景：`#0F172A`；底部边框：1px solid `#1E293B`
- 左侧Logo+品牌名，中间模型切换，右侧设置+用户

### 弹窗

- 圆角：12px；遮罩：`rgba(0,0,0,0.6)`；背景：`#1E293B`
- 标题区：内边距20px 24px，字号16px，字重500，色`#F1F5F9`
- 操作区按钮：主按钮品牌色，次按钮`#334155`背景

### 输入框

- 高度：40px；圆角：8px；背景：`#0F172A`；边框：1px solid `#334155`
- 聚焦边框：1px solid `#4D6BFE`；聚焦阴影：`0 0 0 2px rgba(77,107,254,0.2)`
- 占位文字色：`#64748B`

### AI对话组件

| 组件 | 规格 |
|------|------|
| 用户气泡 | 背景`#4D6BFE`，文字`#FFFFFF`，圆角16px 16px 4px 16px，内边距12px 16px |
| AI气泡 | 背景`#1E293B`，文字`#CBD5E1`，圆角16px 16px 16px 4px，内边距12px 16px |
| 思考过程 | 背景`#0F172A`，文字`#64748B`，左侧2px `#4D6BFE`竖线，内边距12px 16px |
| 代码块 | 背景`#020617`，文字`#E2E8F0`，圆角8px，字号13px，行高20px，内边距16px |
| 代码头部 | 背景`#1E293B`，文字`#94A3B8`，字号12px，语言标签+复制按钮 |
| Markdown标题 | H1 18px/600，H2 16px/500，H3 14px/500，色`#F1F5F9` |
| Markdown代码 | 背景`#0F172A`，文字`#818EFF`，圆角4px，内边距2px 6px，字号13px |
| Markdown链接 | 色`#4D6BFE`，下划线，悬停色`#818EFF` |

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
| none | 0px | 代码块内部 |
| sm | 4px | 标签、行内代码 |
| md | 8px | 按钮、输入框、代码块 |
| lg | 12px | 卡片、弹窗 |
| xl | 16px | 对话气泡 |
| full | 9999px | 头像、药丸标签 |

---

## 六、动效规范

| 场景 | 时长 | 缓动 | 说明 |
|------|------|------|------|
| 按钮悬停 | 150ms | ease | 背景色过渡 |
| 弹窗出现 | 200ms | ease-out | 从中心缩放+淡入 |
| 弹窗关闭 | 150ms | ease-in | 缩放+淡出 |
| AI流式输出 | 25ms/字 | linear | 逐Token输出 |
| 思考过程展开 | 300ms | ease-out | 高度动画+淡入 |
| 代码块展开 | 250ms | ease-out | 高度动画 |
| 侧边栏切换 | 250ms | ease-in-out | 宽度动画 |

---

## 七、暗色模式规范

DeepSeek默认即为暗色模式，亮色模式为可选切换：

| 元素 | 暗色值（默认） | 亮色值 |
|------|----------------|--------|
| 页面背景 | `#0F172A` | `#F8FAFC` |
| 卡片背景 | `#1E293B` | `#FFFFFF` |
| 主色 | `#4D6BFE` | `#4D6BFE` |
| 标题文字 | `#F1F5F9` | `#0F172A` |
| 正文文字 | `#CBD5E1` | `#334155` |
| 次级文字 | `#94A3B8` | `#64748B` |
| 分割线 | `#334155` | `#E2E8F0` |
| 代码块 | `#020617` | `#1E293B` |

---

## 八、设计禁忌（Do's and Don'ts）

### Do

- 默认使用暗色界面，降低长时间对话视觉疲劳
- AI思考过程使用左侧竖线+浅色文字区分
- 代码块使用极深背景+语法高亮
- 品牌色`#4D6BFE`仅用于主操作和关键强调
- 对话区域最大化，减少非必要UI元素

### Don't

- 禁止在暗色界面使用纯白`#FFFFFF`作为大面积背景
- 禁止用户气泡与AI气泡使用相同背景色
- 禁止代码块缺少语言标识和复制按钮
- 禁止思考过程与正式回复视觉无区分
- 禁止正文使用`#64748B`以下色值（对比度不足）

---

## 九、CSS变量快速参考

```css
:root {
  --deepseek-primary: #4D6BFE;
  --deepseek-primary-50: #EEF0FF;
  --deepseek-primary-100: #D5DAFF;
  --deepseek-primary-200: #ABB4FF;
  --deepseek-primary-300: #818EFF;
  --deepseek-primary-400: #677AFF;
  --deepseek-primary-500: #4D6BFE;
  --deepseek-primary-600: #3B55E0;
  --deepseek-primary-700: #2A3FB5;
  --deepseek-primary-800: #1C2A80;
  --deepseek-primary-900: #0F1850;
  --deepseek-success: #10B981;
  --deepseek-warning: #F59E0B;
  --deepseek-error: #EF4444;
  --deepseek-text-title: #F1F5F9;
  --deepseek-text-body: #CBD5E1;
  --deepseek-text-secondary: #94A3B8;
  --deepseek-text-placeholder: #64748B;
  --deepseek-border: #334155;
  --deepseek-bg-page: #0F172A;
  --deepseek-bg-card: #1E293B;
  --deepseek-bg-code: #020617;
  --deepseek-spacing-xs: 4px;
  --deepseek-spacing-sm: 8px;
  --deepseek-spacing-md: 12px;
  --deepseek-spacing-lg: 16px;
  --deepseek-spacing-xl: 24px;
  --deepseek-spacing-2xl: 32px;
  --deepseek-spacing-3xl: 48px;
  --deepseek-radius-sm: 4px;
  --deepseek-radius-md: 8px;
  --deepseek-radius-lg: 12px;
  --deepseek-radius-xl: 16px;
  --deepseek-radius-full: 9999px;
  --deepseek-font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
  --deepseek-font-mono: 'JetBrains Mono', 'Fira Code', 'Cascadia Code', monospace;
}
```
