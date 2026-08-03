# 科大讯飞（iFlytek）设计规范

> **品牌主色**: `#005BAC`（语音蓝）| **平台**: Web | **关键词**: 语音蓝/AI语音/智能交互

---

## 一、设计价值观与原则

1. **语音优先**：语音交互为核心入口，界面为语音服务而非替代
2. **听见未来**：AI语音技术让沟通无障碍，界面包容多场景多人群
3. **专业可靠**：教育、医疗、司法等专业场景，界面严谨规范
4. **智能交互**：语音+文字+图像多模态融合，自然交互

---

## 二、配色体系

### 品牌主色色板（语音蓝 #005BAC）

| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | `#E6F0FA` | 浅底背景 |
| 100 | `#CCE1F5` | 标签底色 |
| 200 | `#99C3EB` | 图标浅色态 |
| 300 | `#66A5E0` | 辅助强调 |
| 400 | `#3387D6` | 悬停态 |
| 500 | `#005BAC` | **品牌主色**，主按钮、链接 |
| 600 | `#004C91` | 按压态 |
| 700 | `#003D76` | 深色强调 |
| 800 | `#002E5B` | 暗色模式主色 |
| 900 | `#001F40` | 极深背景 |

### 功能色

| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | `#10B981` | 识别成功、操作完成 |
| 警告 | `#F59E0B` | 降噪提示 |
| 错误 | `#EF4444` | 识别失败 |
| 信息 | `#005BAC` | 与品牌色统一 |
| 录音 | `#EF4444` | 录音中脉冲指示 |

### 中性色

| 名称 | 色值 | 用途 |
|------|------|------|
| 标题 | `#1A2332` | 一级标题 |
| 正文 | `#374151` | 正文内容 |
| 次级 | `#6B7280` | 辅助说明 |
| 占位 | `#9CA3AF` | 占位文字 |
| 分割 | `#E5E7EB` | 分割线 |
| 浅底 | `#F5F7FA` | 页面底色 |
| 卡片 | `#FFFFFF` | 卡片底色 |

### 渐变色

| 名称 | 值 | 用途 |
|------|-----|------|
| 品牌渐变 | `linear-gradient(135deg, #005BAC, #3387D6)` | Hero区域 |
| 声波渐变 | `linear-gradient(90deg, #005BAC, #10B981)` | 语音波形装饰 |
| 录音脉冲 | `radial-gradient(circle, #EF4444, transparent)` | 录音按钮脉冲 |

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
| 主要按钮 | 36px | 8px | `#005BAC` | `#FFFFFF` | 0 16px |
| 次要按钮 | 36px | 8px | `#E6F0FA` | `#005BAC` | 0 16px |
| 录音按钮 | 56px | 28px | `#EF4444` | `#FFFFFF` | 0，脉冲动画 |
| 文字按钮 | 32px | 4px | transparent | `#005BAC` | 0 8px |

### 卡片

| 类型 | 圆角 | 阴影 | 内边距 | 背景 |
|------|------|------|--------|------|
| 对话卡片 | 12px | none | 16px | `#F5F7FA` |
| 识别结果卡片 | 12px | `0 2px 8px rgba(0,0,0,0.06)` | 20px | `#FFFFFF` |
| 语音波形卡片 | 8px | none | 16px | `#E6F0FA` |

### 导航栏

- 高度：56px；背景：`#FFFFFF`；底部边框：1px solid `#E5E7EB`
- 左侧Logo，中间功能切换，右侧录音入口+用户

### 弹窗

- 圆角：12px；遮罩：`rgba(0,0,0,0.4)`；背景：`#FFFFFF`

### 输入框

- 高度：40px；圆角：8px；背景：`#FFFFFF`；边框：1px solid `#E5E7EB`
- 聚焦边框：1px solid `#005BAC`；聚焦阴影：`0 0 0 3px rgba(0,91,172,0.12)`

### AI对话组件

