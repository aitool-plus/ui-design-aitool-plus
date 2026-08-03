# Moonshot 设计规范

> **品牌主色**: `#94A3B8`（月光银）| **平台**: Web | **关键词**: 月光银/登月精神/长文本

---

## 一、设计价值观与原则

1. **登月精神**：以登月为隐喻，界面极简克制，追求极致长文本能力
2. **月光银调**：银灰色传递冷静理性，专注内容而非装饰
3. **长文本极致**：超长上下文窗口，界面为长文阅读深度优化
4. **极简克制**：去除一切非必要装饰，内容即界面

---

## 二、配色体系

### 品牌主色色板（月光银 #94A3B8）

| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | `#F8FAFC` | 浅底背景 |
| 100 | `#F1F5F9` | 标签底色 |
| 200 | `#E2E8F0` | 图标浅色态 |
| 300 | `#CBD5E1` | 辅助强调 |
| 400 | `#94A3B8` | **品牌主色**，主按钮、链接 |
| 500 | `#64748B` | 深色强调 |
| 600 | `#475569` | 标题文字 |
| 700 | `#334155` | 正文文字 |
| 800 | `#1E293B` | 深色背景 |
| 900 | `#0F172A` | 极深背景 |

### 功能色

| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | `#10B981` | 操作成功 |
| 警告 | `#F59E0B` | 提示注意 |
| 错误 | `#EF4444` | 请求失败 |
| 信息 | `#94A3B8` | 与品牌色统一 |
| 强调蓝 | `#3B82F6` | 链接、关键操作 |

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
| 月光渐变 | `linear-gradient(135deg, #94A3B8, #CBD5E1)` | Hero区域 |
| 银河渐变 | `linear-gradient(180deg, #0F172A, #1E293B, #334155)` | 暗色背景 |
| 登月渐变 | `linear-gradient(90deg, #94A3B8, #3B82F6)` | 能力展示 |

---

## 三、字体排版体系

### 字体家族

- **主字体**: `'Inter', 'Noto Sans SC', -apple-system, BlinkMacSystemFont, sans-serif`
- **代码字体**: `'JetBrains Mono', 'Fira Code', Consolas, monospace`

### 字号阶梯

| 层级 | 字号 | 行高 | 字重 | 用途 |
|------|------|------|------|------|
| H1 | 22px | 30px | 600 | 页面标题 |
| H2 | 18px | 26px | 600 | 模块标题 |
| H3 | 16px | 24px | 500 | 卡片标题 |
| Body | 15px | 26px | 400 | 正文（长文优化行高） |
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
| 主要按钮 | 36px | 8px | `#334155` | `#FFFFFF` | 0 16px |
| 次要按钮 | 36px | 8px | `#F1F5F9` | `#334155` | 0 16px |
| 文字按钮 | 32px | 4px | transparent | `#3B82F6` | 0 8px |

### 卡片

| 类型 | 圆角 | 阴影 | 内边距 | 背景 |
|------|------|------|--------|------|
| 对话卡片 | 12px | none | 16px | `#F8FAFC` |
| 文档卡片 | 8px | `0 1px 2px rgba(0,0,0,0.04)` | 20px | `#FFFFFF` |

### 导航栏

- 高度：52px；背景：`#FFFFFF`；底部边框：1px solid `#E2E8F0`
- 极简导航：左侧Logo，中间标题，右侧设置

### 弹窗

- 圆角：12px；遮罩：`rgba(0,0,0,0.4)`；背景：`#FFFFFF`

### 输入框

- 高度：40px；圆角：8px；背景：`#FFFFFF`；边框：1px solid `#E2E8F0`
- 聚焦边框：1px solid `#94A3B8`；聚焦阴影：`0 0 0 3px rgba(148,163,184,0.15)`

### AI对话组件

