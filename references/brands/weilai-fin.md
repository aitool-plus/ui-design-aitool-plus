# 微众银行 设计规范

> 微众蓝·数字银行·普惠金融 | 主色：#2B6CB0

---

## 一、设计价值观与原则

**价值观**：数字银行·普惠金融·科技驱动
**设计原则**：
- 数字优先：纯线上体验，界面简洁高效
- 普惠友好：降低金融理解门槛，文案通俗易懂
- 安全信任：蓝色传递安全，操作确认步骤清晰
- 无障碍：大字号、高对比度、清晰图标

## 二、配色体系

### 品牌主色色板
| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | #EBF4FF | 主色极浅背景 |
| 100 | #C3D9F5 | 主色浅背景 |
| 200 | #9BBEEB | 主色浅色标签 |
| 300 | #73A3E0 | 主色辅助高亮 |
| 400 | #4F8DD6 | 主色悬浮态 |
| 500 | #2B6CB0 | **品牌主色** |
| 600 | #225895 | 主色按压态 |
| 700 | #1A447A | 主色深色 |
| 800 | #12305F | 主色极深 |
| 900 | #0B1E44 | 主色最深 |

### 功能色
| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | #00B42A | 贷款审批、转账成功 |
| 警告 | #FF7D00 | 还款提醒、额度紧张 |
| 错误 | #F53F3F | 转账失败、审批拒绝 |
| 信息 | #2B6CB0 | 引导提示（复用主色） |

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
- 主色渐变：`linear-gradient(135deg, #2B6CB0, #4, #4F8DD6)`
- 金融渐变：`linear-gradient(135deg, #2B6CB0, #00B42A)`

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
| Bold | 700 | 页面标题、金额 |

## 四、组件设计规范

### 按钮
| 类型 | 高度 | 圆角 | 字号 | 背景色 |
|------|------|------|------|--------|
| 主要按钮 | 44px | 8px | 16px/500 | #2B6CB0 |
| 次要按钮 | 40px | 8px | 14px/500 | #EBF4FF |
| 文字按钮 | — | — | 14px/500 | transparent |
| 标签按钮 | 28px | 4px | 12px/500 | #EBF4FF |

### 卡片
| 类型 | 圆角 | 阴影 | 内边距 |
|------|------|------|--------|
| 账户卡片 | 12px | 0 2px 12px rgba(0,0,0,0.08) | 16px |
| 产品卡片 | 8px | 0 1px 6px rgba(0,0,0,0.06) | 16px |
| 信息卡片 | 8px | 0 1px 4px rgba(0,0,0,0.04) | 16px |

### 导航栏
- 高度：48px，背景 #FFFFFF
- 标题字号：18px/700，颜色 #1D2129
- 返回图标：24px，颜色 #4E5969

### 弹窗
- 圆角：12px，遮罩 rgba(0,0,0,0.5)
- 标题字号：18px/700，内容 14px/400
- 按钮高度：44px

### 输入框
- 高度：40px，圆角 8px
- 边框：1px solid #E5E6EB，聚焦 #2B6CB0
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
| xl | 16px | 大弹窗、底部面板 |
| full | 9999px | 胶囊按钮、头像 |

## 六、动效规范

| 场景 | 时长 | 缓动函数 |
|------|------|----------|
| 按钮反馈 | 150ms | ease-out |
| 页面切换 | 300ms | cubic-bezier(0.25,0.1,0.25,1) |
| 弹窗弹出 | 250ms | cubic-bezier(0.34,1.56,0.64,1) |
| 数据刷新 | 400ms | ease-in-out |
| 骨架屏闪烁 | 1.5s | ease-in-out (loop) |

## 七、暗色模式规范

| 元素 | 亮色 | 暗色 |
|------|------|------|
| 页面背景 | #F7F8FA | #0D0D0D |
| 卡片背景 | #FFFFFF | #1A1A1A |
| 主色 | #2B6CB0 | #4F8DD6 |
| 标题文字 | #1D2129 | #F5F5F5 |
| 正文文字 | #4E5969 | #C9CDD4 |
| 辅助文字 | #86909C | #6B7785 |
| 边框 | #E5E6EB | #2E2E2E |
| 分割线 | #F2F3F5 | #232323 |

## 八、设计禁忌

- ✅ Do：转账金额使用Bold 700，字号≥20px
- ✅ Do：操作确认弹窗必须包含金额、账户信息
- ❌ Don't：禁止金额使用灰色或Regular字重
- ❌ Don't：禁止省略操作确认步骤
- ❌ Don't：禁止使用红色作为主CTA
- ❌ Don't：禁止账户余额缺少币种标识

## 九、CSS变量快速参考

```css
:root {
  --weilai-primary: #2B6CB0;
  --weilai-primary-50: #EBF4FF;
  --weilai-primary-100: #C3D9F5;
  --weilai-primary-200: #9BBEEB;
  --weilai-primary-300: #73A3E0;
  --weilai-primary-400: #4F8DD6;
  --weilai-primary-500: #2B6CB0;
  --weilai-primary-600: #225895;
  --weilai-primary-700: #1A447A;
  --weilai-primary-800: #12305F;
  --weilai-primary-900: #0B1E44;
  --weilai-success: #00B42A;
  --weilai-warning: #FF7D00;
  --weilai-error: #F53F3F;
  --weilai-text-title: #1D2129;
  --weilai-text-body: #4E5969;
  --weilai-text-secondary: #86909C;
  --weilai-text-placeholder: #C9CDD4;
  --weilai-border: #E5E6EB;
  --weilai-bg-page: #F7F8FA;
  --weilai-bg-card: #FFFFFF;
  --weilai-radius-sm: 4px;
  --weilai-radius-md: 8px;
  --weilai-radius-lg: 12px;
  --weilai-radius-xl: 16px;
  --weilai-spacing-xs: 4px;
  --weilai-spacing-sm: 8px;
  --weilai-spacing-md: 12px;
  --weilai-spacing-lg: 16px;
  --weilai-spacing-xl: 24px;
  --weilai-spacing-2xl: 32px;
}
```