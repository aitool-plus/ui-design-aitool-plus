# Stripe 设计规范

> 紫色优雅·金融数据·weight-300 | 主色：#635BFF

---

## 一、设计价值观与原则

**价值观**：紫色优雅·金融数据·weight-300
**设计原则**：
- 紫色优雅 金融数据 轻量排版[0]：核心设计理念贯穿全场景
- 紫色优雅 金融数据 轻量排版[1]：交互与视觉的统一表达
- 紫色优雅 金融数据 轻量排版[2]：用户体验的终极目标
- 一致性：跨平台、跨设备视觉统一

## 二、配色体系

### 品牌主色色板
| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | #EFEDFF | 主色极浅背景 |
| 100 | #D4CFFF | 主色浅背景 |
| 200 | #B8AEFF | 主色浅色标签 |
| 300 | #9B8EFF | 主色辅助高亮 |
| 400 | #7C6EFF | 主色悬浮态 |
| 500 | #635BFF | **品牌主色** |
| 600 | #5147D9 | 主色按压态 |
| 700 | #4038B3 | 主色深色 |
| 800 | #302A8C | 主色极深 |
| 900 | #201C66 | 主色最深 |

### 功能色
| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | #00B42A | 操作成功 |
| 警告 | #FF7D00 | 提醒注意 |
| 错误 | #F53F3F | 操作失败 |
| 信息 | #635BFF | 引导提示 |

### 中性色
| 色阶 | 色值 | 用途 |
|------|------|------|
| 标题 | #1D2129 | 主标题文字 |
| 正文 | #4E5969 | 正文内容 |
| 辅助 | #86909C | 辅助说明 |
| 占位 | #C9CDD4 | 占位文字 |
| 边框 | #E5E6EB | 分割线 |
| 背景 | #F7F8FA | 页面底色 |

### 渐变色
- 主色渐变：`linear-gradient(135deg, #635BFF, #7C6EFF)`
- 品牌渐变：`linear-gradient(90deg, #635BFF, #00B42A)`

## 三、字体排版体系

### 字体家族
- 中文：`"PingFang SC, Noto Sans SC, sans-serif"`
- 英文：`"Inter, -apple-system, sans-serif"`
- 代码/数字：`"JetBrains Mono, monospace"`

### 字号阶梯
| 用途 | 字号 | 行高 |
|------|------|------|
| 大标题 | 28px | 36px |
| 页面标题 | 22px | 30px |
| 模块标题 | 18px | 26px |
| 卡片标题 | 16px | 24px |
| 正文 | 14px | 22px |
| 辅助文字 | 12px | 20px |
| 标签 | 10px | 16px |

### 字重体系
| 字重 | 数值 | 用途 |
|------|------|------|
| Regular | 400 | 正文、辅助文字 |
| Medium | 500 | 卡片标题、按钮 |
| Bold | 700 | 页面标题、强调 |

## 四、组件设计规范

### 按钮
| 类型 | 高度 | 圆角 | 字号 | 背景色 |
|------|------|------|------|--------|
| 主要按钮 | 40px | 8px | 14px/500 | #635BFF |
| 次要按钮 | 36px | 8px | 14px/500 | #EFEDFF |
| 文字按钮 | — | — | 14px/500 | transparent |
| 标签按钮 | 28px | 4px | 12px/500 | #EFEDFF |

### 卡片
| 类型 | 圆角 | 阴影 | 内边距 |
|------|------|------|--------|
| 内容卡片 | 8px | 0 2px 12px rgba(0,0,0,0.08) | 16px |
| 互动卡片 | 8px | 0 1px 6px rgba(0,0,0,0.06) | 16px |
| 信息卡片 | 4px | 0 1px 4px rgba(0,0,0,0.04) | 16px |

### 导航栏
- 高度：48px，背景 #FFFFFF
- 标题字号：16px/700，颜色 #1D2129
- 侧边栏宽度：240px

