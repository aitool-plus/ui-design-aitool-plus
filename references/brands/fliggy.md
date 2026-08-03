# 飞猪 设计规范

> 旅行橙黄·旅行就上飞猪·全球畅游 | 主色：#FF8C00

---

## 一、设计价值观与原则

**价值观**：全球畅游·旅行无忧·说走就走
**设计原则**：
- 旅行感：橙黄色传递阳光与冒险，图片展示目的地美景
- 价格透明：机票酒店价格一目了然，无隐藏费用
- 快速预订：搜索-选择-支付3步完成
- 信任保障：退改政策、保险标识始终可见

## 二、配色体系

### 品牌主色色板
| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | #FFF4E6 | 主色极浅背景 |
| 100 | #FFE4C2 | 主色浅背景 |
| 200 | #FFCC85 | 主色浅色标签 |
| 300 | #FFB34D | 主色辅助高亮 |
| 400 | #FFA01A | 主色悬浮态 |
| 500 | #FF8C00 | **品牌主色** |
| 600 | #E07800 | 主色按压态 |
| 700 | #B86000 | 主色深色 |
| 800 | #8F4A00 | 主色极深 |
| 900 | #6B3800 | 主色最深 |

### 功能色
| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | #00B42A | 预订成功、出票完成 |
| 警告 | #FF7D00 | 价格波动、即将售罄 |
| 错误 | #F53F3F | 预订失败、支付异常 |
| 信息 | #FF8C00 | 引导提示（复用主色） |

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
- 主色渐变：`linear-gradient(135deg, #FF8C00, #FFB34D)`
- 旅行渐变：`linear-gradient(90deg, #FF8C00, #0097FF)`

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
| Bold | 700 | 页面标题、价格 |

## 四、组件设计规范

### 按钮
| 类型 | 高度 | 圆角 | 字号 | 背景色 |
|------|------|------|------|--------|
| 主要按钮 | 44px | 22px | 16px/500 | #FF8C00 |
| 次要按钮 | 40px | 20px | 14px/500 | #FFF4E6 |
| 文字按钮 | — | — | 14px/500 | transparent |
| 标签按钮 | 28px | 14px | 12px/500 | #FFF4E6 |

### 卡片
| 类型 | 圆角 | 阴影 | 内边距 |
|------|------|------|--------|
| 机票卡片 | 12px | 0 2px 12px rgba(0,0,0,0.08) | 12px |
| 酒店卡片 | 12px | 0 2px 12px rgba(0,0,0,0.08) | 12px |
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
- 边框：1px solid #E5E6EB，聚焦 #FF8C00
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
| 日历切换 | 200ms | ease-in-out |
| 骨架屏闪烁 | 1.5s | ease-in-out (loop) |

## 七、暗色模式规范

| 元素 | 亮色 | 暗色 |
|------|------|------|
| 页面背景 | #F7F8FA | #0D0D0D |
| 卡片背景 | #FFFFFF | #1A1A1A |
| 主色 | #FF8C00 | #FFB34D |
| 标题文字 | #1D2129 | #F5F5F5 |
| 正文文字 | #4E5969 | #C9CDD4 |
| 辅助文字 | #86909C | #6B7785 |
| 边框 | #E5E6EB | #2E2E2E |
| 分割线 | #F2F3F5 | #232323 |

## 八、设计禁忌

- ✅ Do：目的地图片使用16:9或3:2比例
- ✅ Do：价格使用Bold字重，主色或深色
- ❌ Don't：禁止价格使用灰色或小字号
- ❌ Don't：禁止机票卡片缺少出发/到达时间
- ❌ Don't：禁止使用蓝色作为主CTA（与橙色冲突）
- ❌ Don't：禁止退改政策信息隐藏在二级页面

## 九、CSS变量快速参考

```css
:root {
  --fliggy-primary: #FF8C00;
  --fliggy-primary-50: #FFF4E6;
  --fliggy-primary-100: #FFE4C2;
  --fliggy-primary-200: #FFCC85;
  --fliggy-primary-300: #FFB34D;
  --fliggy-primary-400: #FFA01A;
  --fliggy-primary-500: #FF8C00;
  --fliggy-primary-600: #E07800;
  --fliggy-primary-700: #B86000;
  --fliggy-primary-800: #8F4A00;
  --fliggy-primary-900: #6B3800;
  --fliggy-success: #00B42A;
  --fliggy-warning: #FF7D00;
  --fliggy-error: #F53F3F;
  --fliggy-text-title: #1D2129;
  --fliggy-text-body: #4E5969;
  --fliggy-text-secondary: #86909C;
  --fliggy-text-placeholder: #C9CDD4;
  --fliggy-border: #E5E6EB;
  --fliggy-bg-page: #F7F8FA;
  --fliggy-bg-card: #FFFFFF;
  --fliggy-radius-sm: 4px;
  --fliggy-radius-md: 8px;
  --fliggy-radius-lg: 12px;
  --fliggy-radius-xl: 16px;
  --fliggy-spacing-xs: 4px;
  --fliggy-spacing-sm: 8px;
  --fliggy-spacing-md: 12px;
  --fliggy-spacing-lg: 16px;
  --fliggy-spacing-xl: 24px;
  --fliggy-spacing-2xl: 32px;
}
```