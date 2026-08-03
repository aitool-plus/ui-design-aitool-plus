# 金蝶 设计规范

> 管理蓝·企业管理·数字转型 | 主色：#0052D9

---

## 一、设计价值观与原则

**价值观**：企业管理·数字转型·致良知
**设计原则**：
- 管理专业：蓝色传递专业与可靠，ERP界面信息密度高
- 数字转型：数据可视化、智能报表传递科技感
- 流程规范：审批流、业务流程可视化
- 企业级：多角色、多权限、多组织适配

## 二、配色体系

### 品牌主色色板
| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | #E8EFFF | 主色极浅背景 |
| 100 | #B3CFF5 | 主色浅背景 |
| 200 | #80AFEB | 主色浅色标签 |
| 300 | #4D8FE0 | 主色辅助高亮 |
| 400 | #2670D6 | 主色悬浮态 |
| 500 | #0052D9 | **品牌主色** |
| 600 | #0044B8 | 主色按压态 |
| 700 | #003697 | 主色深色 |
| 800 | #002876 | 主色极深 |
| 900 | #001A55 | 主色最深 |

### 功能色
| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | #00B42A | 审批通过、操作成功 |
| 警告 | #FF7D00 | 审批待处理、数据异常 |
| 错误 | #F53F3F | 审批拒绝、操作失败 |
| 信息 | #0052D9 | 引导提示（复用主色） |

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
- 主色渐变：`linear-gradient(135deg, #0052D9, #2670D6)`
- 管理渐变：`linear-gradient(90deg, #0052D9, #00B42A)`

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
|------|
| Regular | 400 | 正文、辅助文字 |
| Medium | 500 | 卡片标题、按钮 |
| Bold | 700 | 页面标题、金额 |

## 四、组件设计规范

### 按钮
| 类型 | 高度 | 圆角 | 字号 | 背景色 |
|------|------|------|------|--------|
| 主要按钮 | 36px | 8px | 14px/500 | #0052D9 |
| 次要按钮 | 32px | 8px | 14px/500 | #E8EFFF |
| 文字按钮 | — | — | 14px/500 | transparent |
| 标签按钮 | 24px | 4px | 12px/500 | #E8EFFF |

### 卡片
| 类型 | 圆角 | 阴影 | 内边距 |
|------|------|------|--------|
| 数据卡片 | 8px | 0 1px 4px rgba(0,0,0,0.04) | 16px |
| 审批卡片 | 8px | 0 1px 6px rgba(0,0,0,0.06) | 16px |
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
- 边框：1px solid #E5E6EB，聚焦 #0052D9
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
| 页面背景 | #F7F8FA | #1A1A1A |
| 卡片背景 | #FFFFFF | #2A2A2A |
| 主色 | #0052D9 | #2670D6 |
| 标题文字 | #1D2129 | #F5F5F5 |
| 正文文字 | #4E5969 | #C9CDD4 |
| 辅助文字 | #86909C | #6B7785 |
| 边框 | #E5E6EB | #3A3A3A |
| 分割线 | #F2F3F5 | #2E2E2E |

## 八、设计禁忌

- ✅ Do：财务数据使用等宽字体对齐
- ✅ Do：审批状态使用功能色标签
- ❌ Don't：禁止财务数据使用非等宽字体
- ❌ Don't：禁止审批状态使用灰色标识
- ❌ Don't：禁止使用红色作为主CTA
- ❌ Don't：禁止报表缺少数据单位

## 九、CSS变量快速参考

```css
:root {
  --kingdee-primary: #0052D9;
  --kingdee-primary-50: #E8EFFF;
  --kingdee-primary-100: #B3CFF5;
  --kingdee-primary-200: #80AFEB;
  --kingdee-primary-300: #4D8FE0;
  --kingdee-primary-400: #2670D6;
  --kingdee-primary-500: #0052D9;
  --kingdee-primary-600: #0044B8;
  --kingdee-primary-700: #003697;
  --kingdee-primary-800: #002876;
  --kingdee-primary-900: #001A55;
  --kingdee-success: #00B42A;
  --kingdee-warning: #FF7D00;
  --kingdee-error: #F53F3F;
  --kingdee-text-title: #1D2129;
  --kingdee-text-body: #4E5969;
  --kingdee-text-secondary: #86909C;
  --kingdee-text-placeholder: #C9CDD4;
  --kingdee-border: #E5E6EB;
  --kingdee-bg-page: #F7F8FA;
  --kingdee-bg-card: #FFFFFF;
  --kingdee-radius-sm: 4px;
  --kingdee-radius-md: 8px;
  --kingdee-radius-lg: 12px;
  --kingdee-radius-xl: 16px;
  --kingdee-spacing-xs: 4px;
  --kingdee-spacing-sm: 8px;
  --kingdee-spacing-md: 12px;
  --kingdee-spacing-lg: 16px;
  --kingdee-spacing-xl: 24px;
  --kingdee-spacing-2xl: 32px;
}
```