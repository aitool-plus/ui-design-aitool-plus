# 苏宁 设计规范

> 易购黄·智慧零售·全场景 | 主色：#FFAA00

---

## 一、设计价值观与原则

**价值观**：全场景零售·品质生活·智慧服务
**设计原则**：
- 场景贯通：线上线下视觉一致，购物体验无缝衔接
- 品质信赖：黄色传递温暖与信赖，正品保障始终可见
- 信息清晰：商品参数、服务承诺层级分明
- 家庭友好：温暖色调、大字号、清晰图标

## 二、配色体系

### 品牌主色色板
| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | #FFF8E6 | 主色极浅背景 |
| 100 | #FFEFC2 | 主色浅背景 |
| 200 | #FFE08A | 主色浅色标签 |
| 300 | #FFD04D | 主色辅助高亮 |
| 400 | #FFBA1A | 主色悬浮态 |
| 500 | #FFAA00 | **品牌主色** |
| 600 | #E09500 | 主色按压态 |
| 700 | #B87800 | 主色深色 |
| 800 | #8F5C00 | 主色极深 |
| 900 | #6B4500 | 主色最深 |

### 功能色
| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | #00B42A | 下单成功、配送完成 |
| 警告 | #FF7D00 | 库存紧张、限时提醒 |
| 错误 | #F53F3F | 下单失败、支付异常 |
| 信息 | #FFAA00 | 引导提示（复用主色） |

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
- 主色渐变：`linear-gradient(135deg, #FFAA00, #FFD04D)`
- 促销渐变：`linear-gradient(90deg, #FFAA00, #FF6A00)`

## 三、字体排版体系

### 字体家族
- 中文：`"PingFang SC", "HarmonyOS Sans", "Microsoft YaHei", sans-serif`
- 英文：`"Roboto", "Helvetica Neue", Arial, sans-serif`
- 数字：`"Roboto", "DIN Alternate", sans-serif`

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
| Bold | 700 | 页面标题、价格 |

## 四、组件设计规范

### 按钮
| 类型 | 高度 | 圆角 | 字号 | 背景色 |
|------|
| 主要按钮 | 44px | 22px | 16px/500 | #FFAA00 |
| 次要按钮 | 40px | 20px | 14px/500 | #FFF8E6 |
| 文字按钮 | — | — | 14px/500 | transparent |
| 标签按钮 | 28px | 14px | 12px/500 | #FFF8E6 |

### 卡片
| 类型 | 圆角 | 阴影 | 内边距 |
|------|------|------|--------|
| 商品卡片 | 12px | 0 2px 12px rgba(0,0,0,0.08) | 12px |
| 促销卡片 | 16px | 0 4px 16px rgba(255,170,0,0.12) | 16px |
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
- 边框：1px solid #E5E6EB，聚焦 #FFAA00
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
| md | 8px | 输入框、小卡片 |
| lg | 12px | 卡片、弹窗 |
| xl | 16px | 大弹窗、底部面板 |
| full | 9999px | 胶囊按钮、头像 |

## 六、动效规范

| 场景 | 时长 | 缓动函数 |
|------|------|----------|
| 按钮反馈 | 150ms | ease-out |
| 页面切换 | 300ms | cubic-bezier(0.25,0.1,0.25,1) |
| 弹窗弹出 | 250ms | cubic-bezier(0.34,1.56,0.64,1) |
| 列表加载 | 200ms | ease-in-out |
| 骨架屏闪烁 | 1.5s | ease-in-out (loop) |

## 七、暗色模式规范

| 元素 | 亮色 | 暗色 |
|------|------|------|
| 页面背景 | #F7F8FA | #0D0D0D |
| 卡片背景 | #FFFFFF | #1A1A1A |
| 主色 | #FFAA00 | #FFD04D |
| 标题文字 | #1D2129 | #F5F5F5 |
| 正文文字 | #4E5969 | #C9CDD4 |
| 辅助文字 | #86909C | #6B7785 |
| 边框 | #E5E6EB | #2E2E2E |
| 分割线 | #F2F3F5 | #232323 |

## 八、设计禁忌

- ✅ Do：主色按钮文字使用深色（#1D2129）确保对比度
- ✅ Do：服务保障标签使用主色浅底+深色文字
- ❌ Don't：禁止主色按钮使用白色文字（黄色底白字对比度不足）
- ❌ Don't：禁止大面积使用主色作为页面背景
- ❌ Don't：禁止商品卡片缺少服务保障标识
- ❌ Don't：禁止使用纯黄色文字在白色背景上

## 九、CSS变量快速参考

```css
:root {
  --suning-primary: #FFAA00;
  --suning-primary-50: #FFF8E6;
  --suning-primary-100: #FFEFC2;
  --suning-primary-200: #FFE08A;
  --suning-primary-300: #FFD04D;
  --suning-primary-400: #FFBA1A;
  --suning-primary-500: #FFAA00;
  --suning-primary-600: #E09500;
  --suning-primary-700: #B87800;
  --suning-primary-800: #8F5C00;
  --suning-primary-900: #6B4500;
  --suning-success: #00B42A;
  --suning-warning: #FF7D00;
  --suning-error: #F53F3F;
  --suning-text-title: #1D2129;
  --suning-text-body: #4E5969;
  --suning-text-secondary: #86909C;
  --suning-text-placeholder: #C9CDD4;
  --suning-border: #E5E6EB;
  --suning-bg-page: #F7F8FA;
  --suning-bg-card: #FFFFFF;
  --suning-radius-sm: 4px;
  --suning-radius-md: 8px;
  --suning-radius-lg: 12px;
  --suning-radius-xl: 16px;
  --suning-spacing-xs: 4px;
  --suning-spacing-sm: 8px;
  --suning-spacing-md: 12px;
  --suning-spacing-lg: 16px;
  --suning-spacing-xl: 24px;
  --suning-spacing-2xl: 32px;
}
```
