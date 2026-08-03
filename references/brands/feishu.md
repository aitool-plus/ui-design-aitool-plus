# 飞书 设计规范

> 协作紫·先进协作·高效愉悦 | 主色：#7B67EE

---

## 一、设计价值观与原则

**价值观**：先进协作·高效愉悦·组织进化
**设计原则**：
- 高效愉悦：紫色传递创意与活力，操作流畅自然
- 信息降噪：减少视觉噪音，内容为核心
- 协作优先：多人在线状态、评论批注始终可见
- 一致体验：文档、表格、会议、IM视觉统一

## 二、配色体系

### 品牌主色色板
| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | #F0EDFF | 主色极浅背景 |
| 100 | #D9D3FF | 主色浅背景 |
| 200 | #B8AEFF | 主色浅色标签 |
| 300 | #9B8AFF | 主色辅助高亮 |
| 400 | #8A76FF | 主色悬浮态 |
| 500 | #7B67EE | **品牌主色** |
| 600 | #6552D6 | 主色按压态 |
| 700 | #5040BE | 主色深色 |
| 800 | #3C2FA6 | 主色极深 |
| 900 | #2A208E | 主色最深 |

### 功能色
| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | #00B42A | 发送成功、保存完成 |
| 警告 | #FF7D00 | 权限不足、存储空间 |
| 错误 | #F53F3F | 发送失败、网络异常 |
| 信息 | #7B67EE | 引导提示（复用主色） |

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
- 主色渐变：`linear-gradient(135deg, #7B67EE, #9B8AFF)`
- 协作渐变：`linear-gradient(90deg, #7B67EE, #0089FF)`

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
| 主要按钮 | 36px | 8px | 14px/500 | #7B67EE |
| 次要按钮 | 32px | 8px | 14px/500 | #F0EDFF |
| 文字按钮 | — | — | 14px/500 | transparent |
| 标签按钮 | 24px | 4px | 12px/500 | #F0EDFF |

### 卡片
| 类型 | 圆角 | 阴影 | 内边距 |
|------|------|------|--------|
| 文档卡片 | 8px | 0 1px 4px rgba(0,0,0,0.04) | 16px |
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
- 边框：1px solid #E5E6EB，聚焦 #7B67EE
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
| 主色 | #7B67EE | #9B8AFF |
| 标题文字 | #1D2129 | #F5F5F5 |
| 正文文字 | #4E5969 | #C9CDD4 |
| 辅助文字 | #86909C | #6B7785 |
| 边框 | #E5E6EB | #3A3A3A |
| 分割线 | #F2F3F5 | #2E2E2E |

## 八、设计禁忌

- ✅ Do：在线协作者头像使用主色边框标识
- ✅ Do：消息输入框使用圆角8px，友好感
- ❌ Don't：禁止使用大面积紫色背景（压抑感）
- ❌ Don't：禁止消息列表缺少时间戳
- ❌ Don't：禁止文档编辑区使用深色背景
- ❌ Don't：禁止侧边栏图标缺少hover态

## 九、CSS变量快速参考

```css
:root {
  --feishu-primary: #7B67EE;
  --feishu-primary-50: #F0EDFF;
  --feishu-primary-100: #D9D3FF;
  --feishu-primary-200: #B8AEFF;
  --feishu-primary-300: #9B8AFF;
  --feishu-primary-400: #8A76FF;
  --feishu-primary-500: #7B67EE;
  --feishu-primary-600: #6552D6;
  --feishu-primary-700: #5040BE;
  --feishu-primary-800: #3C2FA6;
  --feishu-primary-900: #2A208E;
  --feishu-success: #00B42A;
  --feishu-warning: #FF7D00;
  --feishu-error: #F53F3F;
  --feishu-text-title: #1D2129;
  --feishu-text-body: #4E5969;
  --feishu-text-secondary: #86909C;
  --feishu-text-placeholder: #C9CDD4;
  --feishu-border: #E5E6EB;
  --feishu-bg-page: #F7F8FA;
  --feishu-bg-card: #FFFFFF;
  --feishu-radius-sm: 4px;
  --feishu-radius-md: 8px;
  --feishu-radius-lg: 12px;
  --feishu-radius-xl: 16px;
  --feishu-spacing-xs: 4px;
  --feishu-spacing-sm: 8px;
  --feishu-spacing-md: 12px;
  --feishu-spacing-lg: 16px;
  --feishu-spacing-xl: 24px;
  --feishu-spacing-2xl: 32px;
}
```