| 组件 | 规格 |
|------|------|
| 用户气泡 | 背景`#005BAC`，文字`#FFFFFF`，圆角16px 16px 4px 16px，内边距12px 16px |
| AI气泡 | 背景`#F5F7FA`，文字`#374151`，圆角16px 16px 16px 4px，内边距12px 16px |
| 语音转写 | 背景`#E6F0FA`，左侧3px `#005BAC`，圆角0 8px 8px 0，内边距12px 16px |
| 代码块 | 背景`#1E293B`，文字`#E2E8F0`，圆角8px，字号13px，行高20px，内边距16px |
| Markdown标题 | H1 18px/600，H2 16px/500，H3 14px/500 |
| Markdown代码 | 背景`#E6F0FA`，文字`#004C91`，圆角4px，内边距2px 6px，字号13px |

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
| full | 9999px | 头像、录音按钮 |

---

## 六、动效规范

| 场景 | 时长 | 缓动 | 说明 |
|------|------|------|------|
| 按钮悬停 | 150ms | ease | 背景色过渡 |
| 弹窗出现 | 250ms | ease-out | 从中心缩放 |
| AI流式输出 | 28ms/字 | linear | 逐Token输出 |
| 录音脉冲 | 1500ms | ease-in-out | 无限循环脉冲 |
| 语音波形 | 100ms | linear | 实时波形更新 |
| 识别结果 | 300ms | ease | 逐段淡入 |

---

## 七、暗色模式规范

| 元素 | 亮色值 | 暗色值 |
|------|--------|--------|
| 页面背景 | `#F5F7FA` | `#0A1628` |
| 卡片背景 | `#FFFFFF` | `#1A2332` |
| 主色 | `#005BAC` | `#3387D6` |
| 标题文字 | `#1A2332` | `#F1F5F9` |
| 正文文字 | `#374151` | `#CBD5E1` |
| 次级文字 | `#6B7280` | `#94A3B8` |
| 分割线 | `#E5E7EB` | `#2A3A4E` |
| AI气泡 | `#F5F7FA` | `#1A2332` |
| 用户气泡 | `#005BAC` | `#3387D6` |
| 代码块 | `#1E293B` | `#0A1628` |

---

## 八、设计禁忌（Do's and Don'ts）

### Do

- 录音按钮使用脉冲动画明确录音状态
- 语音转写结果实时展示，逐段淡入
- 语音波形可视化，增强交互反馈
- 品牌蓝`#005BAC`作为唯一强调色

### Don't

- 禁止录音状态无视觉反馈（用户不知是否在录音）
- 禁止语音转写结果一次性全部展示（体验突兀）
- 禁止录音按钮过小（触控不便）
- 禁止语音波形静态无动画（缺乏活力）

---

## 九、CSS变量快速参考

```css
:root {
  --iflytek-primary: #005BAC;
  --iflytek-primary-50: #E6F0FA;
  --iflytek-primary-100: #CCE1F5;
  --iflytek-primary-200: #99C3EB;
  --iflytek-primary-300: #66A5E0;
  --iflytek-primary-400: #3387D6;
  --iflytek-primary-500: #005BAC;
  --iflytek-primary-600: #004C91;
  --iflytek-primary-700: #003D76;
  --iflytek-primary-800: #002E5B;
  --iflytek-primary-900: #001F40;
  --iflytek-success: #10B981;
  --iflytek-warning: #F59E0B;
  --iflytek-error: #EF4444;
  --iflytek-recording: #EF4444;
  --iflytek-text-title: #1A2332;
  --iflytek-text-body: #374151;
  --iflytek-text-secondary: #6B7280;
  --iflytek-text-placeholder: #9CA3AF;
  --iflytek-border: #E5E7EB;
  --iflytek-bg-page: #F5F7FA;
  --iflytek-bg-card: #FFFFFF;
  --iflytek-spacing-xs: 4px;
  --iflytek-spacing-sm: 8px;
  --iflytek-spacing-md: 12px;
  --iflytek-spacing-lg: 16px;
  --iflytek-spacing-xl: 24px;
  --iflytek-spacing-2xl: 32px;
  --iflytek-spacing-3xl: 48px;
  --iflytek-radius-sm: 4px;
  --iflytek-radius-md: 8px;
  --iflytek-radius-lg: 12px;
  --iflytek-radius-xl: 16px;
  --iflytek-radius-full: 9999px;
  --iflytek-font-family: 'Noto Sans SC', 'PingFang SC', -apple-system, sans-serif;
  --iflytek-font-mono: 'JetBrains Mono', 'Fira Code', Consolas, monospace;
}
```
