# 商汤（SenseTime）设计规范

> **品牌主色**: `#7B2D8E`（视觉紫）| **平台**: Web | **关键词**: 视觉紫/AI视觉/智慧城市

---

## 一、设计价值观与原则

1. **视觉智能**：以计算机视觉为核心，界面注重视觉呈现与图像交互
2. **智慧赋能**：AI赋能百业，界面专业但不冰冷，科技有温度
3. **安全合规**：视觉数据安全第一，隐私保护贯穿设计
4. **场景深耕**：智慧城市、医疗、教育等垂直场景深度定制

---

## 二、配色体系

### 品牌主色色板（视觉紫 #7B2D8E）

| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | `#F5F0F7` | 浅底背景 |
| 100 | `#E6D9ED` | 标签底色 |
| 200 | `#CDB3DB` | 图标浅色态 |
| 300 | `#B48CC9` | 辅助强调 |
| 400 | `#9A66B7` | 悬停态 |
| 500 | `#7B2D8E` | **品牌主色**，主按钮、链接 |
| 600 | `#652476` | 按压态 |
| 700 | `#501C5E` | 深色强调 |
| 800 | `#3B1346` | 暗色模式主色 |
| 900 | `#260A2E` | 极深背景 |

### 功能色

| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | `#10B981` | 识别成功、操作完成 |
| 警告 | `#F59E0B` | 置信度低提示 |
| 错误 | `#EF4444` | 识别失败 |
| 信息 | `#3B82F6` | 数据说明 |

### 中性色

| 名称 | 色值 | 用途 |
|------|------|------|
| 标题 | `#1A1A2E` | 一级标题 |
| 正文 | `#374151` | 正文内容 |
| 次级 | `#6B7280` | 辅助说明 |
| 占位 | `#9CA3AF` | 占位文字 |
| 分割 | `#E5E7EB` | 分割线 |
| 浅底 | `#F9FAFB` | 页面底色 |
| 卡片 | `#FFFFFF` | 卡片底色 |

### 渐变色

| 名称 | 值 | 用途 |
|------|-----|------|
| 品牌渐变 | `linear-gradient(135deg, #7B2D8E, #B48CC9)` | Hero区域 |
| 视觉渐变 | `linear-gradient(90deg, #7B2D8E, #3B82F6)` | 视觉AI能力展示 |
| 深紫渐变 | `linear-gradient(180deg, #1A1A2E, #260A2E)` | 暗色页面背景 |

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
| 主要按钮 | 36px | 8px | `#7B2D8E` | `#FFFFFF` | 0 16px |
| 次要按钮 | 36px | 8px | `#F5F0F7` | `#7B2D8E` | 0 16px |
| 文字按钮 | 32px | 4px | transparent | `#7B2D8E` | 0 8px |

### 卡片

| 类型 | 圆角 | 阴影 | 内边距 | 背景 |
|------|------|------|--------|------|
| 对话卡片 | 12px | none | 16px | `#F9FAFB` |
| 识别结果卡片 | 12px | `0 2px 8px rgba(0,0,0,0.06)` | 20px | `#FFFFFF` |
| 图像标注卡片 | 8px | none | 0 | `#000000`（覆盖层） |

### 导航栏

- 高度：56px；背景：`#FFFFFF`；底部边框：1px solid `#E5E7EB`

### 弹窗

- 圆角：12px；遮罩：`rgba(0,0,0,0.5)`；背景：`#FFFFFF`

### 输入框

- 高度：40px；圆角：8px；背景：`#FFFFFF`；边框：1px solid `#E5E7EB`
- 聚焦边框：1px solid `#7B2D8E`；聚焦阴影：`0 0 0 3px rgba(123,45,142,0.12)`

### AI对话组件

| 组件 | 规格 |
|------|------|
| 用户气泡 | 背景`#7B2D8E`，文字`#FFFFFF`，圆角16px 16px 4px 16px，内边距12px 16px |
| AI气泡 | 背景`#F9FAFB`，文字`#374151`，圆角16px 16px 16px 4px，内边距12px 16px |
| 代码块 | 背景`#1E293B`，文字`#E2E8F0`，圆角8px，字号13px，行高20px，内边距16px |
| Markdown标题 | H1 18px/600，H2 16px/500，H3 14px/500 |
| Markdown代码 | 背景`#F5F0F7`，文字`#652476`，圆角4px，内边距2px 6px，字号13px |

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
| 图像识别 | 500ms | ease-in-out | 标注框渐显 |

---

## 七、暗色模式规范

| 元素 | 亮色值 | 暗色值 |
|------|--------|--------|
| 页面背景 | `#F9FAFB` | `#0F0F1A` |
| 卡片背景 | `#FFFFFF` | `#1A1A2E` |
| 主色 | `#7B2D8E` | `#9A66B7` |
| 标题文字 | `#1A1A2E` | `#F1F5F9` |
| 正文文字 | `#374151` | `#CBD5E1` |
| 次级文字 | `#6B7280` | `#94A3B8` |
| 分割线 | `#E5E7EB` | `#334155` |
| AI气泡 | `#F9FAFB` | `#1A1A2E` |
| 用户气泡 | `#7B2D8E` | `#9A66B7` |
| 代码块 | `#1E293B` | `#0F0F1A` |

---

## 八、设计禁忌（Do's and Don'ts）

### Do

- 图像识别结果使用标注框清晰呈现
- 置信度数据使用进度条或百分比直观展示
- 品牌紫`#7B2D8E`作为唯一强调色
- 暗色模式使用深紫底色而非纯黑

### Don't

- 禁止图像识别结果无标注框
- 禁止置信度数据仅用文字描述
- 禁止暗色模式使用纯黑`#000000`底色
- 禁止紫色与蓝色同时作为主强调色

---

## 九、CSS变量快速参考

```css
:root {
  --sensetime-primary: #7B2D8E;
  --sensetime-primary-50: #F5F0F7;
  --sensetime-primary-100: #E6D9ED;
  --sensetime-primary-200: #CDB3DB;
  --sensetime-primary-300: #B48CC9;
  --sensetime-primary-400: #9A66B7;
  --sensetime-primary-500: #7B2D8E;
  --sensetime-primary-600: #652476;
  --sensetime-primary-700: #501C5E;
  --sensetime-primary-800: #3B1346;
  --sensetime-primary-900: #260A2E;
  --sensetime-success: #10B981;
  --sensetime-warning: #F59E0B;
  --sensetime-error: #EF4444;
  --sensetime-info: #3B82F6;
  --sensetime-text-title: #1A1A2E;
  --sensetime-text-body: #374151;
  --sensetime-text-secondary: #6B7280;
  --sensetime-text-placeholder: #9CA3AF;
  --sensetime-border: #E5E7EB;
  --sensetime-bg-page: #F9FAFB;
  --sensetime-bg-card: #FFFFFF;
  --sensetime-spacing-xs: 4px;
  --sensetime-spacing-sm: 8px;
  --sensetime-spacing-md: 12px;
  --sensetime-spacing-lg: 16px;
  --sensetime-spacing-xl: 24px;
  --sensetime-spacing-2xl: 32px;
  --sensetime-spacing-3xl: 48px;
  --sensetime-radius-sm: 4px;
  --sensetime-radius-md: 8px;
  --sensetime-radius-lg: 12px;
  --sensetime-radius-xl: 16px;
  --sensetime-radius-full: 9999px;
  --sensetime-font-family: 'Noto Sans SC', 'PingFang SC', -apple-system, sans-serif;
  --sensetime-font-mono: 'JetBrains Mono', 'Fira Code', Consolas, monospace;
}
```
