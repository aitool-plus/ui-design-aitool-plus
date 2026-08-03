# 饿了么 设计规范

> 饿了蓝·美食到家·即时配送 | 主色：#0097FF

---

## 一、设计价值观与原则

**价值观**：美食即达·生活便利·即时满足
**设计原则**：
- 美食优先：食物图片为视觉核心，色彩饱满诱人
- 即时感知：配送时间、距离信息始终可见
- 蓝色信任：蓝色传递可靠与速度，配送过程可视化
- 简洁下单：3步完成点餐，减少决策负担

## 二、配色体系

### 品牌主色色板
| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | #E6F4FF | 主色极浅背景 |
| 100 | #BAE0FF | 主色浅背景 |
| 200 | #82C4FF | 主色浅色标签 |
| 300 | #4DA6FF | 主色辅助高亮 |
| 400 | #1A8CFF | 主色悬浮态 |
| 500 | #0097FF | **品牌主色** |
| 600 | #0080E0 | 主色按压态 |
| 700 | #0066B8 | 主色深色 |
| 800 | #004D8F | 主色极深 |
| 900 | #003A6B | 主色最深 |

### 功能色
| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | #00B42A | 下单成功、配送到达 |
| 警告 | #FF7D00 | 高峰提醒、配送延迟 |
| 错误 | #F53F3F | 下单失败、商家休息 |
| 信息 | #0097FF | 引导提示（复用主色） |

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
- 主色渐变：`linear-gradient(135deg, #0097FF, #4DA6FF)`
- 促销渐变：`linear-gradient(90deg, #0097FF, #00D4FF)`

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
|------|------|------|------|--------|
| 主要按钮 | 44px | 22px | 16px/500 | #0097FF |
| 次要按钮 | 40px | 20px | 14px/500 | #E6F4FF |
| 文字按钮 | — | — | 14px/500 | transparent |
| 标签按钮 | 28px | 14px | 12px/500 | #E6F4FF |

### 卡片
| 类型 | 圆角 | 阴影 | 内边距 |
|------|------|------|--------|
| 商家卡片 | 12px | 0 2px 12px rgba(0,0,0,0.08) | 12px |
| 菜品卡片 | 8px | 0 1px 6px rgba(0,0,0,0.06) | 8px |
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
- 边框：1px solid #E5E6EB，聚焦 #0097FF
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
| 配送动画 | 2000ms | linear (loop) |
| 骨架屏闪烁 | 1.5s | ease-in-out (loop) |

## 七、暗色模式规范

| 元素 | 亮色 | 暗色 |
|------|------|------|
| 页面背景 | #F7F8FA | #0D0D0D |
| 卡片背景 | #FFFFFF | #1A1A1A |
| 主色 | #0097FF | #4DA6FF |
| 标题文字 | #1D2129 | #F5F5F5 |
| 正文文字 | #4E5969 | #C9CDD4 |
| 辅助文字 | #86909C | #6B7785 |
| 边框 | #E5E6EB | #2E2E2E |
| 分割线 | #F2F3F5 | #232323 |

## 八、设计禁忌

- ✅ Do：配送时间使用Bold字重，字号≥16px
- ✅ Do：食物图片使用圆角8-12px，保持诱人感
- ❌ Don't：禁止配送信息使用灰色或小字号
- ❌ Don't：禁止商家卡片缺少配送时间/距离
- ❌ Don't：禁止使用红色作为主CTA颜色（与蓝色冲突）
- ❌ Don't：禁止菜品图片使用直角裁切

## 九、CSS变量快速参考

```css
:root {
  --eleme-primary: #0097FF;
  --eleme-primary-50: #E6F4FF;
  --eleme-primary-100: #BAE0FF;
  --eleme-primary-200: #82C4FF;
  --eleme-primary-300: #4DA6FF;
  --eleme-primary-400: #1A8CFF;
  --eleme-primary-500: #0097FF;
  --eleme-primary-600: #0080E0;
  --eleme-primary-700: #0066B8;
  --eleme-primary-800: #004D8F;
  --eleme-primary-900: #003A6B;
  --eleme-success: #00B42A;
  --eleme-warning: #FF7D00;
  --eleme-error: #F53F3F;
  --eleme-text-title: #1D2129;
  --eleme-text-body: #4E5969;
  --eleme-text-secondary: #86909C;
  --eleme-text-placeholder: #C9CDD4;
  --eleme-border: #E5E6EB;
  --eleme-bg-page: #F7F8FA;
  --eleme-bg-card: #FFFFFF;
  --eleme-radius-sm: 4px;
  --eleme-radius-md: 8px;
  --eleme-radius-lg: 12px;
  --eleme-radius-xl: 16px;
  --eleme-spacing-xs: 4px;
  --eleme-spacing-sm: 8px;
  --eleme-spacing-md: 12px;
  --eleme-spacing-lg: 16px;
  --eleme-spacing-xl: 24px;
  --eleme-spacing-2xl: 32px;
}
```
