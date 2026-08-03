# 语雀 设计规范

> 知识绿·文档协作·知识管理 | 主色：#25B864

---

## 一、设计价值观与原则

**价值观**：文档协作·知识管理·优雅写作
**设计原则**：
- 知识专注：绿色传递成长与知识，编辑区极简
- 优雅写作：Markdown优先，排版精致
- 知识图谱：文档关联、标签体系可视化
- 安静创作：减少干扰元素，沉浸式编辑

## 二、配色体系

### 品牌主色色板
| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | #E8F8EF | 主色极浅背景 |
| 100 | #B8E8CC | 主色浅背景 |
| 200 | #80D4A6 | 主色浅色标签 |
| 300 | #4DBF80 | 主色辅助高亮 |
| 400 | #33C870 | 主色悬浮态 |
| 500 | #25B864 | **品牌主色** |
| 600 | #1E9C54 | 主色按压态 |
| 700 | #178044 | 主色深色 |
| 800 | #106434 | 主色极深 |
| 900 | #0A4C26 | 主色最深 |

### 功能色
| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | #00B42A | 保存成功、发布完成 |
| 警告 | #FF7D00 | 权限变更、存储空间 |
| 错误 | #F53F3F | 保存失败、网络异常 |
| 信息 | #25B864 | 引导提示（复用主色） |

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
- 主色渐变：`linear-gradient(135deg, #25B864, #4DBF80)`
- 知识渐变：`linear-gradient(90deg, #25B864, #7B67EE)`

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
| 主要按钮 | 36px | 8px | 14px/500 | #25B864 |
| 次要按钮 | 32px | 8px | 14px/500 | #E8F8EF |
| 文字按钮 | — | — | 14px/500 | transparent |
| 标签按钮 | 24px | 4px | 12px/500 | #E8F8EF |

### 卡片
| 类型 | 圆角 | 阴影 | 内边距 |
|------|------|------|--------|
| 文档卡片 | 8px | 0 1px 4px rgba(0,0,0,0.04) | 16px |
| 知识库卡片 | 12px | 0 2px 8px rgba(0,0,0,0.06) | 16px |
| 信息卡片 | 8px | 0 1px 4px rgba(0,0,0,0.04) | 16px |

### 导航栏
- 高度：48px，背景 #FFFFFF
- 标题字号：16px/700，颜色 #1D2129
- 侧边栏宽度：260px

### 弹窗
- 圆角：12px，遮罩 rgba(0,0,0,0.4)
- 标题字号：16px/700，内容 14px/400
- 按钮高度：36px

### 输入框
- 高度：36px，圆角 8px
- 边框：1px solid #E5E6EB，聚焦 #25B864
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
| 主色 | #25B864 | #4DBF80 |
| 标题文字 | #1D2129 | #F5F5F5 |
| 正文文字 | #4E5969 | #C9CDD4 |
| 辅助文字 | #86909C | #6B7785 |
| 边框 | #E5E6EB | #3A3A3A |
| 分割线 | #F2F3F5 | #2E2E2E |

## 八、设计禁忌

- ✅ Do：编辑区使用纯白背景，无干扰
- ✅ Do：文档标题使用大字号+粗体
- ❌ Don't：禁止编辑区使用彩色背景
- ❌ Don't：禁止文档列表缺少更新时间
- ❌ Don't：禁止使用红色作为主CTA
- ❌ Don't：禁止知识库缺少文档数量标识

## 九、CSS变量快速参考

```css
:root {
  --yuque-primary: #25B864;
  --yuque-primary-50: #E8F8EF;
  --yuque-primary-100: #B8E8CC;
  --yuque-primary-200: #80D4A6;
  --yuque-primary-300: #4DBF80;
  --yuque-primary-400: #33C870;
  --yuque-primary-500: #25B864;
  --yuque-primary-600: #1E9C54;
  --yuque-primary-700: #178044;
  --yuque-primary-800: #106434;
  --yuque-primary-900: #0A4C26;
  --yuque-success: #00B42A;
  --yuque-warning: #FF7D00;
  --yuque-error: #F53F3F;
  --yuque-text-title: #1D2129;
  --yuque-text-body: #4E5969;
  --yuque-text-secondary: #86909C;
  --yuque-text-placeholder: #C9CDD4;
  --yuque-border: #E5E6EB;
  --yuque-bg-page: #F7F8FA;
  --yuque-bg-card: #FFFFFF;
  --yuque-radius-sm: 4px;
  --yuque-radius-md: 8px;
  --yuque-radius-lg: 12px;
  --yuque-radius-xl: 16px;
  --yuque-spacing-xs: 4px;
  --yuque-spacing-sm: 8px;
  --yuque-spacing-md: 12px;
  --yuque-spacing-lg: 16px;
  --yuque-spacing-xl: 24px;
  --yuque-spacing-2xl: 32px;
}
```