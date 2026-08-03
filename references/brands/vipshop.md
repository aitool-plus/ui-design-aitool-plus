# 唯品会 设计规范

> 特卖粉·品牌特卖·正品折扣 | 主色：#FF2D5B

---

## 一、设计价值观与原则

**价值观**：品牌信赖·限时特卖·品质生活
**设计原则**：
- 特卖氛围：倒计时、限时标签营造紧迫感
- 品牌信任：品牌Logo始终醒目，正品标识不可省略
- 折扣清晰：原价划线+折扣价，价格对比一目了然
- 女性友好：圆润造型、柔和渐变、温暖色调

## 二、配色体系

### 品牌主色色板
| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | #FFF0F3 | 主色极浅背景 |
| 100 | #FFD9E2 | 主色浅背景 |
| 200 | #FFB3C4 | 主色浅色标签 |
| 300 | #FF8DA6 | 主色辅助高亮 |
| 400 | #FF5C7E | 主色悬浮态 |
| 500 | #FF2D5B | **品牌主色** |
| 600 | #E0194A | 主色按压态 |
| 700 | #B8123C | 主色深色 |
| 800 | #900C2E | 主色极深 |
| 900 | #6B0822 | 主色最深 |

### 功能色
| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | #00B42A | 下单成功、到货通知 |
| 警告 | #FF7D00 | 限时即将结束 |
| 错误 | #F53F3F | 下单失败、支付异常 |
| 信息 | #FF2D5B | 引导提示（复用主色） |

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
- 主色渐变：`linear-gradient(135deg, #FF2D5B, #FF5C7E)`
- 促销渐变：`linear-gradient(90deg, #FF2D5B, #FF8DA6)`

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
| Bold | 700 | 页面标题、折扣价 |

## 四、组件设计规范

### 按钮
| 类型 | 高度 | 圆角 | 字号 | 背景色 |
|------|------|------|------|--------|
| 主要按钮 | 44px | 22px | 16px/500 | #FF2D5B |
| 次要按钮 | 40px | 20px | 14px/500 | #FFF0F3 |
| 文字按钮 | — | — | 14px/500 | transparent |
| 标签按钮 | 28px | 14px | 12px/500 | #FFF0F3 |

### 卡片
| 类型 | 圆角 | 阴影 | 内边距 |
|------|------|------|--------|
| 商品卡片 | 12px | 0 2px 12px rgba(0,0,0,0.08) | 12px |
| 促销卡片 | 16px | 0 4px 16px rgba(255,45,91,0.12) | 16px |
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
- 边框：1px solid #E5E6EB，聚焦 #FF2D5B
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
| 弹窗弹出 | 250ms | cubic-bezier(0.34,1.56,0.64,0.64,1) |
| 倒计时闪烁 | 500ms | ease-in-out (loop) |
| 骨架屏闪烁 | 1.5s | ease-in-out (loop) |

## 七、暗色模式规范

| 元素 | 亮色 | 暗色 |
|------|------|------|
| 页面背景 | #F7F8FA | #0D0D0D |
| 卡片背景 | #FFFFFF | #1A1A1A |
| 主色 | #FF2D5B | #FF5C7E |
| 标题文字 | #1D2129 | #F5F5F5 |
| 正文文字 | #4E5969 | #C9CDD4 |
| 辅助文字 | #86909C | #6B7785 |
| 边框 | #E5E6EB | #2E2E2E |
| 分割线 | #F2F3F5 | #232323 |

## 八、设计禁忌

- ✅ Do：折扣价使用主色Bold，原价使用灰色删除线
- ✅ Do：限时标签使用主色渐变背景
- ❌ Don't：禁止折扣价使用灰色或低对比度色
- ❌ Don't：禁止倒计时组件字号小于14px
- ❌ Don't：禁止品牌卡片缺少正品标识
- ❌ Don't：禁止使用直角（0圆角）按钮

## 九、CSS变量快速参考

```css
:root {
  --vipshop-primary: #FF2D5B;
  --vipshop-primary-50: #FFF0F3;
  --vipshop-primary-100: #FFD9E2;
  --vipshop-primary-200: #FFB3C4;
  --vipshop-primary-300: #FF8DA6;
  --vipshop-primary-400: #FF5C7E;
  --vipshop-primary-500: #FF2D5B;
  --vipshop-primary-600: #E0194A;
  --vipshop-primary-700: #B8123C;
  --vipshop-primary-800: #900C2E;
  --vipshop-primary-900: #6B0822;
  --vipshop-success: #00B42A;
  --vipshop-warning: #FF7D00;
  --vipshop-error: #F53F3F;
  --vipshop-text-title: #1D2129;
  --vipshop-text-body: #4E5969;
  --vipshop-text-secondary: #86909C;
  --vipshop-text-placeholder: #C9CDD4;
  --vipshop-border: #E5E6EB;
  --vipshop-bg-page: #F7F8FA;
  --vipshop-bg-card: #FFFFFF;
  --vipshop-radius-sm: 4px;
  --vipshop-radius-md: 8px;
  --vipshop-radius-lg: 12px;
  --vipshop-radius-xl: 16px;
  --vipshop-spacing-xs: 4px;
  --vipshop-spacing-sm: 8px;
  --vipshop-spacing-md: 12px;
  --vipshop-spacing-lg: 16px;
  --vipshop-spacing-xl: 24px;
  --vipshop-spacing-2xl: 32px;
}
```
