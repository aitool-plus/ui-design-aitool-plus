# 天工（Tiangong）设计规范

> **品牌主色**: `#1E90FF`（天工蓝）| **平台**: Web | **关键词**: 天工蓝/搜索增强/AI助手

---

## 一、设计价值观与原则

1. **搜索增强**：AI+搜索双引擎，回答有据可查、实时联网
2. **天工开物**：以古代科技百科为灵感，界面现代但不失文化底蕴
3. **开放探索**：支持多模型切换，鼓励用户探索AI能力边界
4. **实时可靠**：联网搜索确保信息时效性，来源可追溯

---

## 二、配色体系

### 品牌主色色板（天工蓝 #1E90FF）

| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | `#E6F2FF` | 浅底背景 |
| 100 | `#CCE5FF` | 标签底色 |
| 200 | `#99CCFF` | 图标浅色态 |
| 300 | `#66B3FF` | 辅助强调 |
| 400 | `#3399FF` | 悬停态 |
| 500 | `#1E90FF` | **品牌主色**，主按钮、链接 |
| 600 | `#0077E6` | 按压态 |
| 700 | `#005FB3` | 深色强调 |
| 800 | `#004780` | 暗色模式主色 |
| 900 | `#002E4D` | 极深背景 |

### 功能色

| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | `#10B981` | 搜索完成、操作成功 |
| 警告 | `#F59E0B` | 提示注意 |
| 错误 | `#EF4444` | 搜索失败 |
| 信息 | `#1E90FF` | 与品牌色统一 |

### 中性色

| 名称 | 色值 | 用途 |
|------|------|------|
| 标题 | `#1A202C` | 一级标题 |
| 正文 | `#2D3748` | 正文内容 |
| 次级 | `#718096` | 辅助说明 |
| 占位 | `#A0AEC0` | 占位文字 |
| 分割 | `#E2E8F0` | 分割线 |
| 浅底 | `#F7FAFC` | 页面底色 |
| 卡片 | `#FFFFFF` | 卡片底色 |

### 渐变色

| 名称 | 值 | 用途 |
|------|-----|------|
| 品牌渐变 | `linear-gradient(135deg, #1E90FF, #66B3FF)` | Hero区域 |
| 搜索渐变 | `linear-gradient(90deg, #1E90FF, #10B981)` | 搜索增强指示 |
| 天空渐变 | `linear-gradient(180deg, #E6F2FF, #F7FAFC)` | 内容区背景 |

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
| 主要按钮 | 36px | 8px | `#1E90FF` | `#FFFFFF` | 0 16px |
| 次要按钮 | 36px | 8px | `#E6F2FF` | `#1E90FF` | 0 16px |
| 文字按钮 | 32px | 4px | transparent | `#1E90FF` | 0 8px |

### 卡片

| 类型 | 圆角 | 阴影 | 内边距 | 背景 |
|------|------|------|--------|------|
| 对话卡片 | 12px | none | 16px | `#F7FAFC` |
| 搜索结果卡片 | 8px | `0 1px 3px rgba(0,0,0,0.06)` | 16px | `#FFFFFF` |
| 来源引用卡片 | 8px | none | 12px 16px | `#E6F2FF`，左侧3px #1E90FF |

### 导航栏

- 高度：56px；背景：`#FFFFFF`；底部边框：1px solid `#E2E8F0`
- 左侧Logo，中间搜索框，右侧模型切换+用户

### 弹窗

- 圆角：12px；遮罩：`rgba(0,0,0,0.4)`；背景：`#FFFFFF`

### 输入框

- 高度：40px；圆角：8px；背景：`#FFFFFF`；边框：1px solid `#E2E8F0`
- 聚焦边框：1px solid `#1E90FF`；聚焦阴影：`0 0 0 3px rgba(30,144,255,0.12)`

### AI对话组件

