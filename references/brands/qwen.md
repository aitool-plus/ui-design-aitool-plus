# 通义千问（Qwen）设计规范

> **品牌主色**: `#6236FF`（通义紫）| **平台**: Web | **关键词**: 通义紫/阿里系AI/多模态

---

## 一、设计价值观与原则

1. **万知万能**：多模态能力全覆盖，界面统一承载文本、图像、代码、音频
2. **阿里生态**：融入阿里设计语言，与钉钉、淘宝等体验一致
3. **专业高效**：企业级AI助手，交互精准、响应迅速、结果可靠
4. **多模态融合**：文本与图像、代码无缝切换，一个界面多种能力

---

## 二、配色体系

### 品牌主色色板（通义紫 #6236FF）

| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | `#F3F0FF` | 浅底背景、标记高亮 |
| 100 | `#E0D9FF` | 标签底色 |
| 200 | `#C4B5FF` | 图标浅色态 |
| 300 | `#A78BFA` | 辅助强调 |
| 400 | `#8B5CF6` | 悬停态 |
| 500 | `#6236FF` | **品牌主色**，主按钮、链接 |
| 600 | `#5521E0` | 按压态 |
| 700 | `#451AB5` | 深色强调 |
| 800 | `#321380` | 暗色模式主色 |
| 900 | `#1E0A4D` | 极深背景 |

### 功能色

| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | `#10B981` | 生成完成、操作成功 |
| 警告 | `#F59E0B` | 配额提醒 |
| 错误 | `#EF4444` | 生成失败、参数错误 |
| 信息 | `#6236FF` | 与品牌色统一 |

### 中性色

| 名称 | 色值 | 用途 |
|------|------|------|
| 标题 | `#1F2937` | 一级标题 |
| 正文 | `#374151` | 正文内容 |
| 次级 | `#6B7280` | 辅助说明 |
| 占位 | `#9CA3AF` | 占位文字 |
| 分割 | `#E5E7EB` | 分割线 |
| 浅底 | `#F9FAFB` | 页面底色 |
| 卡片 | `#FFFFFF` | 卡片底色 |

### 渐变色

| 名称 | 值 | 用途 |
|------|-----|------|
| 品牌渐变 | `linear-gradient(135deg, #6236FF, #A78BFA)` | Hero区域、Banner |
| 多模态渐变 | `linear-gradient(90deg, #6236FF, #EC4899, #F59E0B)` | 多模态能力展示 |
| 创意渐变 | `linear-gradient(135deg, #8B5CF6, #6236FF, #3B82F6)` | 图片生成装饰 |

---

## 三、字体排版体系

### 字体家族

- **主字体**: `'Alibaba PuHuiTi', 'Noto Sans SC', 'PingFang SC', sans-serif`
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
| Micro | 11px | 16px | 400 | 标签 |

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
| 主要按钮 | 36px | 8px | `#6236FF` | `#FFFFFF` | 0 16px |
| 次要按钮 | 36px | 8px | `#F3F0FF` | `#6236FF` | 0 16px |
| 文字按钮 | 32px | 4px | transparent | `#6236FF` | 0 8px |
| 能力标签 | 28px | 14px | `#F3F0FF` | `#6236FF` | 0 12px |

### 卡片

| 类型 | 圆角 | 阴影 | 内边距 | 背景 |
|------|------|------|--------|------|
| 对话卡片 | 12px | none | 16px | `#F9FAFB` |
| 能力卡片 | 12px | `0 2px 8px rgba(0,0,0,0.06)` | 20px | `#FFFFFF` |
| 图片生成卡片 | 8px | `0 4px 12px rgba(0,0,0,0.1)` | 0 | `#FFFFFF` |

### 导航栏

- 高度：56px；背景：`#FFFFFF`；底部边框：1px solid `#E5E7EB`
- 左侧Logo+能力切换（对话/图片/代码），中间标题，右侧用户

### 弹窗

- 圆角：12px；遮罩：`rgba(0,0,0,0.4)`；背景：`#FFFFFF`
- 标题区：内边距20px 24px，字号16px，字重500

### 输入框

- 高度：40px；圆角：8px；背景：`#FFFFFF`；边框：1px solid `#E5E7EB`
- 聚焦边框：1px solid `#6236FF`；聚焦阴影：`0 0 0 3px rgba(98,54,255,0.1)`

### AI对话组件

