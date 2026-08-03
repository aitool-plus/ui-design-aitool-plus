# 中信 设计规范

> 中信红·综合金融·信任价值 | 主色：#C41230

---

## 一、设计价值观与原则

**价值观**：综合金融·信任价值·稳健经营
**设计原则**：
- 信任权威：红色传递力量与信任，金融信息权威呈现
- 综合服务：银行、证券、信托多业务视觉统一
- 稳健克制：减少装饰，数据与表单为核心
- 合规底线：风险提示、合规声明不可省略

## 二、配色体系

### 品牌主色色板
| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | #FCE8EB | 主色极浅背景 |
| 100 | #F5B8C2 | 主色浅背景 |
| 200 | #ED8DA0 | 主色浅色标签 |
| 300 | #E5627D | 主色辅助高亮 |
| 400 | #D93D58 | 主色悬浮态 |
| 500 | #C41230 | **品牌主色** |
| 600 | #A30E28 | 主色按压态 |
| 700 | #820A20 | 主色深色 |
| 800 | #610718 | 主色极深 |
| 900 | #450410 | 主色最深 |

### 功能色
| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | #00B42A | 交易成功、审批通过 |
| 警告 | #FF7D00 | 风险提醒、额度紧张 |
| 错误 | #F53F3F | 交易失败、审批拒绝 |
| 信息 | #C41230 | 引导提示（复用主色） |

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
- 主色渐变：`linear-gradient(135deg, #C41230, #D93D58)`
- 金融渐变：`linear-gradient(135deg, #C41230, #1E40AF)`

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
| 主要按钮 | 44px | 8px | 16px/500 | #C41230 |
| 次要按钮 | 40px | 8px | 14px/500 | #FCE8EB |
| 文字按钮 | — | — | 14px/500 | transparent |
| 标签按钮 | 28px | 4px | 12px/500 | #FCE8EB |

### 卡片
| 类型 | 圆角 | 阴影 | 内边距 |
|------|------|------|--------|
| 产品卡片 | 12px | 0 2px 12px rgba(0,0,0,0.08) | 16px |
| 账户卡片 | 8px | 0 1px 6px rgba(0,0,0,0.06) | 16px |
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
- 边框：1px solid #E5E6EB，聚焦 #C41230
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
| 主色 | #C41230 | #D93D58 |
| 标题文字 | #1D2129 | #F5F5F5 |
| 正文文字 | #4E5969 | #C9CDD4 |
| 辅助文字 | #86909C | #6B7785 |
| 边框 | #E5E6EB | #2E2E2E |
| 分割线 | #F2F3F5 | #232323 |

## 八、设计禁忌

- ✅ Do：金额数字使用Bold 700，字号≥18px
- ✅ Do：风险提示使用警告色+图标
- ❌ Don't：禁止金额使用灰色或小字号
- ❌ Don't：禁止隐藏风险提示或合规声明
- ❌ Don't：禁止使用绿色作为主CTA（与红色冲突）
- ❌ Don't：禁止金融产品缺少风险等级标识

## 九、CSS变量快速参考

```css
:root {
  --zhongxin-primary: #C41230;
  --zhongxin-primary-50: #FCE8EB;
  --zhongxin-primary-100: #F5B8C2;
  --zhongxin-primary-200: #ED8DA0;
  --zhongxin-primary-300: #E5627D;
  --zhongxin-primary-400: #D93D58;
  --zhongxin-primary-500: #C41230;
  --zhongxin-primary-600: #A30E28;
  --zhongxin-primary-700: #820A20;
  --zhongxin-primary-800: #610718;
  --zhongxin-primary-900: #450410;
  --zhongxin-success: #00B42A;
  --zhongxin-warning: #FF7D00;
  --zhongxin-error: #F53F3F;
  --zhongxin-text-title: #1D2129;
  --zhongxin-text-body: #4E5969;
  --zhongxin-text-secondary: #86909C;
  --zhongxin-text-placeholder: #C9CDD4;
  --zhongxin-border: #E5E6EB;
  --zhongxin-bg-page: #F7F8FA;
  --zhongxin-bg-card: #FFFFFF;
  --zhongxin-radius-sm: 4px;
  --zhongxin-radius-md: 8px;
  --zhongxin-radius-lg: 12px;
  --zhongxin-radius-xl: 16px;
  --zhongxin-spacing-xs: 4px;
  --zhongxin-spacing-sm: 8px;
  --zhongxin-spacing-md: 12px;
  --zhongxin-spacing-lg: 16px;
  --zhongxin-spacing-xl: 24px;
  --zhongxin-spacing-2xl: 32px;
}
```