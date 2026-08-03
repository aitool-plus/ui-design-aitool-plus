# QQ音乐 设计规范

> 听歌绿·听我想听·音乐生活 | 主色：#31C27C

---

## 一、设计价值观与原则

**价值观**：听歌绿·听我想听·音乐生活
**设计原则**：
- 内容核心：听歌绿 音乐生活 海量曲库[0]为核心视觉驱动力
- 用户体验：降低使用门槛，3步完成核心操作
- 社区氛围：鼓励互动、分享、参与
- 品牌辨识：主色贯穿全场景，视觉统一

## 二、配色体系

### 品牌主色色板
| 色阶 | 色值 | 用途 |
|------|------|------|
| 50 | #E8F8F0 | 主色极浅背景 |
| 100 | #B8EACC | 主色浅背景 |
| 200 | #80DAA8 | 主色浅色标签 |
| 300 | #4DC884 | 主色辅助高亮 |
| 400 | #33BE6E | 主色悬浮态 |
| 500 | #31C27C | **品牌主色** |
| 600 | #28A468 | 主色按压态 |
| 700 | #1E8A56 | 主色深色 |
| 800 | #147044 | 主色极深 |
| 900 | #0A5632 | 主色最深 |

### 功能色
| 类型 | 色值 | 用途 |
|------|------|------|
| 成功 | #00B42A | 操作成功 |
| 警告 | #FF7D00 | 提醒注意 |
| 错误 | #F53F3F | 操作失败 |
| 信息 | #31C27C | 引导提示 |

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
- 主色渐变：`linear-gradient(135deg, #31C27C, #33BE6E)`
- 功能渐变：`linear-gradient(90deg, #31C27C, #00B42A)`

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
| 主要按钮 | 44px | 22px | 16px/500 | #31C27C |
| 次要按钮 | 40px | 20px | 14px/500 | #E8F8F0 |
| 文字按钮 | — | — | 14px/500 | transparent |
| 标签按钮 | 28px | 14px | 12px/500 | #E8F8F0 |

### 卡片
| 类型 | 圆角 | 阴影 | 内边距 |
|------|------|------|--------|
| 内容卡片 | 12px | 0 2px 12px rgba(0,0,0,0.08) | 12px |
| 互动卡片 | 8px | 0 1px 6px rgba(0,0,0,0.06) | 16px |
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
- 边框：1px solid #E5E6EB，聚焦 #31C27C
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
| 列表加载 | 200ms | ease-in-out |
| 骨架屏闪烁 | 1.5s | ease-in-out (loop) |

## 七、暗色模式规范

| 元素 | 亮色 | 暗色 |
|------|------|------|
| 页面背景 | #F7F8FA | #0D0D0D |
| 卡片背景 | #FFFFFF | #1A1A1A |
| 主色 | #31C27C | #33BE6E |
| 标题文字 | #1D2129 | #F5F5F5 |
| 正文文字 | #4E5969 | #C9CDD4 |
| 辅助文字 | #86909C | #6B7785 |
| 边框 | #E5E6EB | #2E2E2E |
| 分割线 | #F2F3F5 | #232323 |

## 八、设计禁忌

- ✅ Do：核心交互元素使用主色强调
- ✅ Do：内容卡片使用圆角≥8px
- ❌ Don't：禁止核心操作使用灰色或低对比度
- ❌ Don't：禁止内容卡片缺少关键信息标识
- ❌ Don't：禁止使用与主色冲突的强调色
- ❌ Don't：禁止图片使用直角裁切

## 九、CSS变量快速参考

``css
:root {
  --qqmusic-primary: #31C27C;
  --qqmusic-primary-50: #E8F8F0;
  --qqmusic-primary-100: #B8EACC;
  --qqmusic-primary-200: #80DAA8;
  --qqmusic-primary-300: #4DC884;
  --qqmusic-primary-400: #33BE6E;
  --qqmusic-primary-500: #31C27C;
  --qqmusic-primary-600: #28A468;
  --qqmusic-primary-700: #1E8A56;
  --qqmusic-primary-800: #147044;
  --qqmusic-primary-900: #0A5632;
  --qqmusic-success: #00B42A;
  --qqmusic-warning: #FF7D00;
  --qqmusic-error: #F53F3F;
  --qqmusic-text-title: #1D2129;
  --qqmusic-text-body: #4E5969;
  --qqmusic-text-secondary: #86909C;
  --qqmusic-text-placeholder: #C9CDD4;
  --qqmusic-border: #E5E6EB;
  --qqmusic-bg-page: #F7F8FA;
  --qqmusic-bg-card: #FFFFFF;
  --qqmusic-radius-sm: 4px;
  --qqmusic-radius-md: 8px;
  --qqmusic-radius-lg: 12px;
  --qqmusic-radius-xl: 16px;
  --qqmusic-spacing-xs: 4px;
  --qqmusic-spacing-sm: 8px;
  --qqmusic-spacing-md: 12px;
  --qqmusic-spacing-lg: 16px;
  --qqmusic-spacing-xl: 24px;
  --qqmusic-spacing-2xl: 32px;
}
``

