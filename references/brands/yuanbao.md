# 元宝（Yuanbao）设计规范

> **品牌主色**: `#D4A017`（金融金）| **平台**: Web | **关键词**: 金融金/腾讯系AI/理财助手

---

## 一、设计价值观与原则

1. **财富智慧**：金色传递财富与信任，AI赋能理财决策
2. **腾讯品质**：继承腾讯设计基因，专业可靠、体验流畅
3. **安全可信**：金融场景安全第一，数据加密、隐私保护
4. **智能理财**：AI助手辅助投资分析、风险评估、资产配置

---

## 二、配色体系

### 品牌主色色板（金融金 #D4A017）

| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | `#FEF9E7` | 浅底背景、标记高亮 |
| 100 | `#FDF0C8` | 标签底色 |
| 200 | `#FBE49A` | 图标浅色态 |
| 300 | `#F5D26B` | 辅助强调 |
| 400 | `#E8B93E` | 悬停态 |
| 500 | `#D4A017` | **品牌主色**，主按钮、链接 |
| 600 | `#B8860B` | 按压态 |
| 700 | `#956D09` | 深色强调 |
| 800 | `#6B4F06` | 暗色模式主色 |
| 900 | `#3D2E03` | 极深背景 |

### 功能色

| 类型 | 色值 | 用途 |
|------|------|------|
| 涨/成功 | `#CF3030` | 上涨、盈利（中国股市红涨） |
| 跌/错误 | `#16A34A` | 下跌、亏损（中国股市绿跌） |
| 警告 | `#F59E0B` | 风险提示 |
| 信息 | `#3B82F6` | 数据说明 |

### 中性色

| 名称 | 色值 | 用途 |
|------|------|------|
| 标题 | `#1A1A1A` | 一级标题 |
| 正文 | `#333333` | 正文内容 |
| 次级 | `#666666` | 辅助说明 |
| 占位 | `#999999` | 占位文字 |
| 分割 | `#E5E5E5` | 分割线 |
| 浅底 | `#F5F5F5` | 页面底色 |
| 卡片 | `#FFFFFF` | 卡片底色 |

### 渐变色

| 名称 | 值 | 用途 |
|------|-----|------|
| 品牌渐变 | `linear-gradient(135deg, #D4A017, #F5D26B)` | Hero区域、Logo装饰 |
| 财富渐变 | `linear-gradient(90deg, #D4A017, #B8860B)` | 数据卡片头部 |
| 信任渐变 | `linear-gradient(180deg, #FEF9E7, #FFFFFF)` | 内容区背景 |

---

## 三、字体排版体系

### 字体家族

- **主字体**: `'PingFang SC', 'Noto Sans SC', 'Helvetica Neue', sans-serif`
- **数据字体**: `'DIN Alternate', 'Roboto Mono', 'Tabular Nums', monospace`
- **代码字体**: `'JetBrains Mono', 'Fira Code', Consolas, monospace`

### 字号阶梯

| 层级 | 字号 | 行高 | 字重 | 用途 |
|------|------|------|------|------|
| H1 | 24px | 32px | 600 | 页面标题 |
| H2 | 20px | 28px | 600 | 模块标题 |
| H3 | 16px | 24px | 500 | 卡片标题 |
| 数据 | 28px | 36px | 700 | 核心金融数据 |
| Body | 14px | 22px | 400 | 正文内容 |
| Code | 13px | 20px | 400 | 代码块 |
| Caption | 12px | 18px | 400 | 辅助说明 |

### 字重体系

| 字重 | 值 | 用途 |
|------|-----|------|
| Regular | 400 | 正文、代码 |
| Medium | 500 | 小标题、按钮 |
| Semibold | 600 | 标题 |
| Bold | 700 | 金融数据 |

---

## 四、组件设计规范

### 按钮

| 类型 | 高度 | 圆角 | 背景 | 文字色 | 内边距 |
|------|------|------|------|--------|--------|
| 主要按钮 | 36px | 8px | `#D4A017` | `#FFFFFF` | 0 16px |
| 次要按钮 | 36px | 8px | `#FEF9E7` | `#D4A017` | 0 16px |
| 文字按钮 | 32px | 4px | transparent | `#D4A017` | 0 8px |
| 风险按钮 | 36px | 8px | `#CF3030` | `#FFFFFF` | 0 16px |

### 卡片

| 类型 | 圆角 | 阴影 | 内边距 | 背景 |
|------|------|------|--------|------|
| 对话卡片 | 12px | none | 16px | `#F5F5F5` |
| 数据卡片 | 12px | `0 2px 8px rgba(0,0,0,0.06)` | 20px | `#FFFFFF` |
| 资产卡片 | 16px | `0 4px 16px rgba(212,160,23,0.12)` | 24px | `linear-gradient(135deg, #FEF9E7, #FFFFFF)` |

### 导航栏

- 高度：56px；背景：`#FFFFFF`；底部边框：1px solid `#E5E5E5`
- 左侧Logo，中间功能切换（对话/理财/分析），右侧用户

### 弹窗

- 圆角：12px；遮罩：`rgba(0,0,0,0.5)`；背景：`#FFFFFF`
- 标题区：内边距20px 24px，字号16px，字重500