| 组件 | 规格 |
|------|------|
| 用户气泡 | 背景`#334155`，文字`#FFFFFF`，圆角16px 16px 4px 16px，内边距12px 16px |
| AI气泡 | 背景`#F8FAFC`，文字`#334155`，圆角16px 16px 16px 4px，内边距12px 16px |
| 代码块 | 背景`#0F172A`，文字`#E2E8F0`，圆角8px，字号13px，行高20px，内边距16px |
| Markdown标题 | H1 18px/600，H2 16px/500，H3 14px/500 |
| Markdown代码 | 背景`#F1F5F9`，文字`#475569`，圆角4px，内边距2px 6px，字号13px |
| Markdown链接 | 色`#3B82F6`，悬停下划线 |

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
| 长文滚动 | 0ms | linear | 原生滚动，无动画干扰 |

---

## 七、暗色模式规范

| 元素 | 亮色值 | 暗色值 |
|------|--------|--------|
| 页面背景 | `#F8FAFC` | `#0F172A` |
| 卡片背景 | `#FFFFFF` | `#1E293B` |
| 主色 | `#94A3B8` | `#CBD5E1` |
| 标题文字 | `#0F172A` | `#F1F5F9` |
| 正文文字 | `#334155` | `#CBD5E1` |
| 次级文字 | `#64748B` | `#94A3B8` |
| 分割线 | `#E2E8F0` | `#334155` |
| AI气泡 | `#F8FAFC` | `#1E293B` |
| 用户气泡 | `#334155` | `#475569` |
| 代码块 | `#0F172A` | `#020617` |

---

## 八、设计禁忌（Do's and Don'ts）

### Do

- 银灰色系贯穿全站，极简克制
- 长文阅读使用15px+26px行高优化
- 链接使用蓝色`#3B82F6`而非银灰色（可辨识度）
- 代码块使用深色背景+语法高亮

### Don't

- 禁止大面积使用鲜艳色彩（破坏极简调性）
- 禁止正文行高低于1.6
- 禁止链接使用银灰色（与正文无法区分）
- 禁止添加非必要装饰元素

---

## 九、CSS变量快速参考

```css
:root {
  --moonshot-primary: #94A3B8;
  --moonshot-primary-50: #F8FAFC;
  --moonshot-primary-100: #F1F5F9;
  --moonshot-primary-200: #E2E8F0;
  --moonshot-primary-300: #CBD5E1;
  --moonshot-primary-400: #94A3B8;
  --moonshot-primary-500: #64748B;
  --moonshot-primary-600: #475569;
  --moonshot-primary-700: #334155;
  --moonshot-primary-800: #1E293B;
  --moonshot-primary-900: #0F172A;
  --moonshot-accent: #3B82F6;
  --moonshot-success: #10B981;
  --moonshot-warning: #F59E0B;
  --moonshot-error: #EF4444;
  --moonshot-text-title: #0F172A;
  --moonshot-text-body: #334155;
  --moonshot-text-secondary: #64748B;
  --moonshot-text-placeholder: #94A3B8;
  --moonshot-border: #E2E8F0;
  --moonshot-bg-page: #F8FAFC;
  --moonshot-bg-card: #FFFFFF;
  --moonshot-spacing-xs: 4px;
  --moonshot-spacing-sm: 8px;
  --moonshot-spacing-md: 12px;
  --moonshot-spacing-lg: 16px;
  --moonshot-spacing-xl: 24px;
  --moonshot-spacing-2xl: 32px;
  --moonshot-spacing-3xl: 48px;
  --moonshot-radius-sm: 4px;
  --moonshot-radius-md: 8px;
  --moonshot-radius-lg: 12px;
  --moonshot-radius-xl: 16px;
  --moonshot-radius-full: 9999px;
  --moonshot-font-family: 'Inter', 'Noto Sans SC', -apple-system, sans-serif;
  --moonshot-font-mono: 'JetBrains Mono', 'Fira Code', Consolas, monospace;
}
```
