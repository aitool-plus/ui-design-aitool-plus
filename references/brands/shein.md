# SHEIN 设计规范

> 时尚黑·快时尚帝国·全球穿搭 | 主色：#000000

---

## 一、设计价值观与原则

**价值观**：时尚前沿·人人可及·风格无限
**设计原则**：
- 时尚优先：视觉呈现杂志级品质，图片即内容核心
- 极简黑调：黑色为视觉锚点，让商品色彩成为主角
- 快速浏览：瀑布流+无限滚动，降低选择摩擦
- 全球审美：跨文化视觉语言，图标与图片优先于文字

## 二、配色体系

### 品牌主色色板
| 色阶 | 色值 | 用途 |
|------|------|------|------|
| 50 | #F5F5F5 | 主色极浅背景 |
| 100 | #E8E8E8 | 主色浅背景 |
| 200 | #CCCCCC | 主色浅色标签 |
| 300 | #999999 | 主色辅助高亮 |
| 400 | #666666 | 主色悬浮态 |
| 500 | #333333 | 主色深色 |
| 600 | #1A1A1A | 主色按压态 |
| 700 | #0D0D0D | 主色极深 |
| 800 | #050505 | 主色最深 |
| 900 | #000000 | **品牌主色** |

### 功能色
| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | #00B42A | 下单成功、库存确认 |
| 警告 | #FF7D00 | 限时提醒、库存紧张 |
| 错误 | #F53F3F | 下单失败、缺货 |
| 信息 | #000000 | 引导提示（复用主色） |

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
- 主色渐变：`linear-gradient(135deg, #1A1A1A, #4D4D4D)`
- 促销渐变：`linear-gradient(90deg, #000000, #FF2D5B)`

## 三、字体排版体系

### 字体家族
- 中文：`"PingFang SC", "HarmonyOS Sans", "Microsoft YaHei", sans-serif`
- 英文：`"Montserrat", "Helvetica Neue", Arial, sans-serif`
- 数字：`"Montserrat", "DIN Alternate", sans-serif`

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
| Light | 300 | 装饰性大标题 |
| Regular | 400 | 正文、辅助文字 |
| Medium | 500 | 卡片标题、按钮 |
| Bold | 700 | 页面标题、价格 |

## 四、组件设计规范

### 按钮
| 类型 | 高度 | 圆角 | 字号 | 背景色 |
|------|------|------|------|--------|
| 主要按钮 | 44px | 22px | 16px/500 | #000000 |
| 次要按钮 | 40px | 20px | 14px/500 | #F5F5F5 |
| 文字按钮 | — | — | 14px/500 | transparent |
| 标签按钮 | 28px | 14px | 12px/500 | #F5F5F5 |

### 卡片
| 类型 | 圆角 | 阴影 | 内边距 |
|------|------|------|--------|
| 商品卡片 | 8px | 0 2px 8px rgba(0,0,0,0.06) | 8px |
| 促销卡片 | 12px | 0 4px 16px rgba(0,0,0,0.1) | 16px |
| 信息卡片 | 8px | 0 1px 4px rgba(0,0,0,0.04) | 16px |

### 导航栏
- 高度：48px，背景 #FFFFFF
- 标题字号：18px/700，颜色 #1D2129
- 返回图标：24px，颜色 #4E5969

### 弹窗
- 圆角：16px，遮罩 rgba(0,0,0,0.5)
- 标题字号：18px/700，内容 14px/400
- 按钮高度：44px

### 输入框
- 高度：40px，圆角 8px
- 边框：1px solid #E5E6EB，聚焦 #000000
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
| md | 8px | 输入框、卡片 |
| lg | 12px | 大卡片、弹窗 |
| xl | 16px | 大弹窗、底部面板 |
| full | 9999px | 胶囊按钮、头像 |

## 六、动效规范

| 场景 | 时长 | 缓动函数 |
|------|------|----------|
| 按钮反馈 | 150ms | ease-out |
| 页面切换 | 300ms | cubic-bezier(0.25,0.1,0.25,1) |
| 弹窗弹出 | 250ms | cubic-bezier(0.34,1.56,0.64,1) |
| 图片加载 | 200ms | ease-in-out |
| 骨架屏闪烁 | 1.5s | ease-in-out (loop) |

## 七、暗色模式规范

| 元素 | 亮色 | 暗色 |
|------|------|------|
| 页面背景 | #F7F8FA | #0A0A0A |
| 卡片背景 | #FFFFFF | #1A1A1A |
| 主色 | #000000 | #E8E8E8 |
| 标题文字 | #1D2129 | #F5F5F5 |
| 正文文字 | #4E5969 | #C9CDD4 |
| 辅助文字 | #86909C | #6B7785 |
| 边框 | #E5E6EB | #2E2E2E |
| 分割线 | #F2F3F5 | #232323 |

## 八、设计禁忌

- ✅ Do：商品图片占据卡片70%以上面积
- ✅ Do：使用黑色按钮作为CTA，白色文字
- ❌ Don't：禁止在商品卡片上使用大面积彩色背景
- ❌ Don't：禁止使用超过2种字重在单个卡片内
- ❌ Don't：禁止使用圆角超过12px的商品卡片
- ❌ Don't：禁止价格信息使用Light字重

## 九、CSS变量快速参考

```css
:root {
  --shein-primary: #000000;
  --shein-primary-50: #F5F5F5;
  --shein-primary-100: #E8E8E8;
  --shein-primary-200: #CCCCCC;
  --shein-primary-300: #999999;
  --shein-primary-400: #666666;
  --shein-primary-500: #333333;
  --shein-primary-600: #1A1A1A;
  --shein-primary-700: #0D0D0D;
  --shein-primary-800: #050505;
  --shein-primary-900: #000000;
  --shein-success: #00B42A;
  --shein-warning: #FF7D00;
  --shein-error: #F53F3F;
  --shein-text-title: #1D2129;
  --shein-text-body: #4E5969;
  --shein-text-secondary: #86909C;
  --shein-text-placeholder: #C9CDD4;
  --shein-border: #E5E6EB;
  --shein-bg-page: #F7F8FA;
  --shein-bg-card: #FFFFFF;
  --shein-radius-sm: 4px;
  --shein-radius-md: 8px;
  --shein-radius-lg: 12px;
  --shein-radius-xl: 16px;
  --shein-spacing-xs: 4px;
  --shein-spacing-sm: 8px;
  --shein-spacing-md: 12px;
  --shein-spacing-lg: 16px;
  --shein-spacing-xl: 24px;
  --shein-spacing-2xl: 32px;
}
```