| 组件 | 规格 |
|------|------|
| 用户气泡 | 背景`#6236FF`，文字`#FFFFFF`，圆角16px 16px 4px 16px，内边距12px 16px |
| AI气泡 | 背景`#F9FAFB`，文字`#374151`，圆角16px 16px 16px 4px，内边距12px 16px |
| 代码块 | 背景`#1E293B`，文字`#E2E8F0`，圆角8px，字号13px，行高20px，内边距16px |
| 图片结果 | 圆角8px，最大宽度100%，阴影`0 2px 8px rgba(0,0,0,0.1)` |
| Markdown标题 | H1 18px/600，H2 16px/500，H3 14px/500 |
| Markdown代码 | 背景`#F3F0FF`，文字`#6236FF`，圆角4px，内边距2px 6px，字号13px |

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
| full | 9999px | 头像、药丸标签 |

---

## 六、动效规范

| 场景 | 时长 | 缓动 | 说明 |
|------|------|------|------|
| 按钮悬停 | 150ms | ease | 背景色过渡 |
| 弹窗出现 | 250ms | ease-out | 从中心缩放 |
| AI流式输出 | 28ms/字 | linear | 逐Token输出 |
| 图片生成 | 800ms | ease-in-out | 渐显效果 |
| 能力切换 | 300ms | ease-in-out | 淡入淡出 |
| 代码高亮 | 200ms | ease | 逐行高亮 |

---

## 七、暗色模式规范

| 元素 | 亮色值 | 暗色值 |
|------|--------|--------|
| 页面背景 | `#F9FAFB` | `#0F172A` |
| 卡片背景 | `#FFFFFF` | `#1E293B` |
| 主色 | `#6236FF` | `#8B5CF6` |
| 标题文字 | `#1F2937` | `#F1F5F9` |
| 正文文字 | `#374151` | `#CBD5E1` |
| 次级文字 | `#6B7280` | `#94A3B8` |
| 分割线 | `#E5E7EB` | `#334155` |
| AI气泡 | `#F9FAFB` | `#1E293B` |
| 用户气泡 | `#6236FF` | `#8B5CF6` |
| 代码块 | `#1E293B` | `#0F172A` |

---

## 八、设计禁忌（Do's and Don'ts）

### Do

- 多模态能力使用标签式切换，一目了然
- 图片生成结果使用卡片式展示，支持放大和下载
- 代码块提供运行按钮（接入阿里云函数计算）
- 品牌紫`#6236FF`作为唯一强调色贯穿全站

### Don't

- 禁止多模态能力隐藏在二级菜单
- 禁止图片生成结果无放大预览
- 禁止代码块无语言标识
- 禁止品牌紫与蓝色同时作为主强调色（色彩冲突）

---

## 九、CSS变量快速参考

```css
:root {
  --qwen-primary: #6236FF;
  --qwen-primary-50: #F3F0FF;
  --qwen-primary-100: #E0D9FF;
  --qwen-primary-200: #C4B5FF;
  --qwen-primary-300: #A78BFA;
  --qwen-primary-400: #8B5CF6;
  --qwen-primary-500: #6236FF;
  --qwen-primary-600: #5521E0;
  --qwen-primary-700: #451AB5;
  --qwen-primary-800: #321380;
  --qwen-primary-900: #1E0A4D;
  --qwen-success: #10B981;
  --qwen-warning: #F59E0B;
  --qwen-error: #EF4444;
  --qwen-text-title: #1F2937;
  --qwen-text-body: #374151;
  --qwen-text-secondary: #6B7280;
  --qwen-text-placeholder: #9CA3AF;
  --qwen-border: #E5E7EB;
  --qwen-bg-page: #F9FAFB;
  --qwen-bg-card: #FFFFFF;
  --qwen-spacing-xs: 4px;
  --qwen-spacing-sm: 8px;
  --qwen-spacing-md: 12px;
  --qwen-spacing-lg: 16px;
  --qwen-spacing-xl: 24px;
  --qwen-spacing-2xl: 32px;
  --qwen-spacing-3xl: 48px;
  --qwen-radius-sm: 4px;
  --qwen-radius-md: 8px;
  --qwen-radius-lg: 12px;
  --qwen-radius-xl: 16px;
  --qwen-radius-full: 9999px;
  --qwen-font-family: 'Alibaba PuHuiTi', 'Noto Sans SC', 'PingFang SC', sans-serif;
  --qwen-font-mono: 'JetBrains Mono', 'Fira Code', Consolas, monospace;
}
```
