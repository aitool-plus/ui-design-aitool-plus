# 创客贴 设计规范

> 设计橙·在线设计·一键出图 | 主色：#FF6B35

---

## 一、设计价值观与原则

**价值观**：在线设计·一键出图·人人都是设计师
**设计原则**：
- 设计民主：降低设计门槛，模板驱动快速出图
- 创意活力：橙色传递创意与活力，画布为核心
- 所见即所得：编辑区实时预览，操作即时反馈
- 模板优先：海量模板降低创作门槛

## 二、配色体系

### 品牌主色色板
| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | #FFF2EB | 主色极浅背景 |
| 100 | #FFD9C7 | 主色浅背景 |
| 200 | #FFB89E | 主色浅色标签 |
| 300 | #FF9775 | 主色辅助高亮 |
| 400 | #FF8055 | 主色悬浮态 |
| 500 | #FF6B35 | **品牌主色** |
| 600 | #E05A28 | 主色按压态 |
| 700 | #B8491E | 主色深色 |
| 800 | #8F3815 | 主色极深 |
| 900 | #6B2A0E | 主色最深 |

### 功能色
| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | #00B42A | 导出成功、保存完成 |
| 警告 | #FF7D00 | 存储空间、会员到期 |
| 错误 | #F53F3F | 导出失败、网络异常 |
| 信息 | #FF6B35 | 引导提示（复用主色） |

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
- 主色渐变：`linear-gradient(135deg, #FF6B35, #FF9775)`
- 创意渐变：`linear-gradient(90deg, #FF6B35, #7B67EE)`

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
| 主要按钮 | 36px | 8px | 14px/500 | #FF6B35 |
| 次要按钮 | 32px | 8px | 14px/500 | #FFF2EB |
| 文字按钮 | — | — | 14px/500 | transparent |
| 标签按钮 | 24px | 4px | 12px/500 | #FFF2EB |

### 卡片
| 类型 | 圆角 | 阴影 | 内边距 |
|------|------|------|--------|
| 模板卡片 | 8px | 0 2px 8px rgba(0,0,0,0.06) | 8px |
| 作品卡片 | 8px | 0 1px 4px rgba(0,0,0,0.04) | 12px |
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
- 边框：1px solid #E5E6EB，聚焦 #FF6B35
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
| 画布缩放 | 150ms | ease-out |
| 骨架屏闪烁 | 1.5s | ease-in-out (loop) |

## 七、暗色模式规范

| 元素 | 亮色 | 暗色 |
|------|------|------|
| 页面背景 | #F7F8FA | #1A1A1A |
| 卡片背景 | #FFFFFF | #2A2A2A |
| 主色 | #FF6B35 | #FF9775 |
| 标题文字 | #1D2129 | #F5F5F5 |
| 正文文字 | #4E5969 | #C9CDD4 |
| 辅助文字 | #86909C | #6B7785 |
| 边框 | #E5E6EB | #3A3A3A |
| 分割线 | #F2F3F5 | #2E2E2E |

## 八、设计禁忌

- ✅ Do：模板缩略图使用真实预览
- ✅ Do：画布编辑区使用灰色棋盘格背景
- ❌ Don't：禁止模板缩略图使用占位图
- ❌ Don't：禁止画布编辑区使用白色背景（与白色元素混淆）
- ❌ Don't：禁止使用蓝色作为主CTA
- ❌ Don't：禁止导出按钮使用非主色

## 九、CSS变量快速参考

```css
:root {
  --canvacn-primary: #FF6B35;
  --canvacn-primary-50: #FFF2EB;
  --canvacn-primary-100: #FFD9C7;
  --canvacn-primary-200: #FFB89E;
  --canvacn-primary-300: #FF9775;
  --canvacn-primary-400: #FF8055;
  --canvacn-primary-500: #FF6B35;
  --canvacn-primary-600: #E05A28;
  --canvacn-primary-700: #B8491E;
  --canvacn-primary-800: #8F3815;
  --canvacn-primary-900: #6B2A0E;
  --canvacn-success: #00B42A;
  --canvacn-warning: #FF7D00;
  --canvacn-error: #F53F3F;
  --canvacn-text-title: #1D2129;
  --canvacn-text-body: #4E5969;
  --canvacn-text-secondary: #86909C;
  --canvacn-text-placeholder: #C9CDD4;
  --canvacn-border: #E5E6EB;
  --canvacn-bg-page: #F7F8FA;
  --canvacn-bg-card: #FFFFFF;
  --canvacn-radius-sm: 4px;
  --canvacn-radius-md: 8px;
  --canvacn-radius-lg: 12px;
  --canvacn-radius-xl: 16px;
  --canvacn-spacing-xs: 4px;
  --canvacn-spacing-sm: 8px;
  --canvacn-spacing-md: 12px;
  --canvacn-spacing-lg: 16px;
  --canvacn-spacing-xl: 24px;
  --canvacn-spacing-2xl: 32px;
}
```