# 阿里云 设计规范

> 计算橙·数字经济·智能算力 | 主色：#FF6A00

---

## 一、设计价值观与原则

**价值观**：数字经济·智能算力·为了无法计算的价值
**设计原则**：
- 计算力量：橙色传递活力与创新，技术文档专业
- 开发者优先：API、SDK、CLI体验统一
- 产品矩阵：ECS、OSS、RDS等产品视觉一致
- 安全可靠：安全认证、SLA标识始终可见

## 二、配色体系

### 品牌主色色板
| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | #FFF2E6 | 主色极浅背景 |
| 100 | #FFD9B3 | 主色浅背景 |
| 200 | #FFBF80 | 主色浅色标签 |
| 300 | #FFA64D | 主色辅助高亮 |
| 400 | #FF851A | 主色悬浮态 |
| 500 | #FF6A00 | **品牌主色** |
| 600 | #E05A00 | 主色按压态 |
| 700 | #B84D00 | 主色深色 |
| 800 | #8F3B00 | 主色极深 |
| 900 | #6B2D00 | 主色最深 |

### 功能色
| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | #00B42A | 部署成功、实例运行 |
| 警告 | #FF7D00 | 资源不足、费用预警 |
| 错误 | #F53F3F | 部署失败、实例异常 |
| 信息 | #FF6A00 | 引导提示（复用主色） |

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
- 主色渐变：`linear-gradient(135deg, #FF6A00, #FF851A)`
- 算力渐变：`linear-gradient(90deg, #FF6A00, #0052D9)`

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
| 主要按钮 | 36px | 8px | 14px/500 | #FF6A00 |
| 次要按钮 | 32px | 8px | 14px/500 | #FFF2E6 |
| 文字按钮 | — | — | 14px/500 | transparent |
| 标签按钮 | 24px | 4px | 12px/500 | #FFF2E6 |

### 卡片
| 类型 | 圆角 | 阴影 | 内边距 |
|------|------|------|--------|
| 产品卡片 | 8px | 0 1px 4px rgba(0,0,0,0.04) | 16px |
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
- 边框：1px solid #E5E6EB，聚焦 #FF6A00
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
| 主色 | #FF6A00 | #FF851A |
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
  --aliyun-primary: #FF6A00;
  --aliyun-primary-50: #FFF2E6;
  --aliyun-primary-100: #FFD9B3;
  --aliyun-primary-200: #FFBF80;
  --aliyun-primary-300: #FFA64D;
  --aliyun-primary-400: #FF851A;
  --aliyun-primary-500: #FF6A00;
  --aliyun-primary-600: #E05A00;
  --aliyun-primary-700: #B84D00;
  --aliyun-primary-800: #8F3B00;
  --aliyun-primary-900: #6B2D00;
  --aliyun-success: #00B42A;
  --aliyun-warning: #FF7D00;
  --aliyun-error: #F53F3F;
  --aliyun-text-title: #1D2129;
  --aliyun-text-body: #4E5969;
  --aliyun-text-secondary: #86909C;
  --aliyun-text-placeholder: #C9CDD4;
  --aliyun-border: #E5E6EB;
  --aliyun-bg-page: #F7F8FA;
  --aliyun-bg-card: #FFFFFF;
  --aliyun-radius-sm: 4px;
  --aliyun-radius-md: 8px;
  --aliyun-radius-lg: 12px;
  --aliyun-radius-xl: 16px;
  --aliyun-spacing-xs: 4px;
  --aliyun-spacing-sm: 8px;
  --aliyun-spacing-md: 12px;
  --aliyun-spacing-lg: 16px;
  --aliyun-spacing-xl: 24px;
  --aliyun-spacing-2xl: 32px;
}
```