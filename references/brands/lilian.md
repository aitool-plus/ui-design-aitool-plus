# 立林 设计规范

> 金融蓝·智能投顾·量化交易 | 主色：#1E40AF

---

## 一、设计价值观与原则

**价值观**：智能投顾·量化精准·专业金融
**设计原则**：
- 专业深度：深蓝传递专业与权威，数据密度高
- 量化精准：图表、K线、数据面板为核心视觉
- 效率优先：信息层级清晰，操作路径最短
- 风控可见：风险指标、止损线始终可见

## 二、配色体系

### 品牌主色色板
| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | #E8EAF6 | 主色极浅背景 |
| 100 | #C5CAE9 | 主色浅背景 |
| 200 | #9FA8DA | 主色浅色标签 |
| 300 | #7986CB | 主色辅助高亮 |
| 400 | #3949AB | 主色悬浮态 |
| 500 | #1E40AF | **品牌主色** |
| 600 | #173590 | 主色按压态 |
| 700 | #112A72 | 主色深色 |
| 800 | #0C1F55 | 主色极深 |
| 900 | #08153D | 主色最深 |

### 功能色
| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | #00B42A | 盈利、交易成功 |
| 警告 | #FF7D00 | 风险预警、止损提醒 |
| 错误 | #F53F3F | 亏损、交易失败 |
| 信息 | #1E40AF | 引导提示（复用主色） |

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
- 主色渐变：`linear-gradient(135deg, #1E40AF, #3949AB)`
- 涨跌渐变：`linear-gradient(90deg, #F53F3F, #00B42A)`

## 三、字体排版体系

### 字体家族
- 中文：`"PingFang SC", "HarmonyOS Sans", "Microsoft YaHei", sans-serif`
- 英文：`"Roboto Mono", "SF Mono", monospace`
- 数字：`"Roboto Mono", "DIN Alternate", monospace`

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
| 主要按钮 | 44px | 8px | 16px/500 | #1E40AF |
| 次要按钮 | 40px | 8px | 14px/500 | #E8EAF6 |
| 文字按钮 | — | — | 14px/500 | transparent |
| 标签按钮 | 28px | 4px | 12px/500 | #E8EAF6 |

### 卡片
| 类型 | 圆角 | 阴影 | 内边距 |
|------|------|------|--------|
| 交易卡片 | 8px | 0 2px 12px rgba(0,0,0,0.08) | 16px |
| 数据卡片 | 8px | 0 1px 6px rgba(0,0,0,0.06) | 16px |
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
- 边框：1px solid #E5E6EB，聚焦 #1E40AF
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
| 主色 | #1E40AF | #3949AB |
| 标题文字 | #1D2129 | #F5F5F5 |
| 正文文字 | #4E5969 | #C9CDD4 |
| 辅助文字 | #86909C | #6B7785 |
| 边框 | #E5E6EB | #2E2E2E |
| 分割线 | #F2F3F5 | #232323 |

## 八、设计禁忌

- ✅ Do：交易数据使用等宽字体对齐
- ✅ Do：涨跌使用红绿双色明确区分
- ❌ Don't：禁止交易金额使用非等宽字体
- ❌ Don't：禁止隐藏风险指标或止损线
- ❌ Don't：禁止使用橙色作为主CTA
- ❌ Don't：禁止K线图缺少时间轴标注

## 九、CSS变量快速参考

```css
:root {
  --lilian-primary: #1E40AF;
  --lilian-primary-50: #E8EAF6;
  --lilian-primary-100: #C5CAE9;
  --lilian-primary-200: #9FA8DA;
  --lilian-primary-300: #7986CB;
  --lilian-primary-400: #3949AB;
  --lilian-primary-500: #1E40AF;
  --lilian-primary-600: #173590;
  --lilian-primary-700: #112A72;
  --lilian-primary-800: #0C1F55;
  --lilian-primary-900: #08153D;
  --lilian-success: #00B42A;
  --lilian-warning: #FF7D00;
  --lilian-error: #F53F3F;
  --lilian-text-title: #1D2129;
  --lilian-text-body: #4E5969;
  --lilian-text-secondary: #86909C;
  --lilian-text-placeholder: #C9CDD4;
  --lilian-border: #E5E6EB;
  --lilian-bg-page: #F7F8FA;
  --lilian-bg-card: #FFFFFF;
  --lilian-radius-sm: 4px;
  --lilian-radius-md: 8px;
  --lilian-radius-lg: 12px;
  --lilian-radius-xl: 16px;
  --lilian-spacing-xs: 4px;
  --lilian-spacing-sm: 8px;
  --lilian-spacing-md: 12px;
  --lilian-spacing-lg: 16px;
  --lilian-spacing-xl: 24px;
  --lilian-spacing-2xl: 32px;
}
```