# 陆金所 设计规范

> 稳健蓝绿·财富管理·安全增值 | 主色：#00857C

---

## 一、设计价值观与原则

**价值观**：稳健增值·专业财富·安全信赖
**设计原则**：
- 稳健信任：蓝绿色传递稳健与专业，金融数据精确呈现
- 安全感知：风险等级、安全保障标识始终可见
- 专业克制：减少装饰元素，数据与图表为核心
- 合规优先：风险提示、合规声明不可省略

## 二、配色体系

### 品牌主色色板
| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | #E6F5F4 | 主色极浅背景 |
| 100 | #B3E3E0 | 主色浅背景 |
| 200 | #80D1CC | 主色浅色标签 |
| 300 | #4DBFB8 | 主色辅助高亮 |
| 400 | #26B3AA | 主色悬浮态 |
| 500 | #00857C | **品牌主色** |
| 600 | #006E67 | 主色按压态 |
| 700 | #005752 | 主色深色 |
| 800 | #00403C | 主色极深 |
| 900 | #002D2A | 主色最深 |

### 功能色
| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | #00B42A | 收益到账、申购成功 |
| 警告 | #FF7D00 | 风险提醒、净值波动 |
| 错误 | #F53F3F | 交易失败、风险超限 |
| 信息 | #00857C | 引导提示（复用主色） |

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
- 主色渐变：`linear-gradient(135deg, #00857C, #26B3AA)`
- 收益渐变：`linear-gradient(135deg, #00857C, #00B42A)`

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
| 主要按钮 | 44px | 8px | 16px/500 | #00857C |
| 次要按钮 | 40px | 8px | 14px/500 | #E6F5F4 |
| 文字按钮 | — | — | 14px/500 | transparent |
| 标签按钮 | 28px | 4px | 12px/500 | #E6F5F4 |

### 卡片
| 类型 | 圆角 | 阴影 | 内边距 |
|------|------|------|--------|
| 产品卡片 | 12px | 0 2px 12px rgba(0,0,0,0.08) | 16px |
| 收益卡片 | 8px | 0 1px 6px rgba(0,0,0,0.06) | 16px |
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
- 边框：1px solid #E5E6EB，聚焦 #00857C
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
| 主色 | #00857C | #26B3AA |
| 标题文字 | #1D2129 | #F5F5F5 |
| 正文文字 | #4E5969 | #C9CDD4 |
| 辅助文字 | #86909C | #6B7785 |
| 边框 | #E5E6EB | #2E2E2E |
| 分割线 | #F2F3F5 | #232323 |

## 八、设计禁忌

- ✅ Do：收益率使用主色Bold，字号≥18px
- ✅ Do：风险等级标签使用对应功能色
- ❌ Don't：禁止收益率使用灰色或小字号
- ❌ Don't：禁止隐藏风险提示或合规声明
- ❌ Don't：禁止使用红色作为主CTA（引发焦虑）
- ❌ Don't：禁止收益数据缺少时间范围标识

## 九、CSS变量快速参考

```css
:root {
  --lufax-primary: #00857C;
  --lufax-primary-50: #E6F5F4;
  --lufax-primary-100: #B3E3E0;
  --lufax-primary-200: #80D1CC;
  --lufax-primary-300: #4DBFB8;
  --lufax-primary-400: #26B3AA;
  --lufax-primary-500: #00857C;
  --lufax-primary-600: #006E67;
  --lufax-primary-700: #005752;
  --lufax-primary-800: #00403C;
  --lufax-primary-900: #002D2A;
  --lufax-success: #00B42A;
  --lufax-warning: #FF7D00;
  --lufax-error: #F53F3F;
  --lufax-text-title: #1D2129;
  --lufax-text-body: #4E5969;
  --lufax-text-secondary: #86909C;
  --lufax-text-placeholder: #C9CDD4;
  --lufax-border: #E5E6EB;
  --lufax-bg-page: #F7F8FA;
  --lufax-bg-card: #FFFFFF;
  --lufax-radius-sm: 4px;
  --lufax-radius-md: 8px;
  --lufax-radius-lg: 12px;
  --lufax-radius-xl: 16px;
  --lufax-spacing-xs: 4px;
  --lufax-spacing-sm: 8px;
  --lufax-spacing-md: 12px;
  --lufax-spacing-lg: 16px;
  --lufax-spacing-xl: 24px;
  --lufax-spacing-2xl: 32px;
}
```