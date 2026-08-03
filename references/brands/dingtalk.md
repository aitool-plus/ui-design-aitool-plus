# 钉钉 设计规范

> 效率蓝·让工作更简单·数字化 | 主色：#0089FF

---

## 一、设计价值观与原则

**价值观**：让工作更简单·数字化·效率优先
**设计原则**：
- 效率至上：蓝色传递专业与效率，操作路径最短
- 工作优先：减少娱乐化元素，专注工作场景
- 数字化驱动：审批、考勤、日志流程可视化
- 组织协同：组织架构、权限层级清晰

## 二、配色体系

### 品牌主色色板
| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | #E6F2FF | 主色极浅背景 |
| 100 | #B3D9FF | 主色浅背景 |
| 200 | #80BFFF | 主色浅色标签 |
| 300 | #4DA6FF | 主色辅助高亮 |
| 400 | #1A95FF | 主色悬浮态 |
| 500 | #0089FF | **品牌主色** |
| 600 | #0073D9 | 主色按压态 |
| 700 | #005CB3 | 主色深色 |
| 800 | #00458C | 主色极深 |
| 900 | #003166 | 主色最深 |

### 功能色
| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | #00B42A | 审批通过、打卡成功 |
| 警告 | #FF7D00 | 审批待处理、考勤异常 |
| 错误 | #F53F3F | 审批拒绝、网络异常 |
| 信息 | #0089FF | 引导提示（复用主色） |

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
- 主色渐变：`linear-gradient(135deg, #0089FF, #4DA6FF)`
- 效率渐变：`linear-gradient(90deg, #0089FF, #00B42A)`

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
| Bold | 700 | 页面标题、强调 |

## 四、组件设计规范

### 按钮
| 类型 | 高度 | 圆角 | 字号 | 背景色 |
|------|------|------|------|--------|
| 主要按钮 | 36px | 8px | 14px/500 | #0089FF |
| 次要按钮 | 32px | 8px | 14px/500 | #E6F2FF |
| 文字按钮 | — | — | 14px/500 | transparent |
| 标签按钮 | 24px | 4px | 12px/500 | #E6F2FF |

### 卡片
| 类型 | 圆角 | 阴影 | 内边距 |
|------|------|------|--------|
| 审批卡片 | 8px | 0 1px 4px rgba(0,0,0,0.04) | 16px |
| 消息卡片 | 8px | 0 1px 3px rgba(0,0,0,0.03) | 12px |
| 信息卡片 | 8px | 0 1px 4px rgba(0,0,0,0.04) | 16px |

### 导航栏
- 高度：48px，背景 #FFFFFF
- 标题字号：16px/700，颜色 #1D2129
- 侧边栏宽度：240px

### 弹窗
- 圆角：12px，遮罩 rgba(0,0,0,0.4)
- 标题字号：16px/700，内容 14px/400
- 按钮高度：36px

### 输入框
- 高度：36px，圆角 8px
- 边框：1px solid #E5E6EB，聚焦 #0089FF
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
| 侧边栏展开 | 250ms | ease-in-out |
| 骨架屏闪烁 | 1.5s | ease-in-out (loop) |

## 七、暗色模式规范

| 元素 | 亮色 | 暗色 |
|------|------|------|
| 页面背景 | #F7F8FA | #1A1A1A |
| 卡片背景 | #FFFFFF | #2A2A2A |
| 主色 | #0089FF | #4DA6FF |
| 标题文字 | #1D2129 | #F5F5F5 |
| 正文文字 | #4E5969 | #C9CDD4 |
| 辅助文字 | #86909C | #6B7785 |
| 边框 | #E5E6EB | #3A3A3A |
| 分割线 | #F2F3F5 | #2E2E2E |

## 八、设计禁忌

- ✅ Do：审批状态使用功能色明确标识
- ✅ Do：考勤打卡按钮使用主色大圆角
- ❌ Don't：禁止审批状态使用灰色或模糊标识
- ❌ Don't：禁止使用紫色或绿色作为主CTA
- ❌ Don't：禁止消息列表缺少已读/未读状态
- ❌ Don't：禁止工作台使用娱乐化动效

## 九、CSS变量快速参考

```css
:root {
  --dingtalk-primary: #0089FF;
  --dingtalk-primary-50: #E6F2FF;
  --dingtalk-primary-100: #B3D9FF;
  --dingtalk-primary-200: #80BFFF;
  --dingtalk-primary-300: #4DA6FF;
  --dingtalk-primary-400: #1A95FF;
  --dingtalk-primary-500: #0089FF;
  --dingtalk-primary-600: #0073D9;
  --dingtalk-primary-700: #005CB3;
  --dingtalk-primary-800: #00458C;
  --dingtalk-primary-900: #003166;
  --dingtalk-success: #00B42A;
  --dingtalk-warning: #FF7D00;
  --dingtalk-error: #F53F3F;
  --dingtalk-text-title: #1D2129;
  --dingtalk-text-body: #4E5969;
  --dingtalk-text-secondary: #86909C;
  --dingtalk-text-placeholder: #C9CDD4;
  --dingtalk-border: #E5E6EB;
  --dingtalk-bg-page: #F7F8FA;
  --dingtalk-bg-card: #FFFFFF;
  --dingtalk-radius-sm: 4px;
  --dingtalk-radius-md: 8px;
  --dingtalk-radius-lg: 12px;
  --dingtalk-radius-xl: 16px;
  --dingtalk-spacing-xs: 4px;
  --dingtalk-spacing-sm: 8px;
  --dingtalk-spacing-md: 12px;
  --dingtalk-spacing-lg: 16px;
  --dingtalk-spacing-xl: 24px;
  --dingtalk-spacing-2xl: 32px;
}
```