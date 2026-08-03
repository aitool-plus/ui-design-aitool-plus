# 平安 设计规范

> 平安橙·金融+科技·专业价值 | 主色：#FF6600

---

## 一、设计价值观与原则

**价值观**：金融+科技·专业价值·平安保障
**设计原则**：
- 专业信赖：橙色传递活力与专业，金融信息清晰
- 科技赋能：数据可视化、智能推荐传递科技感
- 保障感知：保险、理赔标识始终醒目
- 一站服务：银行、保险、投资多业务视觉统一

## 二、配色体系

### 品牌主色色板
| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | #FFF2E6 | 主色极浅背景 |
| 100 | #FFD9B3 | 主色浅背景 |
| 200 | #FFBF80 | 主色浅色标签 |
| 300 | #FFA64D | 主色辅助高亮 |
| 400 | #FF851A | 主色悬浮态 |
| 500 | #FF6600 | **品牌主色** |
| 600 | #E05A00 | 主色按压态 |
| 700 | #B84D00 | 主色深色 |
| 800 | #8F3B00 | 主色极深 |
| 900 | #6B2D00 | 主色最深 |

### 功能色
| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | #00B42A | 理赔成功、审批通过 |
| 警告 | #FF7D00 | 保费到期、还款提醒 |
| 错误 | #F53F3F | 理赔拒绝、支付失败 |
| 信息 | #FF6600 | 引导提示（复用主色） |

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
- 主色渐变：`linear-gradient(135deg, #FF6600, #FF851A)`
- 金融渐变：`linear-gradient(135deg, #FF6600, #00B42A)`

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
| 主要按钮 | 44px | 8px | 16px/500 | #FF6600 |
| 次要按钮 | 40px | 8px | 14px/500 | #FFF2E6 |
| 文字按钮 | — | — | 14px/500 | transparent |
| 标签按钮 | 28px | 4px | 12px/500 | #FFF2E6 |

### 卡片
| 类型 | 圆角 | 阴影 | 内边距 |
|------|------|------|--------|
| 保险卡片 | 12px | 0 2px 12px rgba(0,0,0,0.08) | 16px |
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
- 边框：1px solid #E5E6EB，聚焦 #FF6600
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
| 主色 | #FF6600 | #FF851A |
| 标题文字 | #1D2129 | #F5F5F5 |
| 正文文字 | #4E5969 | #C9CDD4 |
| 辅助文字 | #86909C | #6B7785 |
| 边框 | #E5E6EB | #2E2E2E |
| 分割线 | #F2F3F5 | #232323 |

## 八、设计禁忌

- ✅ Do：保险产品卡片必须包含保障范围摘要
- ✅ Do：理赔进度使用步骤条可视化
- ❌ Don't：禁止保险产品缺少保障范围标识
- ❌ Don't：禁止理赔进度使用纯文字无可视化
- ❌ Don't：禁止使用蓝色作为主CTA（与橙色冲突）
- ❌ Don't：禁止保费金额使用灰色或小字号

## 九、CSS变量快速参考

```css
:root {
  --pingan-primary: #FF6600;
  --pingan-primary-50: #FFF2E6;
  --pingan-primary-100: #FFD9B3;
  --pingan-primary-200: #FFBF80;
  --pingan-primary-300: #FFA64D;
  --pingan-primary-400: #FF851A;
  --pingan-primary-500: #FF6600;
  --pingan-primary-600: #E05A00;
  --pingan-primary-700: #B84D00;
  --pingan-primary-800: #8F3B00;
  --pingan-primary-900: #6B2D00;
  --pingan-success: #00B42A;
  --pingan-warning: #FF7D00;
  --pingan-error: #F53F3F;
  --pingan-text-title: #1D2129;
  --pingan-text-body: #4E5969;
  --pingan-text-secondary: #86909C;
  --pingan-text-placeholder: #C9CDD4;
  --pingan-border: #E5E6EB;
  --pingan-bg-page: #F7F8FA;
  --pingan-bg-card: #FFFFFF;
  --pingan-radius-sm: 4px;
  --pingan-radius-md: 8px;
  --pingan-radius-lg: 12px;
  --pingan-radius-xl: 16px;
  --pingan-spacing-xs: 4px;
  --pingan-spacing-sm: 8px;
  --pingan-spacing-md: 12px;
  --pingan-spacing-lg: 16px;
  --pingan-spacing-xl: 24px;
  --pingan-spacing-2xl: 32px;
}
```