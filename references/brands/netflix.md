# Netflix 设计规范

> 暗红全屏·沉浸观影·原创为王 | 主色：#E50914

---

## 一、设计价值观与原则

**价值观**：暗红全屏·沉浸观影·原创为王
**设计原则**：
- 暗红全屏 沉浸观影 原创为王[0]：核心设计理念贯穿全场景
- 暗红全屏 沉浸观影 原创为王[1]：交互与视觉的统一表达
- 暗红全屏 沉浸观影 原创为王[2]：用户体验的终极目标
- 一致性：跨平台、跨设备视觉统一

## 二、配色体系

### 品牌主色色板
| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | #FCE8E9 | 主色极浅背景 |
| 100 | #F5B8BC | 主色浅背景 |
| 200 | #ED8D93 | 主色浅色标签 |
| 300 | #E5626A | 主色辅助高亮 |
| 400 | #E03340 | 主色悬浮态 |
| 500 | #E50914 | **品牌主色** |
| 600 | #BE0810 | 主色按压态 |
| 700 | #9E070D | 主色深色 |
| 800 | #7E050A | 主色极深 |
| 900 | #5E0408 | 主色最深 |

### 功能色
| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | #00B42A | 操作成功 |
| 警告 | #FF7D00 | 提醒注意 |
| 错误 | #F53F3F | 操作失败 |
| 信息 | #E50914 | 引导提示 |

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
- 主色渐变：`linear-gradient(135deg, #E50914, #E03340)`
- 品牌渐变：`linear-gradient(90deg, #E50914, #00B42A)`

## 三、字体排版体系

### 字体家族
- 中文：`"PingFang SC, Noto Sans SC, sans-serif"`
- 英文：`"Netflix Sans, Helvetica Neue, sans-serif"`
- 代码/数字：`"Roboto Mono, monospace"`

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
| 主要按钮 | 40px | 4px | 14px/500 | #E50914 |
| 次要按钮 | 36px | 4px | 14px/500 | #FCE8E9 |
| 文字按钮 | — | — | 14px/500 | transparent |
| 标签按钮 | 28px | 2px | 12px/500 | #FCE8E9 |

### 卡片
| 类型 | 圆角 | 阴影 | 内边距 |
|------|------|------|--------|
| 内容卡片 | 4px | 0 2px 12px rgba(0,0,0,0.08) | 16px |
| 互动卡片 | 4px | 0 1px 6px rgba(0,0,0,0.06) | 16px |
| 信息卡片 | 2px | 0 1px 4px rgba(0,0,0,0.04) | 16px |

### 导航栏
- 高度：48px，背景 #FFFFFF
- 标题字号：16px/700，颜色 #1D2129
- 侧边栏宽度：240px

### 弹窗
- 圆角：4px，遮罩 rgba(0,0,0,0.4)
- 标题字号：16px/700，内容 14px/400
- 按钮高度：40px

### 输入框
- 高度：36px，圆角 4px
- 边框：1px solid #E5E6EB，聚焦 #E50914
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
| 主色 | #E50914 | #E03340 |
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
  --netflix-primary: #E50914;
  --netflix-primary-50: #FCE8E9;
  --netflix-primary-100: #F5B8BC;
  --netflix-primary-200: #ED8D93;
  --netflix-primary-300: #E5626A;
  --netflix-primary-400: #E03340;
  --netflix-primary-500: #E50914;
  --netflix-primary-600: #BE0810;
  --netflix-primary-700: #9E070D;
  --netflix-primary-800: #7E050A;
  --netflix-primary-900: #5E0408;
  --netflix-success: #00B42A;
  --netflix-warning: #FF7D00;
  --netflix-error: #F53F3F;
  --netflix-text-title: #1D2129;
  --netflix-text-body: #4E5969;
  --netflix-text-secondary: #86909C;
  --netflix-text-placeholder: #C9CDD4;
  --netflix-border: #E5E6EB;
  --netflix-bg-page: #F7F8FA;
  --netflix-bg-card: #FFFFFF;
  --netflix-radius-sm: 4px;
  --netflix-radius-md: 8px;
  --netflix-radius-lg: 12px;
  --netflix-radius-xl: 16px;
  --netflix-spacing-xs: 4px;
  --netflix-spacing-sm: 8px;
  --netflix-spacing-md: 12px;
  --netflix-spacing-lg: 16px;
  --netflix-spacing-xl: 24px;
  --netflix-spacing-2xl: 32px;
}
``

