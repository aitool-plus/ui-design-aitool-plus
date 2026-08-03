# 大众点评 设计规范

> 点评橙·真实评价·生活指南 | 主色：#FF6633

---

## 一、设计价值观与原则

**价值观**：真实评价·生活指南·发现好店
**设计原则**：
- 真实可信：评价内容为视觉核心，星级评分始终可见
- 生活指南：橙色传递温暖与活力，引导探索周边
- 评价优先：用户评价、评分、图片占据核心视觉位置
- 本地连接：距离、地址、营业状态信息清晰

## 二、配色体系

### 品牌主色色板
| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | #FFF2EB | 主色极浅背景 |
| 100 | #FFD9C7 | 主色浅背景 |
| 200 | #FFB299 | 主色浅色标签 |
| 300 | #FF8C66 | 主色辅助高亮 |
| 400 | #FF774D | 主色悬浮态 |
| 500 | #FF6633 | **品牌主色** |
| 600 | #E0551A | 主色按压态 |
| 700 | #B84414 | 主色深色 |
| 800 | #8F340E | 主色极深 |
| 900 | #6B270A | 主色最深 |

### 功能色
| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | #00B42A | 预约成功、营业中 |
| 警告 | #FF7D00 | 即将打烊、排队中 |
| 错误 | #F53F3F | 预约失败、已休息 |
| 信息 | #FF6633 | 引导提示（复用主色） |

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
- 主色渐变：`linear-gradient(135deg, #FF6633, #FF8C66)`
- 评分渐变：`linear-gradient(90deg, #FF6633, #FFD700)`

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
| Bold | 700 | 页面标题、评分 |

## 四、组件设计规范

### 按钮
| 类型 | 高度 | 圆角 | 字号 | 背景色 |
|------|------|------|------|--------|
| 主要按钮 | 44px | 22px | 16px/500 | #FF6633 |
| 次要按钮 | 40px | 20px | 14px/500 | #FFF2EB |
| 文字按钮 | — | — | 14px/500 | transparent |
| 标签按钮 | 28px | 14px | 12px/500 | #FFF2EB |

### 卡片
| 类型 | 圆角 | 阴影 | 内边距 |
|------|------|------|--------|
| 商家卡片 | 12px | 0 2px 12px rgba(0,0,0,0.08) | 12px |
| 评价卡片 | 12px | 0 1px 6px rgba(0,0,0,0.06) | 16px |
| 信息卡片 | 8px | 0 1px 4px rgba(0,0,0,0.04) | 16px |

### 导航栏
- 高度：48px，背景 #FFFFFF
- 标题字号：18px/700，颜色 #1D2129
- 返回图标：24px，颜色 #4E5969

### 弹窗
- 圆角：16px，遮罩 rgba(0,0,0,0.5)
- 标题字号：18px/700，内容 14px/400
- 按钮高度：44px

### 输入框
- 高度：40px，圆角 8px
- 边框：1px solid #E5E6EB，聚焦 #FF6633
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
| md | 8px | 输入框、小卡片 |
| lg | 12px | 卡片、弹窗 |
| xl | 16px | 大弹窗、底部面板 |
| full | 9999px | 胶囊按钮、头像 |

## 六、动效规范

| 场景 | 时长 | 缓动函数 |
|------|------|----------|
| 按钮反馈 | 150ms | ease-out |
| 页面切换 | 300ms | cubic-bezier(0.25,0.1,0.25,1) |
| 弹窗弹出 | 250ms | cubic-bezier(0.34,1.56,0.64,1) |
| 星级评分 | 200ms | ease-in-out |
| 骨架屏闪烁 | 1.5s | ease-in-out (loop) |

## 七、暗色模式规范

| 元素 | 亮色 | 暗色 |
|------|------|------|
| 页面背景 | #F7F8FA | #0D0D0D |
| 卡片背景 | #FFFFFF | #1A1A1A |
| 主色 | #FF6633 | #FF8C66 |
| 标题文字 | #1D2129 | #F5F5F5 |
| 正文文字 | #4E5969 | #C9CDD4 |
| 辅助文字 | #86909C | #6B7785 |
| 边框 | #E5E6EB | #2E2E2E |
| 分割线 | #F2F3F5 | #232323 |

## 八、设计禁忌

- ✅ Do：评分星级使用主色填充，空星使用浅灰
- ✅ Do：评价内容字号≥14px，确保可读性
- ❌ Don't：禁止评分星级使用非主色填充
- ❌ Don't：禁止商家卡片缺少评分/距离信息
- ❌ Don't：禁止评价文字字号小于12px
- ❌ Don't：禁止使用蓝色作为主CTA（与橙色冲突）

## 九、CSS变量快速参考

```css
:root {
  --dianping-primary: #FF6633;
  --dianping-primary-50: #FFF2EB;
  --dianping-primary-100: #FFD9C7;
  --dianping-primary-200: #FFB299;
  --dianping-primary-300: #FF8C66;
  --dianping-primary-400: #FF774D;
  --dianping-primary-500: #FF6633;
  --dianping-primary-600: #E0551A;
  --dianping-primary-700: #B84414;
  --dianping-primary-800: #8F340E;
  --dianping-primary-900: #6B270A;
  --dianping-success: #00B42A;
  --dianping-warning: #FF7D00;
  --dianping-error: #F53F3F;
  --dianping-text-title: #1D2129;
  --dianping-text-body: #4E5969;
  --dianping-text-secondary: #86909C;
  --dianping-text-placeholder: #C9CDD4;
  --dianping-border: #E5E6EB;
  --dianping-bg-page: #F7F8FA;
  --dianping-bg-card: #FFFFFF;
  --dianping-radius-sm: 4px;
  --dianping-radius-md: 8px;
  --dianping-radius-lg: 12px;
  --dianping-radius-xl: 16px;
  --dianping-spacing-xs: 4px;
  --dianping-spacing-sm: 8px;
  --dianping-spacing-md: 12px;
  --dianping-spacing-lg: 16px;
  --dianping-spacing-xl: 24px;
  --dianping-spacing-2xl: 32px;
}
```