### 弹窗
- 圆角：8px，遮罩 rgba(0,0,0,0.4)
- 标题字号：16px/700，内容 14px/400
- 按钮高度：40px

### 输入框
- 高度：36px，圆角 8px
- 边框：1px solid #E5E6EB，聚焦 #635BFF
- 字号：14px，占位色 #C9CDD4

## 五、间距与圆角体系

### 间距阶梯（4px基准）
| Token | 值 | 用途 |
|-------|-----|------|
| xs | 4px | 图标与文字间距 |
| sm | 8px | 紧凑元素间距 |
| md | 12px | 卡片内边距 |
| lg | 16px | 模块间距 |
| xl | 24px | 区块间距 |
| 2xl | 32px | 页面边距 |

### 圆角阶梯
| Token | 值 | 用途 |
|-------|-----|------|
| sm | 4px | 标签、小元素 |
| md | 8px | 输入框、按钮 |
| lg | 12px | 卡片、弹窗 |
| xl | 16px | 大弹窗 |
| full | 9999px | 胶囊按钮、头像 |

## 六、动效规范

| 场景 | 时长 | 缓动函数 |
|------|------|----------|
| 按钮反馈 | 120ms | ease-out |
| 页面切换 | 200ms | cubic-bezier(0.25,0.1,0.25,1) |
| 弹窗弹出 | 200ms | cubic-bezier(0.34,1.56,0.64,1) |
| 列表加载 | 200ms | ease-in-out |
| 骨架屏闪烁 | 1.5s | ease-in-out (loop) |

## 七、暗色模式规范

| 元素 | 亮色 | 暗色 |
|------|------|------|
| 页面背景 | #F7F8FA | #0D0D0D |
| 卡片背景 | #FFFFFF | #1A1A1A |
| 主色 | #635BFF | #9B8EFF |
| 标题文字 | #1D2129 | #F5F5F5 |
| 正文文字 | #4E5969 | #C9CDD4 |
| 辅助文字 | #86909C | #6B7785 |
| 边框 | #E5E6EB | #2E2E2E |
| 分割线 | #F2F3F5 | #232323 |

## 八、设计禁忌

- ✅ Do：核心交互使用主色，保持视觉一致性
- ✅ Do：圆角统一使用设计系统规范
- ❌ Don't：禁止核心操作使用灰色或低对比度
- ❌ Don't：禁止圆角数值不统一
- ❌ Don't：禁止使用与品牌调性冲突的配色
- ❌ Don't：禁止动效时长超过300ms

## 九、CSS变量快速参考

``css
:root {
  --stripe-primary: #635BFF;
  --stripe-primary-50: #EFEDFF;
  --stripe-primary-100: #D4CFFF;
  --stripe-primary-200: #B8AEFF;
  --stripe-primary-300: #9B8EFF;
  --stripe-primary-400: #7C6EFF;
  --stripe-primary-500: #635BFF;
  --stripe-primary-600: #5147D9;
  --stripe-primary-700: #4038B3;
  --stripe-primary-800: #302A8C;
  --stripe-primary-900: #201C66;
  --stripe-success: #00B42A;
  --stripe-warning: #FF7D00;
  --stripe-error: #F53F3F;
  --stripe-text-title: #1D2129;
  --stripe-text-body: #4E5969;
  --stripe-text-secondary: #86909C;
  --stripe-text-placeholder: #C9CDD4;
  --stripe-border: #E5E6EB;
  --stripe-bg-page: #F7F8FA;
  --stripe-bg-card: #FFFFFF;
  --stripe-radius-sm: 4px;
  --stripe-radius-md: 8px;
  --stripe-radius-lg: 12px;
  --stripe-radius-xl: 16px;
  --stripe-spacing-xs: 4px;
  --stripe-spacing-sm: 8px;
  --stripe-spacing-md: 12px;
  --stripe-spacing-lg: 16px;
  --stripe-spacing-xl: 24px;
  --stripe-spacing-2xl: 32px;
}
``

