# WPS 设计规范

> 办公蓝·智慧办公·多端协同 | 主色：#2B5FD9

---

## 一、设计价值观与原则

**价值观**：智慧办公·多端协同·人人用得起
**设计原则**：
- 办公专业：蓝色传递专业与可靠，工具栏功能清晰
- 多端一致：PC、移动端、Web视觉统一
- 效率工具：快捷键、模板、AI辅助提升效率
- 兼容优先：Office格式完美兼容

## 二、配色体系

### 品牌主色色板
| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | #EBF0FF | 主色极浅背景 |
| 100 | #C7D4F5 | 主色浅背景 |
| 200 | #9FB3EB | 主色浅色标签 |
| 300 | #7792E0 | 主色辅助高亮 |
| 400 | #5075D6 | 主色悬浮态 |
| 500 | #2B5FD9 | **品牌主色** |
| 600 | #224DB8 | 主色按压态 |
| 700 | #1A3D97 | 主色深色 |
| 800 | #122D76 | 主色极深 |
| 900 | #0B1E55 | 主色最深 |

### 功能色
| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | #00B42A | 保存成功、分享完成 |
| 警告 | #FF7D00 | 存储空间、会员到期 |
| 错误 | #F53F3F | 保存失败、格式错误 |
| 信息 | #2B5FD9 | 引导提示（复用主色） |

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
- 主色渐变：`linear-gradient(135deg, #2B5FD9, #5075D6)`
- 办公渐变：`linear-gradient(90deg, #2B5FD9, #00B42A)`

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
| 主要按钮 | 36px | 8px | 14px/500 | #2B5FD9 |
| 次要按钮 | 32px | 8px | 14px/500 | #EBF0FF |
| 文字按钮 | — | — | 14px/500 | transparent |
| 标签按钮 | 24px | 4px | 12px/500 | #EBF0FF |

### 卡片
| 类型 | 圆角 | 阴影 | 内边距 |
|------|------|------|--------|
| 文档卡片 | 8px | 0 1px 4px rgba(0,0,0,0.04) | 16px |
| 模板卡片 | 8px | 0 2px 8px rgba(0,0,0,0.06) | 12px |
| 信息卡片 | 8px | 0 1px 4px rgba(0,0,0,0.04) | 16px |

### 导航栏
- 高度：48px，背景 #FFFFFF
- 标题字号：16px/700，颜色 #1D2129
- 工具栏高度：40px

### 弹窗
- 圆角：12px，遮罩 rgba(0,0,0,0.4)
- 标题字号：16px/700，内容 14px/400
- 按钮高度：36px

### 输入框
- 高度：36px，圆角 8px
- 边框：1px solid #E5E6EB，聚焦 #2B5FD9
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
| 工具栏展开 | 150ms | ease-in-out |
| 骨架屏闪烁 | 1.5s | ease-in-out (loop) |

## 七、暗色模式规范

| 元素 | 亮色 | 暗色 |
|------|------|------|
| 页面背景 | #F7F8FA | #1A1A1A |
| 卡片背景 | #FFFFFF | #2A2A2A |
| 主色 | #2B5FD9 | #5075D6 |
| 标题文字 | #1D2129 | #F5F5F5 |
| 正文文字 | #4E5969 | #C9CDD4 |
| 辅助文字 | #86909C | #6B7785 |
| 边框 | #E5E6EB | #3A3A3A |
| 分割线 | #F2F3F5 | #2E2E2E |

## 八、设计禁忌

- ✅ Do：工具栏图标使用24px，间距8px
- ✅ Do：文档编辑区使用纯白背景
- ❌ Don't：禁止工具栏图标间距不一致
- ❌ Don't：禁止编辑区使用彩色背景
- ❌ Don't：禁止使用红色作为主CTA
- ❌ Don't：禁止文档列表缺少修改时间

## 九、CSS变量快速参考

```css
:root {
  --wps-primary: #2B5FD9;
  --wps-primary-50: #EBF0FF;
  --wps-primary-100: #C7D4F5;
  --wps-primary-200: #9FB3EB;
  --wps-primary-300: #7792E0;
  --wps-primary-400: #5075D6;
  --wps-primary-500: #2B5FD9;
  --wps-primary-600: #224DB8;
  --wps-primary-700: #1A3D97;
  --wps-primary-800: #122D76;
  --wps-primary-900: #0B1E55;
  --wps-success: #00B42A;
  --wps-warning: #FF7D00;
  --wps-error: #F53F3F;
  --wps-text-title: #1D2129;
  --wps-text-body: #4E5969;
  --wps-text-secondary: #86909C;
  --wps-text-placeholder: #C9CDD4;
  --wps-border: #E5E6EB;
  --wps-bg-page: #F7F8FA;
  --wps-bg-card: #FFFFFF;
  --wps-radius-sm: 4px;
  --wps-radius-md: 8px;
  --wps-radius-lg: 12px;
  --wps-radius-xl: 16px;
  --wps-spacing-xs: 4px;
  --wps-spacing-sm: 8px;
  --wps-spacing-md: 12px;
  --wps-spacing-lg: 16px;
  --wps-spacing-xl: 24px;
  --wps-spacing-2xl: 32px;
}
```