### 输入框

- 高度：40px；圆角：8px；背景：`#FFFFFF`；边框：1px solid `#E5E5E5`
- 聚焦边框：1px solid `#D4A017`；聚焦阴影：`0 0 0 3px rgba(212,160,23,0.12)`

### AI对话组件

| 组件 | 规格 |
|------|------|
| 用户气泡 | 背景`#D4A017`，文字`#FFFFFF`，圆角16px 16px 4px 16px，内边距12px 16px |
| AI气泡 | 背景`#F5F5F5`，文字`#333333`，圆角16px 16px 16px 4px，内边距12px 16px |
| 数据展示 | 背景`#FEF9E7`，左侧3px `#D4A017`，圆角0 8px 8px 0，内边距12px 16px |
| 代码块 | 背景`#1E1E1E`，文字`#D4D4D4`，圆角8px，字号13px，行高20px，内边距16px |
| Markdown标题 | H1 18px/600，H2 16px/500，H3 14px/500 |
| Markdown代码 | 背景`#FEF9E7`，文字`#956D09`，圆角4px，内边距2px 6px，字号13px |

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
| xl | 16px | 对话气泡、资产卡片 |
| full | 9999px | 头像 |

---

## 六、动效规范

| 场景 | 时长 | 缓动 | 说明 |
|------|------|------|------|
| 按钮悬停 | 150ms | ease | 背景色过渡 |
| 弹窗出现 | 250ms | ease-out | 从中心缩放 |
| AI流式输出 | 28ms/字 | linear | 逐Token输出 |
| 数据刷新 | 500ms | ease-in-out | 数字滚动动画 |
| 资产卡片 | 300ms | ease | 悬停微上浮 |

---

## 七、暗色模式规范

| 元素 | 亮色值 | 暗色值 |
|------|--------|--------|
| 页面背景 | `#F5F5F5` | `#0F0F0F` |
| 卡片背景 | `#FFFFFF` | `#1A1A1A` |
| 主色 | `#D4A017` | `#E8B93E` |
| 标题文字 | `#1A1A1A` | `#F0F0F0` |
| 正文文字 | `#333333` | `#CCCCCC` |
| 次级文字 | `#666666` | `#888888` |
| 分割线 | `#E5E5E5` | `#2A2A2A` |
| AI气泡 | `#F5F5F5` | `#1A1A1A` |
| 用户气泡 | `#D4A017` | `#E8B93E` |
| 代码块 | `#1E1E1E` | `#0A0A0A` |

---

## 八、设计禁忌（Do's and Don'ts）

### Do

- 金融数据使用等宽数字字体，对齐精确
- 涨跌颜色遵循中国股市惯例（红涨绿跌）
- 资产卡片使用金色渐变底，突出财富感
- 风险提示使用醒目的红色标注

### Don't

- 禁止涨跌颜色反转（与国际惯例相反但必须遵循中国市场）
- 禁止金融数据使用比例字体（对齐混乱）
- 禁止风险提示使用与普通文字相同样式
- 禁止金色大面积铺底（视觉疲劳）

---

## 九、CSS变量快速参考

```css
:root {
  --yuanbao-primary: #D4A017;
  --yuanbao-primary-50: #FEF9E7;
  --yuanbao-primary-100: #FDF0C8;
  --yuanbao-primary-200: #FBE49A;
  --yuanbao-primary-300: #F5D26B;
  --yuanbao-primary-400: #E8B93E;
  --yuanbao-primary-500: #D4A017;
  --yuanbao-primary-600: #B8860B;
  --yuanbao-primary-700: #956D09;
  --yuanbao-primary-800: #6B4F06;
  --yuanbao-primary-900: #3D2E03;
  --yuanbao-up: #CF3030;
  --yuanbao-down: #16A34A;
  --yuanbao-warning: #F59E0B;
  --yuanbao-info: #3B82F6;
  --yuanbao-text-title: #1A1A1A;
  --yuanbao-text-body: #333333;
  --yuanbao-text-secondary: #666666;
  --yuanbao-text-placeholder: #999999;
  --yuanbao-border: #E5E5E5;
  --yuanbao-bg-page: #F5F5F5;
  --yuanbao-bg-card: #FFFFFF;
  --yuanbao-spacing-xs: 4px;
  --yuanbao-spacing-sm: 8px;
  --yuanbao-spacing-md: 12px;
  --yuanbao-spacing-lg: 16px;
  --yuanbao-spacing-xl: 24px;
  --yuanbao-spacing-2xl: 32px;
  --yuanbao-spacing-3xl: 48px;
  --yuanbao-radius-sm: 4px;
  --yuanbao-radius-md: 8px;
  --yuanbao-radius-lg: 12px;
  --yuanbao-radius-xl: 16px;
  --yuanbao-radius-full: 9999px;
  --yuanbao-font-family: 'PingFang SC', 'Noto Sans SC', 'Helvetica Neue', sans-serif;
  --yuanbao-font-data: 'DIN Alternate', 'Roboto Mono', monospace;
  --yuanbao-font-mono: 'JetBrains Mono', 'Fira Code', Consolas, monospace;
}
```
