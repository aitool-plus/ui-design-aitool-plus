# 百川智能（Baichuan）设计规范

> **品牌主色**: `#059669`（百川绿）| **平台**: Web | **关键词**: 百川绿/知识汇聚/中文大模型

---

## 一、设计价值观与原则

1. **汇聚百川**：绿色传递知识汇聚与流淌，海纳百川有容乃大
2. **中文深耕**：专注中文大模型，界面中文排版优先、阅读体验极致
3. **知识流淌**：信息如水流般自然呈现，层次清晰、逻辑流畅
4. **开放生态**：开源模型驱动，开发者社区友好

---

## 二、配色体系

### 品牌主色色板（百川绿 #059669）

| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | `#ECFDF5` | 浅底背景 |
| 100 | `#D1FAE5` | 标签底色 |
| 200 | `#A7F3D0` | 图标浅色态 |
| 300 | `#6EE7B7` | 辅助强调 |
| 400 | `#34D399` | 悬停态 |
| 500 | `#059669` | **品牌主色**，主按钮、链接 |
| 600 | `#047857` | 按压态 |
| 700 | `#065F46` | 深色强调 |
| 800 | `#064E3B` | 暗色模式主色 |
| 900 | `#022C22` | 极深背景 |

### 功能色

| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | `#059669` | 与品牌色统一 |
| 警告 | `#F59E0B` | 提示注意 |
| 错误 | `#EF4444` | 请求失败 |
| 信息 | `#0EA5E9` | 数据说明 |

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
| 品牌渐变 | `linear-gradient(135deg, #059669, #34D399)` | Hero区域 |
| 汇聚渐变 | `linear-gradient(90deg, #059669, #0EA5E9)` | 知识流淌装饰 |
| 自然渐变 | `linear-gradient(180deg, #ECFDF5, #F8FAFC)` | 内容区背景 |

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
| 主要按钮 | 36px | 8px | `#059669` | `#FFFFFF` | 0 16px |
| 次要按钮 | 36px | 8px | `#ECFDF5` | `#059669` | 0 16px |
| 文字按钮 | 32px | 4px | transparent | `#059669` | 0 8px |

### 卡片

| 类型 | 圆角 | 阴影 | 内边距 | 背景 |
|------|------|------|--------|------|
| 对话卡片 | 12px | none | 16px | `#F8FAFC` |
| 模型卡片 | 12px | `0 2px 8px rgba(0,0,0,0.06)` | 20px | `#FFFFFF` |
| 知识卡片 | 8px | none | 12px 16px | `#ECFDF5`，左侧3px #059669 |

### 导航栏

- 高度：56px；背景：`#FFFFFF`；底部边框：1px solid `#E2E8F0`

### 弹窗

- 圆角：12px；遮罩：`rgba(0,0,0,0.4)`；背景：`#FFFFFF`

### 输入框

- 高度：40px；圆角：8px；背景：`#FFFFFF`；边框：1px solid `#E2E8F0`
- 聚焦边框：1px solid `#059669`；聚焦阴影：`0 0 0 3px rgba(5,150,105,0.12)`

### AI对话组件

| 组件 | 规格 |
|------|------|
| 用户气泡 | 背景`#059669`，文字`#FFFFFF`，圆角16px 16px 4px 16px，内边距12px 16px |
| AI气泡 | 背景`#F8FAFC`，文字`#334155`，圆角16px 16px 16px 4px，内边距12px 16px |
| 代码块 | 背景`#0F172A`，文字`#E2E8F0`，圆角8px，字号13px，行高20px，内边距16px |
| Markdown标题 | H1 18px/600，H2 16px/500，H3 14px/500 |
| Markdown代码 | 背景`#ECFDF5`，文字`#047857`，圆角4px，内边距2px 6px，字号13px |

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
| 知识引用展开 | 250ms | ease-out | 高度动画 |

---

## 七、暗色模式规范

| 元素 | 亮色值 | 暗色值 |
|------|--------|--------|
| 页面背景 | `#F8FAFC` | `#0A0F0D` |
| 卡片背景 | `#FFFFFF` | `#1A2420` |
| 主色 | `#059669` | `#34D399` |
| 标题文字 | `#0F172A` | `#F1F5F9` |
| 正文文字 | `#334155` | `#CBD5E1` |
| 次级文字 | `#64748B` | `#94A3B8` |
| 分割线 | `#E2E8F0` | `#2A3A34` |
| AI气泡 | `#F8FAFC` | `#1A2420` |
| 用户气泡 | `#059669` | `#34D399` |
| 代码块 | `#0F172A` | `#050A08` |

---

## 八、设计禁忌（Do's and Don'ts）

### Do

- 品牌绿`#059669`作为唯一强调色
- 中文排版优先，行高不低于1.6
- 知识引用使用左侧竖线+浅绿底
- 暗色模式使用深绿底色而非纯黑

### Don't

- 禁止暗色模式使用纯黑底色
- 禁止中文行高低于1.6
- 禁止绿色与蓝色同时作为主强调色
- 禁止正文使用`#94A3B8`以下色值

---

## 九、CSS变量快速参考

```css
:root {
  --baichuan-primary: #059669;
  --baichuan-primary-50: #ECFDF5;
  --baichuan-primary-100: #D1FAE5;
  --baichuan-primary-200: #A7F3D0;
  --baichuan-primary-300: #6EE7B7;
  --baichuan-primary-400: #34D399;
  --baichuan-primary-500: #059669;
  --baichuan-primary-600: #047857;
  --baichuan-primary-700: #065F46;
  --baichuan-primary-800: #064E3B;
  --baichuan-primary-900: #022C22;
  --baichuan-success: #059669;
  --baichuan-warning: #F59E0B;
  --baichuan-error: #EF4444;
  --baichuan-info: #0EA5E9;
  --baichuan-text-title: #0F172A;
  --baichuan-text-body: #334155;
  --baichuan-text-secondary: #64748B;
  --baichuan-text-placeholder: #94A3B8;
  --baichuan-border: #E2E8F0;
  --baichuan-bg-page: #F8FAFC;
  --baichuan-bg-card: #FFFFFF;
  --baichuan-spacing-xs: 4px;
  --baichuan-spacing-sm: 8px;
  --baichuan-spacing-md: 12px;
  --baichuan-spacing-lg: 16px;
  --baichuan-spacing-xl: 24px;
  --baichuan-spacing-2xl: 32px;
  --baichuan-spacing-3xl: 48px;
  --baichuan-radius-sm: 4px;
  --baichuan-radius-md: 8px;
  --baichuan-radius-lg: 12px;
  --baichuan-radius-xl: 16px;
  --baichuan-radius-full: 9999px;
  --baichuan-font-family: 'Noto Sans SC', 'PingFang SC', -apple-system, sans-serif;
  --baichuan-font-mono: 'JetBrains Mono', 'Fira Code', Consolas, monospace;
}
```
