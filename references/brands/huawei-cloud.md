# 华为云 设计规范

> 云端红·智能云·一切皆服务 | 主色：#CF0A2C

---

## 一、设计价值观与原则

**价值观**：智能云·一切皆服务·技术自立
**设计原则**：
- 技术权威：红色传递力量与自信，技术文档专业
- 一切皆服务：IaaS/PaaS/SaaS层级清晰
- 开发者友好：API文档、SDK、控制台体验统一
- 安全可信：安全认证、合规标识始终可见

## 二、配色体系

### 品牌主色色板
| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | #FCE8EB | 主色极浅背景 |
| 100 | #F5B8C2 | 主色浅背景 |
| 200 | #ED8DA0 | 主色浅色标签 |
| 300 | #E562D58 | 主色辅助高亮 |
| 400 | #E03050 | 主色悬浮态 |
| 500 | #CF0A2C | **品牌主色** |
| 600 | #B00824 | 主色按压态 |
| 700 | #91061D | 主色深色 |
| 800 | #720416 | 主色极深 |
| 900 | #56030F | 主色最深 |

### 功能色
| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | #00B42A | 部署成功、实例运行 |
| 警告 | #FF7D00 | 资源不足、费用预警 |
| 错误 | #F53F3F | 部署失败、实例异常 |
| 信息 | #CF0A2C | 引导提示（复用主色） |

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
- 主色渐变：`linear-gradient(135deg, #CF0A2C, #E03050)`
- 云端渐变：`linear-gradient(90deg, #CF0A2C, #0052D9)`

## 三、字体排版体系

### 字体家族
- 中文：`"PingFang SC", "HarmonyOS Sans", "Microsoft YaHei", sans-serif`
- 英文：`"Roboto", "Helvetica Neue", Arial, sans-serif`
- 数字/代码：`"Roboto Mono", "SF Mono", monospace`

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
| 主要按钮 | 36px | 8px | 14px/500 | #CF0A2C |
| 次要按钮 | 32px | 8px | 14px/500 | #FCE8EB |
| 文字按钮 | — | — | 14px/500 | transparent |
| 标签按钮 | 24px | 4px | 12px/500 | #FCE8EB |

### 卡片
| 类型 | 圆角 | 阴影 | 内边距 |
|------|------|------|--------|
| 服务卡片 | 8px | 0 1px 4px rgba(0,0,0,0.04) | 16px |
| 实例卡片 | 8px | 0 1px 6px rgba(0,0,0,0.06) | 16px |
| 信息卡片 | 8px | 0 1px 4px rgba(0,0,0,0.04) | 16px |

### 导航栏
- 高度：48px，背景 #FFFFFF
- 标题字号：16px/700，颜色 #1D2129
- 侧边栏宽度：220px

### 弹窗
- 圆角：12px，遮罩 rgba(0,0,0,0.4)
- 标题字号：16px/700，内容 14px/400
- 按钮高度：36px

### 输入框
- 高度：36px，圆角 8px
- 边框：1px solid #E5E6EB，聚焦 #CF0A2C
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
| md | 8px | 输入框、按钮、卡片 |
| lg | 12px | 弹窗、面板 |
| xl | 16px | 大弹窗 |
| full | 9999px | 头像、胶囊 |

## 六、动效规范

| 场景 | 时长 | 缓动函数 |
|------|------|----------|
| 按钮反馈 | 120ms | ease-out |
| 页面切换 | 200ms | cubic-bezier(0.25,0.1,0.25,1) |
| 弹窗弹出 | 200ms | cubic-bezier(0.34,1.56,0.64,1) |
| 数据刷新 | 400ms | ease-in-out |
| 骨架屏闪烁 | 1.5s | ease-in-out (loop) |

## 七、暗色模式规范

| 元素 | 亮色 | 暗色 |
|------|------|------|
| 页面背景 | #F7F8FA | #0D0D0D |
| 卡片背景 | #FFFFFF | #1A1A1A |
| 主色 | #CF0A2C | #E03050 |
| 标题文字 | #1D2129 | #F5F5F5 |
| 正文文字 | #4E5969 | #C9CDD4 |
| 辅助文字 | #86909C | #6B7785 |
| 边框 | #E5E6EB | #2E2E2E |
| 分割线 | #F2F3F5 | #232323 |

## 八、设计禁忌

- ✅ Do：API文档使用等宽字体
- ✅ Do：实例状态使用功能色标签
- ❌ Don't：禁止API文档使用非等宽字体
- ❌ Don't：禁止实例状态使用灰色标识
- ❌ Don't：禁止使用蓝色作为主CTA
- ❌ Don't：禁止控制台缺少费用信息

## 九、CSS变量快速参考

```css
:root {
  --hwcloud-primary: #CF0A2C;
  --hwcloud-primary-50: #FCE8EB;
  --hwcloud-primary-100: #F5B8C2;
  --hwcloud-primary-200: #ED8DA0;
  --hwcloud-primary-300: #E03050;
  --hwcloud-primary-400: #D81C3E;
  --hwcloud-primary-500: #CF0A2C;
  --hwcloud-primary-600: #B00824;
  --hwcloud-primary-700: #91061D;
  --hwcloud-primary-800: #720416;
  --hwcloud-primary-900: #56030F;
  --hwcloud-success: #00B42A;
  --hwcloud-warning: #FF7D00;
  --hwcloud-error: #F53F3F;
  --hwcloud-text-title: #1D2129;
  --hwcloud-text-body: #4E5969;
  --hwcloud-text-secondary: #86909C;
  --hwcloud-text-placeholder: #C9CDD4;
  --hwcloud-border: #E5E6EB;
  --hwcloud-bg-page: #F7F8FA;
  --hwcloud-bg-card: #FFFFFF;
  --hwcloud-radius-sm: 4px;
  --hwcloud-radius-md: 8px;
  --hwcloud-radius-lg: 12px;
  --hwcloud-radius-xl: 16px;
  --hwcloud-spacing-xs: 4px;
  --hwcloud-spacing-sm: 8px;
  --hwcloud-spacing-md: 12px;
  --hwcloud-spacing-lg: 16px;
  --hwcloud-spacing-xl: 24px;
  --hwcloud-spacing-2xl: 32px;
}
```