| 组件 | 规格 |
|------|------|
| 用户气泡 | 背景`#1E90FF`，文字`#FFFFFF`，圆角16px 16px 4px 16px，内边距12px 16px |
| AI气泡 | 背景`#F7FAFC`，文字`#2D3748`，圆角16px 16px 16px 4px，内边距12px 16px |
| 搜索来源 | 背景`#E6F2FF`，左侧3px `#1E90FF`，圆角0 8px 8px 0，内边距12px 16px |
| 代码块 | 背景`#1E293B`，文字`#E2E8F0`，圆角8px，字号13px，行高20px，内边距16px |
| Markdown标题 | H1 18px/600，H2 16px/500，H3 14px/500 |
| Markdown代码 | 背景`#E6F2FF`，文字`#0077E6`，圆角4px，内边距2px 6px，字号13px |

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
| 搜索结果加载 | 300ms | ease | 淡入效果 |
| 来源引用展开 | 250ms | ease-out | 高度动画 |

---

## 七、暗色模式规范

| 元素 | 亮色值 | 暗色值 |
|------|--------|--------|
| 页面背景 | `#F7FAFC` | `#0F172A` |
| 卡片背景 | `#FFFFFF` | `#1E293B` |
| 主色 | `#1E90FF` | `#3399FF` |
| 标题文字 | `#1A202C` | `#F1F5F9` |
| 正文文字 | `#2D3748` | `#CBD5E1` |
| 次级文字 | `#718096` | `#94A3B8` |
| 分割线 | `#E2E8F0` | `#334155` |
| AI气泡 | `#F7FAFC` | `#1E293B` |
| 用户气泡 | `#1E90FF` | `#3399FF` |
| 代码块 | `#1E293B` | `#0F172A` |

---

## 八、设计禁忌（Do's and Don'ts）

### Do

- 搜索来源使用左侧竖线+浅蓝底清晰标注
- 联网搜索状态实时可见（搜索中/已搜索/无结果）
- 代码块提供语言标识和复制功能
- 品牌蓝`#1E90FF`作为唯一强调色

### Don't

- 禁止搜索来源无URL和标题标注
- 禁止联网搜索状态无视觉反馈
- 禁止代码块无语法高亮
- 禁止正文使用`#A0AEC0`以下色值

---

## 九、CSS变量快速参考

```css
:root {
  --tiangong-primary: #1E90FF;
  --tiangong-primary-50: #E6F2FF;
  --tiangong-primary-100: #CCE5FF;
  --tiangong-primary-200: #99CCFF;
  --tiangong-primary-300: #66B3FF;
  --tiangong-primary-400: #3399FF;
  --tiangong-primary-500: #1E90FF;
  --tiangong-primary-600: #0077E6;
  --tiangong-primary-700: #005FB3;
  --tiangong-primary-800: #004780;
  --tiangong-primary-900: #002E4D;
  --tiangong-success: #10B981;
  --tiangong-warning: #F59E0B;
  --tiangong-error: #EF4444;
  --tiangong-text-title: #1A202C;
  --tiangong-text-body: #2D3748;
  --tiangong-text-secondary: #718096;
  --tiangong-text-placeholder: #A0AEC0;
  --tiangong-border: #E2E8F0;
  --tiangong-bg-page: #F7FAFC;
  --tiangong-bg-card: #FFFFFF;
  --tiangong-spacing-xs: 4px;
  --tiangong-spacing-sm: 8px;
  --tiangong-spacing-md: 12px;
  --tiangong-spacing-lg: 16px;
  --tiangong-spacing-xl: 24px;
  --tiangong-spacing-2xl: 32px;
  --tiangong-spacing-3xl: 48px;
  --tiangong-radius-sm: 4px;
  --tiangong-radius-md: 8px;
  --tiangong-radius-lg: 12px;
  --tiangong-radius-xl: 16px;
  --tiangong-radius-full: 9999px;
  --tiangong-font-family: 'Noto Sans SC', 'PingFang SC', -apple-system, sans-serif;
  --tiangong-font-mono: 'JetBrains Mono', 'Fira Code', Consolas, monospace;
}
```
