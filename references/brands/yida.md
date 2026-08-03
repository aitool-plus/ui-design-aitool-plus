# 宜搭 设计规范

> 低代码蓝·应用搭建·敏捷开发 | 主色：#1677FF

---

## 一、设计价值观与原则

**价值观**：低代码·应用搭建·敏捷开发
**设计原则**：
- 低代码优先：拖拽搭建，减少代码编写
- 敏捷开发：快速迭代，所见即所得
- 配置驱动：属性面板、组件配置为核心交互
- 开发者友好：兼顾低代码与Pro Code

## 二、配色体系

### 品牌主色色板
| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | #E8F3FF | 主色极浅背景 |
| 100 | #BEDAFF | 主色浅背景 |
| 200 | #94BFFF | 主色浅色标签 |
| 300 | #6AA3FF | 主色辅助高亮 |
| 400 | #4080FF | 主色悬浮态 |
| 500 | #1677FF | **品牌主色** |
| 600 | #0E5FD8 | 主色按压态 |
| 700 | #0A47B0 | 主色深色 |
| 800 | #073388 | 主色极深 |
| 900 | #042460 | 主色最深 |

### 功能色
| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | #00B42A | 发布成功、保存完成 |
| 警告 | #FF7D00 | 配置缺失、权限不足 |
| 错误 | #F53F3F | 发布失败、语法错误 |
| 信息 | #1677FF | 引导提示（复用主色） |

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
- 主色渐变：`linear-gradient(135deg, #1677FF, #4080FF)`
- 低代码渐变：`linear-gradient(90deg, #1677FF, #7B67EE)`

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
| 主要按钮 | 36px | 8px | 14px/500 | #1677FF |
| 次要按钮 | 32px | 8px | 14px/500 | #E8F3FF |
| 文字按钮 | — | — | 14px/500 | transparent |
| 标签按钮 | 24px | 4px | 12px/500 | #E8F3FF |

### 卡片
| 类型 | 圆角 | 阴影 | 内边距 |
|------|------|------|--------|
| 组件卡片 | 8px | 0 1px 4px rgba(0,0,0,0.04) | 12px |
| 应用卡片 | 12px | 0 2px 8px rgba(0,0,0,0.06) | 16px |
| 信息卡片 | 8px | 0 1px 4px rgba(0,0,0,0.04) | 16px |

### 导航栏
- 高度：48px，背景 #FFFFFF
- 标题字号：16px/700，颜色 #1D2129
- 属性面板宽度：280px

### 弹窗
- 圆角：12px，遮罩 rgba(0,0,0,0.4)
- 标题字号：16px/700，内容 14px/400
-400
- 按钮高度：36px

### 输入框
- 高度：36px，圆角 8px
- 边框：1px solid #E5E6EB，聚焦 #1677FF
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
| 拖拽放置 | 150ms | ease-out |
| 骨架屏闪烁 | 1.5s | ease-in-out (loop) |

## 七、暗色模式规范

| 元素 | 亮色 | 暗色 |
|------|------|------|
| 页面背景 | #F7F8FA | #1A1A1A |
| 卡片背景 | #FFFFFF | #2A2A2A |
| 主色 | #1677FF | #4080FF |
| 标题文字 | #1D2129 | #F5F5F5 |
| 正文文字 | #4E5969 | #C9CDD4 |
| 辅助文字 | #86909C | #6B7785 |
| 边框 | #E5E6EB | #3A3A3A |
| 分割线 | #F2F3F5 | #2E2E2E |

## 八、设计禁忌

- ✅ Do：组件拖拽使用虚线占位提示
- ✅ Do：属性面板使用分组折叠
- ❌ Don't：禁止拖拽区域缺少视觉提示
- ❌ Don't：禁止属性面板信息过载无分组
- ❌ Don't：禁止使用紫色作为主CTA
- ❌ Don't：禁止画布缺少网格参考线

## 九、CSS变量快速参考

```css
:root {
  --yida-primary: #1677FF;
  --yida-primary-50: #E8F3FF;
  --yida-primary-100: #BEDAFF;
  --yida-primary-200: #94BFFF;
  --yida-primary-300: #6AA3FF;
  --yida-primary-400: #4080FF;
  --yida-primary-500: #1677FF;
  --yida-primary-600: #0E5FD8;
  --yida-primary-700: #0A47B0;
  --yida-primary-800: #073388;
  --yida-primary-900: #042460;
  --yida-success: #00B42A;
  --yida-warning: #FF7D00;
  --yida-error: #F53F3F;
  --yida-text-title: #1D2129;
  --yida-text-body: #4E5969;
  --yida-text-secondary: #86909C;
  --yida-text-placeholder: #C9CDD4;
  --yida-border: #E5E6EB;
  --yida-bg-page: #F7F8FA;
  --yida-bg-card: #FFFFFF;
  --yida-radius-sm: 4px;
  --yida-radius-md: 8px;
  --yida-radius-lg: 12px;
  --yida-radius-xl: 16px;
  --yida-spacing-xs: 4px;
  --yida-spacing-sm: 8px;
  --yida-spacing-md: 12px;
  --yida-spacing-lg: 16px;
  --yida-spacing-xl: 24px;
  --yida-spacing-2xl: 32px;
}
```