# 阶跃星辰（StepFun）设计规范

> **品牌主色**: `#2563EB`（星辰蓝）| **平台**: Web | **关键词**: 星辰蓝/跃迁智能/多模态

---

## 一、设计价值观与原则

1. **跃迁智能**：以跃迁为隐喻，界面传递突破与进化的科技感
2. **多模态统一**：文本、图像、音频、视频统一交互范式
3. **开发者友好**：API文档清晰，SDK接入便捷，技术社区活跃
4. **星辰大海**：深空蓝为底色，星辰点缀，传递探索精神

---

## 二、配色体系

### 品牌主色色板（星辰蓝 #2563EB）

| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | `#EFF6FF` | 浅底背景 |
| 100 | `#DBEAFE` | 标签底色 |
| 200 | `#BFDBFE` | 图标浅色态 |
| 300 | `#93C5FD` | 辅助强调 |
| 400 | `#60A5FA` | 悬停态 |
| 500 | `#2563EB` | **品牌主色**，主按钮、链接 |
| 600 | `#1D4ED8` | 按压态 |
| 700 | `#1E40AF` | 深色强调 |
| 800 | `#1E3A8A` | 暗色模式主色 |
| 900 | `#172554` | 极深背景 |

### 功能色

| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | `#10B981` | 操作成功 |
| 警告 | `#F59E0B` | 提示注意 |
| 错误 | `#EF4444` | 请求失败 |
| 信息 | `#2563EB` | 与品牌色统一 |

### 中性色

| 名称 | 色值 | 用途 |
|------|------|------|
| 标题 | `#0F172A` | 一级标题 |
| 正文 | `#334155` | 正文内容 |
| 次级 | `#64748B` | 辅助说明 |
| 占位 | `#94A3B8` | 占位文字 |
| 分割 | `#E2E8F0` | 分割线 |
| 浅底 | `#F8FAFC` | 页面底色 |
| 卡片 | `#FFFFFF` | 卡片底色 |

### 渐变色

| 名称 | 值 | 用途 |
|------|-----|------|
| 品牌渐变 | `linear-gradient(135deg, #2563EB, #60A5FA)` | Hero区域 |
| 星辰渐变 | `linear-gradient(180deg, #0F172A, #172554, #1E3A8A)` | 暗色背景 |
| 跃迁渐变 | `linear-gradient(90deg, #2563EB, #8B5CF6)` | 多模态装饰 |

---

## 三、字体排版体系

### 字体家族

- **主字体**: `'Inter', 'Noto Sans SC', -apple-system, BlinkMacSystemFont, sans-serif`
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
| 主要按钮 | 36px | 8px | `#2563EB` | `#FFFFFF` | 0 16px |
| 次要按钮 | 36px | 8px | `#EFF6FF` | `#2563EB` | 0 16px |
| 文字按钮 | 32px | 4px | transparent | `#2563EB` | 0 8px |

### 卡片

| 类型 | 圆角 | 阴影 | 内边距 | 背景 |
|------|------|------|--------|------|
| 对话卡片 | 12px | none | 16px | `#F8FAFC` |
| 模型卡片 | 12px | `0 2px 8px rgba(0,0,0,0.06)` | 20px | `#FFFFFF` |
| API文档卡片 | 8px | `0 1px 3px rgba(0,0,0,0.06)` | 16px | `#F8FAFC` |

### 导航栏

- 高度：56px；背景：`#FFFFFF`；底部边框：1px solid `#E2E8F0`

### 弹窗

- 圆角：12px；遮罩：`rgba(0,0,0,0.4)`；背景：`#FFFFFF`

### 输入框

- 高度：40px；圆角：8px；背景：`#FFFFFF`；边框：1px solid `#E2E8F0`
- 聚焦边框：1px solid `#2563EB`；聚焦阴影：`0 0 0 3px rgba(37,99,235,0.1)`

### AI对话组件

| 组件 | 规格 |
|------|------|
| 用户气泡 | 背景`#2563EB`，文字`#FFFFFF`，圆角16px 16px 4px 16px，内边距12px 16px |
| AI气泡 | 背景`#F8FAFC`，文字`#334155`，圆角16px 16px 16px 4px，内边距12px 16px |
| 代码块 | 背景`#0F172A`，文字`#E2E8F0`，圆角8px，字号13px，行高20px，内边距16px |
| Markdown标题 | H1 18px/600，H2 16px/500，H3 14px/500 |
| Markdown代码 | 背景`#EFF6FF`，文字`#1D4ED8`，圆角4px，内边距2px 6px，字号13px |

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

---

## 七、暗色模式规范

| 元素 | 亮色值 | 暗色值 |
|------|--------|--------|
| 页面背景 | `#F8FAFC` | `#0F172A` |
| 卡片背景 | `#FFFFFF` | `#1E293B` |
| 主色 | `#2563EB` | `#60A5FA` |
| 标题文字 | `#0F172A` | `#F1F5F9` |
| 正文文字 | `#334155` | `#CBD5E1` |
| 次级文字 | `#64748B` | `#94A3B8` |
| 分割线 | `#E2E8F0` | `#334155` |
| AI气泡 | `#F8FAFC` | `#1E293B` |
| 用户气泡 | `#2563EB` | `#60A5FA` |
| 代码块 | `#0F172A` | `#020617` |

---

## 八、设计禁忌（Do's and Don'ts）

### Do

- 品牌蓝`#2563EB`作为唯一强调色
- 代码块使用深空蓝底色，与品牌调性一致
- API文档使用结构化排版
- 暗色模式使用深蓝底色而非纯黑

### Don't

- 禁止暗色模式使用纯黑`#000000`底色
- 禁止代码块无语法高亮
- 禁止正文使用`#94A3B8`以下色值
- 禁止品牌蓝与紫色同时作为主强调色

---

## 九、CSS变量快速参考

```css
:root {
  --stepfun-primary: #2563EB;
  --stepfun-primary-50: #EFF6FF;
  --stepfun-primary-100: #DBEAFE;
  --stepfun-primary-200: #BFDBFE;
  --stepfun-primary-300: #93C5FD;
  --stepfun-primary-400: #60A5FA;
  --stepfun-primary-500: #2563EB;
  --stepfun-primary-600: #1D4ED8;
  --stepfun-primary-700: #1E40AF;
  --stepfun-primary-800: #1E3A8A;
  --stepfun-primary-900: #172554;
  --stepfun-success: #10B981;
  --stepfun-warning: #F59E0B;
  --stepfun-error: #EF4444;
  --stepfun-text-title: #0F172A;
  --stepfun-text-body: #334155;
  --stepfun-text-secondary: #64748B;
  --stepfun-text-placeholder: #94A3B8;
  --stepfun-border: #E2E8F0;
  --stepfun-bg-page: #F8FAFC;
  --stepfun-bg-card: #FFFFFF;
  --stepfun-spacing-xs: 4px;
  --stepfun-spacing-sm: 8px;
  --stepfun-spacing-md: 12px;
  --stepfun-spacing-lg: 16px;
  --stepfun-spacing-xl: 24px;
  --stepfun-spacing-2xl: 32px;
  --stepfun-spacing-3xl: 48px;
  --stepfun-radius-sm: 4px;
  --stepfun-radius-md: 8px;
  --stepfun-radius-lg: 12px;
  --stepfun-radius-xl: 16px;
  --stepfun-radius-full: 9999px;
  --stepfun-font-family: 'Inter', 'Noto Sans SC', -apple-system, sans-serif;
  --stepfun-font-mono: 'JetBrains Mono', 'Fira Code', Consolas, monospace;
}
```
