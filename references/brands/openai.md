# OpenAI 设计规范

> 学术极简·渐变紫光·智能对话 | 主色：#412991

---

## 一、设计价值观与原则

**价值观**：学术极简·渐变紫光·智能对话
**设计原则**：
- 学术极简 渐变紫光 智能对话[0]：核心设计理念贯穿全场景
- 学术极简 渐变紫光 智能对话[1]：交互与视觉的统一表达
- 学术极简 渐变紫光 智能对话[2]：用户体验的终极目标
- 一致性：跨平台、跨设备视觉统一

## 二、配色体系

### 品牌主色色板
| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | #EDE8F7 | 主色极浅背景 |
| 100 | #CFC0E8 | 主色浅背景 |
| 200 | #B098D9 | 主色浅色标签 |
| 300 | #9170CA | 主色辅助高亮 |
| 400 | #6A4DB8 | 主色悬浮态 |
| 500 | #412991 | **品牌主色** |
| 600 | #362278 | 主色按压态 |
| 700 | #2B1A60 | 主色深色 |
| 800 | #1F1248 | 主色极深 |
| 900 | #140A30 | 主色最深 |

### 功能色
| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | #00B42A | 操作成功 |
| 警告 | #FF7D00 | 提醒注意 |
| 错误 | #F53F3F | 操作失败 |
| 信息 | #412991 | 引导提示 |

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
- 主色渐变：`linear-gradient(135deg, #412991, #6A4DB8)`
- 品牌渐变：`linear-gradient(90deg, #412991, #00B42A)`

## 三、字体排版体系

### 字体家族
- 中文：`"PingFang SC, HarmonyOS Sans, sans-serif"`
- 英文：`"Inter, sans-serif"`
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
| 主要按钮 | 40px | 12px | 14px/500 | #412991 |
| 次要按钮 | 36px | 12px | 14px/500 | #EDE8F7 |
| 文字按钮 | — | — | 14px/500 | transparent |
| 标签按钮 | 28px | 6px | 12px/500 | #EDE8F7 |

### 卡片
| 类型 | 圆角 | 阴影 | 内边距 |
|------|------|------|--------|
| 内容卡片 | 12px | 0 2px 12px rgba(0,0,0,0.08) | 16px |
| 互动卡片 | 12px | 0 1px 6px rgba(0,0,0,0.06) | 16px |
| 信息卡片 | 6px | 0 1px 4px rgba(0,0,0,0.04) | 16px |

### 导航栏
- 高度：48px，背景 #FFFFFF
- 标题字号：16px/700，颜色 #1D2129
- 侧边栏宽度：240px

### 弹窗
- 圆角：12px，遮罩 rgba(0,0,0,0.4)
- 标题字号：16px/700，内容 14px/400
- 按钮高度：40px

### 输入框
- 高度：36px，圆角 12px
- 边框：1px solid #E5E6EB，聚焦 #412991
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
| 主色 | #412991 | #6A4DB8 |
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
  --openai-primary: #412991;
  --openai-primary-50: #EDE8F7;
  --openai-primary-100: #CFC0E8;
  --openai-primary-200: #B098D9;
  --openai-primary-300: #9170CA;
  --openai-primary-400: #6A4DB8;
  --openai-primary-500: #412991;
  --openai-primary-600: #362278;
  --openai-primary-700: #2B1A60;
  --openai-primary-800: #1F1248;
  --openai-primary-900: #140A30;
  --openai-success: #00B42A;
  --openai-warning: #FF7D00;
  --openai-error: #F53F3F;
  --openai-text-title: #1D2129;
  --openai-text-body: #4E5969;
  --openai-text-secondary: #86909C;
  --openai-text-placeholder: #C9CDD4;
  --openai-border: #E5E6EB;
  --openai-bg-page: #F7F8FA;
  --openai-bg-card: #FFFFFF;
  --openai-radius-sm: 4px;
  --openai-radius-md: 8px;
  --openai-radius-lg: 12px;
  --openai-radius-xl: 16px;
  --openai-spacing-xs: 4px;
  --openai-spacing-sm: 8px;
  --openai-spacing-md: 12px;
  --openai-spacing-lg: 16px;
  --openai-spacing-xl: 24px;
  --openai-spacing-2xl: 32px;
}
``

