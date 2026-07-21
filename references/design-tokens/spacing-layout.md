> @author aitool.plus

# 间距与布局体系

## 概述

本间距与布局体系覆盖11大操作系统平台，包含基础间距单位、间距阶梯、边距规范、栅格系统、响应式断点和安全区域规范。

---

## 基础间距单位

### 各OS基础网格

| OS平台 | 基础单位 | 网格系统 | 说明 |
|--------|----------|----------|------|
| Apple iOS | 4px | 4px网格 | 所有间距为4px的倍数 |
| Google Android | 4px | 4dp网格 | Material Design标准网格 |
| Samsung One UI | 4px | 4px网格 | 基于Android标准 |
| Huawei HarmonyOS | 4px | 4px网格 | 鸿蒙设计规范 |
| Xiaomi HyperOS | 4px | 4px网格 | 基于Android标准 |
| Honor MagicOS | 4px | 4px网格 | 基于Android标准 |
| OPPO ColorOS | 4px | 4px网格 | 基于Android标准 |
| vivo OriginOS | 4px | 4px网格 | 基于Android标准 |
| Meizu Flyme | 4px | 4px网格 | 基于Android标准 |
| Windows Fluent | 4px | 4px网格 | Fluent Design标准 |
| WeChat WeUI | 4px | 4px网格 | 微信小程序规范 |

---

## 间距阶梯

### 完整间距表（单位：px）

| Token名称 | 数值 | 用途 |
|-----------|------|------|
| space-0 | 0px | 无间距 |
| space-1 | 4px | 最小间距、图标内边距 |
| space-2 | 8px | 紧凑间距、小按钮内边距 |
| space-3 | 12px | 标准间距、列表项内边距 |
| space-4 | 16px | 常用间距、卡片内边距 |
| space-5 | 20px | 中等间距、表单内边距 |
| space-6 | 24px | 较大间距、区块间距 |
| space-8 | 32px | 大间距、模块间距 |
| space-10 | 40px | 更大间距、区域间距 |
| space-12 | 48px | 大模块间距 |
| space-16 | 64px | 超大间距、页面区块间距 |
| space-20 | 80px | 页面级间距 |
| space-24 | 96px | 最大间距、页面分区 |

### 各OS间距阶梯对照

| Token名称 | Apple iOS | Google Android | Samsung One UI | Huawei HarmonyOS | Xiaomi HyperOS | Honor MagicOS | OPPO ColorOS | vivo OriginOS | Meizu Flyme | Windows Fluent | WeChat WeUI |
|-----------|-----------|----------------|----------------|------------------|----------------|---------------|--------------|---------------|-------------|----------------|-------------|
| space-1 | 4px | 4dp | 4px | 4px | 4px | 4px | 4px | 4px | 4px | 4px | 4px |
| space-2 | 8px | 8dp | 8px | 8px | 8px | 8px | 8px | 8px | 8px | 8px | 8px |
| space-3 | 12px | 12dp | 12px | 12px | 12px | 12px | 12px | 12px | 12px | 12px | 12px |
| space-4 | 16px | 16dp | 16px | 16px | 16px | 16px | 16px | 16px | 16px | 16px | 16px |
| space-5 | 20px | 20dp | 20px | 20px | 20px | 20px | 20px | 20px | 20px | 20px | 20px |
| space-6 | 24px | 24dp | 24px | 24px | 24px | 24px | 24px | 24px | 24px | 24px | 24px |
| space-8 | 32px | 32dp | 32px | 32px | 32px | 32px | 32px | 32px | 32px | 32px | 32px |
| space-10 | 40px | 40dp | 40px | 40px | 40px | 40px | 40px | 40px | 40px | 40px | 40px |
| space-12 | 48px | 48dp | 48px | 48px | 48px | 48px | 48px | 48px | 48px | 48px | 48px |
| space-16 | 64px | 64dp | 64px | 64px | 64px | 64px | 64px | 64px | 64px | 64px | 64px |
| space-20 | 80px | 80dp | 80px | 80px | 80px | 80px | 80px | 80px | 80px | 80px | 80px |
| space-24 | 96px | 96dp | 96px | 96px | 96px | 96px | 96px | 96px | 96px | 96px | 96px |

---

## 边距规范

### 页面边距

| 设备类型 | Apple iOS | Google Android | Samsung One UI | Huawei HarmonyOS | Xiaomi HyperOS | Honor MagicOS | OPPO ColorOS | vivo OriginOS | Meizu Flyme | Windows Fluent | WeChat WeUI |
|----------|-----------|----------------|----------------|------------------|----------------|---------------|--------------|---------------|-------------|----------------|-------------|
| 手机 | 16px | 16dp | 16px | 16px | 16px | 16px | 16px | 16px | 16px | 16px | 16px |
| 折叠屏 | 24px | 24dp | 24px | 24px | 24px | 24px | 24px | 24px | 24px | 24px | 24px |
| 平板 | 32px | 32dp | 32px | 32px | 32px | 32px | 32px | 32px | 32px | 32px | 32px |
| 桌面 | 48px | 48dp | 48px | 48px | 48px | 48px | 48px | 48px | 48px | 48px | 48px |

### 内容区边距

| 内容类型 | 手机 | 折叠屏 | 平板 | 桌面 |
|----------|------|--------|------|------|
| 卡片内容 | 16px | 20px | 24px | 32px |
| 列表项 | 16px | 20px | 24px | 32px |
| 表单内容 | 16px | 20px | 24px | 32px |
| 弹窗内容 | 20px | 24px | 32px | 40px |
| 底部操作区 | 16px | 20px | 24px | 32px |

### 组件内边距

| 组件类型 | 水平内边距 | 垂直内边距 |
|----------|-----------|-----------|
| 按钮-小 | 12px | 8px |
| 按钮-中 | 16px | 12px |
| 按钮-大 | 24px | 16px |
| 输入框 | 16px | 12px |
| 卡片 | 16px | 16px |
| 列表项 | 16px | 12px |
| 标签 | 8px | 4px |
| 弹窗 | 20px | 20px |
| 导航栏 | 16px | 12px |
| 底部标签栏 | 0px | 8px |

---

## 栅格系统

### 各OS栅格规范

#### Apple iOS

- 手机：单列布局，内容宽度 = 屏幕宽度 - 32px（左右边距各16px）
- 平板：支持双栏布局，主内容区占 2/3，侧边栏占 1/3
- 桌面：支持三栏布局，侧边栏固定宽度 320px
- 列间距：16px

#### Google Android

- 手机：单列布局，内容宽度 = 屏幕宽度 - 32dp
- 平板：支持双栏布局，主内容区占 60%，侧边栏占 40%
- 桌面：支持三栏布局，侧边栏固定宽度 256dp
- 列间距：16dp

#### Samsung One UI

- 手机：单列布局，内容宽度 = 屏幕宽度 - 32px
- 折叠屏展开：支持双栏布局，比例 1:1
- 平板：支持双栏布局，主内容区占 65%
- 列间距：16px

#### Huawei HarmonyOS

- 手机：单列布局，内容宽度 = 屏幕宽度 - 32px
- 平板：支持双栏布局，主内容区占 62%
- 桌面：支持三栏布局，侧边栏固定宽度 280px
- 列间距：16px

#### Xiaomi HyperOS

- 手机：单列布局，内容宽度 = 屏幕宽度 - 32px
- 平板：支持双栏布局，主内容区占 60%
- 桌面：支持三栏布局
- 列间距：16px

#### Honor MagicOS

- 手机：单列布局，内容宽度 = 屏幕宽度 - 32px
- 平板：支持双栏布局，主内容区占 63%
- 桌面：支持三栏布局
- 列间距：16px

#### OPPO ColorOS

- 手机：单列布局，内容宽度 = 屏幕宽度 - 32px
- 平板：支持双栏布局，主内容区占 60%
- 桌面：支持三栏布局
- 列间距：16px

#### vivo OriginOS

- 手机：单列布局，内容宽度 = 屏幕宽度 - 32px
- 平板：支持双栏布局，主内容区占 62%
- 桌面：支持三栏布局
- 列间距：16px

#### Meizu Flyme

- 手机：单列布局，内容宽度 = 屏幕宽度 - 32px
- 平板：支持双栏布局，主内容区占 60%
- 桌面：支持三栏布局
- 列间距：16px

#### Windows Fluent

- 手机：单列布局，内容宽度 = 屏幕宽度 - 32px
- 平板：支持双栏布局，主内容区占 65%
- 桌面：支持三栏布局，侧边栏固定宽度 280px
- 列间距：16px

#### WeChat WeUI

- 手机：单列布局，内容宽度 = 屏幕宽度 - 32px
- 平板：支持双栏布局，主内容区占 60%
- 桌面：支持双栏布局
- 列间距：16px

---

## 响应式断点

### 断点定义

| 断点名称 | 宽度范围 | 设备类型 | 布局策略 |
|----------|----------|----------|----------|
| xs | 0-374px | 小屏手机 | 单列布局，紧凑间距 |
| sm | 375-428px | 标准手机 | 单列布局，标准间距 |
| md | 429-599px | 大屏手机 | 单列布局，宽松间距 |
| fold | 600-839px | 折叠屏 | 可切换单/双栏布局 |
| lg | 840-1279px | 平板 | 双栏布局，侧边栏可折叠 |
| xl | 1280-1919px | 桌面 | 三栏布局，侧边栏常驻 |
| xxl | 1920px+ | 大屏桌面 | 三栏布局，最大内容宽度 |

### 各断点详细参数

#### xs（0-374px）

- 页面边距：12px
- 内容区边距：12px
- 组件间距：8px
- 字号基准：14px
- 按钮高度：40px
- 输入框高度：40px

#### sm（375-428px）

- 页面边距：16px
- 内容区边距：16px
- 组件间距：12px
- 字号基准：15px（iOS）/ 16px（Android）
- 按钮高度：44px
- 输入框高度：44px

#### md（429-599px）

- 页面边距：20px
- 内容区边距：20px
- 组件间距：16px
- 字号基准：16px
- 按钮高度：48px
- 输入框高度：48px

#### fold（600-839px）

- 页面边距：24px
- 内容区边距：24px
- 组件间距：16px
- 字号基准：16px
- 按钮高度：48px
- 输入框高度：48px
- 折叠态：单列布局
- 展开态：双栏布局

#### lg（840-1279px）

- 页面边距：32px
- 内容区边距：32px
- 组件间距：20px
- 字号基准：16px
- 按钮高度：48px
- 输入框高度：48px
- 布局：双栏，侧边栏宽度 280px

#### xl（1280-1919px）

- 页面边距：48px
- 内容区边距：40px
- 组件间距：24px
- 字号基准：16px
- 按钮高度：48px
- 输入框高度：48px
- 布局：三栏，左侧边栏 280px，右侧边栏 320px
- 最大内容宽度：1200px

#### xxl（1920px+）

- 页面边距：64px
- 内容区边距：48px
- 组件间距：32px
- 字号基准：16px
- 按钮高度：48px
- 输入框高度：48px
- 布局：三栏，内容居中
- 最大内容宽度：1440px

### CSS断点变量

```css
--breakpoint-xs: 0px;
--breakpoint-sm: 375px;
--breakpoint-md: 429px;
--breakpoint-fold: 600px;
--breakpoint-lg: 840px;
--breakpoint-xl: 1280px;
--breakpoint-xxl: 1920px;
```

---

## 安全区域

### 各OS安全区域规范

#### Apple iOS

| 区域 | 数值 | 说明 |
|------|------|------|
| 顶部安全区 | 44px（刘海屏）/ 20px（非刘海屏） | 状态栏+刘海区域 |
| 底部安全区 | 34px（有Home指示器）/ 0px | Home指示器区域 |
| 左右安全区 | 0px | 无圆角屏幕安全区 |
| 圆角安全区 | 上圆角 44px，下圆角 34px | 圆角屏幕内容避让 |

#### Google Android

| 区域 | 数值 | 说明 |
|------|------|------|
| 顶部安全区 | 24dp（状态栏） | 状态栏高度 |
| 底部安全区 | 48dp（导航栏）/ 0dp（手势导航） | 导航栏或手势区域 |
| 左右安全区 | 0dp | 无圆角屏幕安全区 |
| 刘海安全区 | 因设备而异 | 刘海屏内容避让 |

#### Samsung One UI

| 区域 | 数值 | 说明 |
|------|------|------|
| 顶部安全区 | 24px | 状态栏高度 |
| 底部安全区 | 48px（导航栏）/ 0px（手势） | 导航栏或手势区域 |
| 左右安全区 | 0px | 无圆角屏幕安全区 |

#### Huawei HarmonyOS

| 区域 | 数值 | 说明 |
|------|------|------|
| 顶部安全区 | 24px | 状态栏高度 |
| 底部安全区 | 48px（导航栏）/ 0px（手势） | 导航栏或手势区域 |
| 左右安全区 | 0px | 无圆角屏幕安全区 |

#### Xiaomi HyperOS

| 区域 | 数值 | 说明 |
|------|------|------|
| 顶部安全区 | 24px | 状态栏高度 |
| 底部安全区 | 48px（导航栏）/ 0px（手势） | 导航栏或手势区域 |
| 左右安全区 | 0px | 无圆角屏幕安全区 |

#### Honor MagicOS

| 区域 | 数值 | 说明 |
|------|------|------|
| 顶部安全区 | 24px | 状态栏高度 |
| 底部安全区 | 48px（导航栏）/ 0px（手势） | 导航栏或手势区域 |
| 左右安全区 | 0px | 无圆角屏幕安全区 |

#### OPPO ColorOS

| 区域 | 数值 | 说明 |
|------|------|------|
| 顶部安全区 | 24px | 状态栏高度 |
| 底部安全区 | 48px（导航栏）/ 0px（手势） | 导航栏或手势区域 |
| 左右安全区 | 0px | 无圆角屏幕安全区 |

#### vivo OriginOS

| 区域 | 数值 | 说明 |
|------|------|------|
| 顶部安全区 | 24px | 状态栏高度 |
| 底部安全区 | 48px（导航栏）/ 0px（手势） | 导航栏或手势区域 |
| 左右安全区 | 0px | 无圆角屏幕安全区 |

#### Meizu Flyme

| 区域 | 数值 | 说明 |
|------|------|------|
| 顶部安全区 | 24px | 状态栏高度 |
| 底部安全区 | 48px（导航栏）/ 0px（手势） | 导航栏或手势区域 |
| 左右安全区 | 0px | 无圆角屏幕安全区 |

#### Windows Fluent

| 区域 | 数值 | 说明 |
|------|------|------|
| 顶部安全区 | 32px | 标题栏高度 |
| 底部安全区 | 0px | 无底部安全区 |
| 左右安全区 | 0px | 无左右安全区 |
| 窗口边距 | 16px | 窗口内容边距 |

#### WeChat WeUI

| 区域 | 数值 | 说明 |
|------|------|------|
| 顶部安全区 | 20px | 小程序胶囊按钮区域 |
| 底部安全区 | 0px | 无底部安全区 |
| 左右安全区 | 0px | 无左右安全区 |
| 页面边距 | 16px | 小程序页面边距 |

### CSS安全区域变量

```css
/* iOS安全区域 */
--safe-area-top: env(safe-area-inset-top, 0px);
--safe-area-bottom: env(safe-area-inset-bottom, 0px);
--safe-area-left: env(safe-area-inset-left, 0px);
--safe-area-right: env(safe-area-inset-right, 0px);

/* 通用安全区域 */
--safe-area-top-default: 24px;
--safe-area-bottom-default: 0px;
--safe-area-bottom-nav: 48px;
```

---

## 11大平台间距阶梯对照表

### 基准网格与间距阶梯

| 间距Token | iOS(4pt) | Android(4dp) | One UI(4px) | HarmonyOS(4px/8vp) | HyperOS(4px) | MagicOS(4px) | ColorOS(4px) | OriginOS(4px) | Flyme(4px) | Fluent(4px) | WeUI(4px) |
|-----------|----------|--------------|-------------|---------------------|--------------|--------------|--------------|---------------|------------|-------------|-----------|
| space-0.5 | 2px | 2dp | 2px | 2px/4vp | 2px | 2px | 2px | 2px | 2px | 2px | 2px |
| space-1 | 4px | 4dp | 4px | 4px/8vp | 4px | 4px | 4px | 4px | 4px | 4px | 4px |
| space-1.5 | 6px | 6dp | 6px | 6px/12vp | 6px | 6px | 6px | 6px | 6px | 6px | 6px |
| space-2 | 8px | 8dp | 8px | 8px/16vp | 8px | 8px | 8px | 8px | 8px | 8px | 8px |
| space-2.5 | 10px | 10dp | 10px | 10px/20vp | 10px | 10px | 10px | 10px | 10px | 10px | 10px |
| space-3 | 12px | 12dp | 12px | 12px/24vp | 12px | 12px | 12px | 12px | 12px | 12px | 12px |
| space-3.5 | 14px | 14dp | 14px | 14px/28vp | 14px | 14px | 14px | 14px | 14px | 14px | 14px |
| space-4 | 16px | 16dp | 16px | 16px/32vp | 16px | 16px | 16px | 16px | 16px | 16px | 16px |
| space-5 | 20px | 20dp | 20px | 20px/40vp | 20px | 20px | 20px | 20px | 20px | 20px | 20px |
| space-6 | 24px | 24dp | 24px | 24px/48vp | 24px | 24px | 24px | 24px | 24px | 24px | 24px |
| space-7 | 28px | 28dp | 28px | 28px/56vp | 28px | 28px | 28px | 28px | 28px | 28px | 28px |
| space-8 | 32px | 32dp | 32px | 32px/64vp | 32px | 32px | 32px | 32px | 32px | 32px | 32px |
| space-9 | 36px | 36dp | 36px | 36px/72vp | 36px | 36px | 36px | 36px | 36px | 36px | 36px |
| space-10 | 40px | 40dp | 40px | 40px/80vp | 40px | 40px | 40px | 40px | 40px | 40px | 40px |
| space-12 | 48px | 48dp | 48px | 48px/96vp | 48px | 48px | 48px | 48px | 48px | 48px | 48px |
| space-14 | 56px | 56dp | 56px | 56px/112vp | 56px | 56px | 56px | 56px | 56px | 56px | 56px |
| space-16 | 64px | 64dp | 64px | 64px/128vp | 64px | 64px | 64px | 64px | 64px | 64px | 64px |
| space-20 | 80px | 80dp | 80px | 80px/160vp | 80px | 80px | 80px | 80px | 80px | 80px | 80px |
| space-24 | 96px | 96dp | 96px | 96px/192vp | 96px | 96px | 96px | 96px | 96px | 96px | 96px |
| space-32 | 128px | 128dp | 128px | 128px/256vp | 128px | 128px | 128px | 128px | 128px | 128px | 128px |

### HarmonyOS vp单位换算表

HarmonyOS使用vp(virtual pixel)作为独立间距单位，基准为8vp网格：

| vp值 | px值(基准密度) | 换算公式 |
|------|---------------|---------|
| 1vp | 0.5px | px = vp * (屏幕密度/160) |
| 2vp | 1px | 基准密度下1vp=0.5px |
| 4vp | 2px | |
| 8vp | 4px | HarmonyOS最小间距单位 |
| 12vp | 6px | |
| 16vp | 8px | |
| 20vp | 10px | |
| 24vp | 12px | |
| 32vp | 16px | |
| 40vp | 20px | |
| 48vp | 24px | |
| 56vp | 28px | |
| 64vp | 32px | |
| 80vp | 40px | |
| 96vp | 48px | |

---

## 组件内间距规范

### 按钮组件间距

| 间距属性 | iOS | Android | One UI | HarmonyOS | HyperOS | MagicOS | ColorOS | OriginOS | Flyme | Fluent | WeUI |
|----------|-----|---------|--------|-----------|---------|---------|---------|----------|-------|--------|------|
| button-sm-padding-h | 12px | 12dp | 12px | 12px | 12px | 12px | 12px | 12px | 12px | 12px | 12px |
| button-sm-padding-v | 4px | 4dp | 4px | 4px | 4px | 4px | 4px | 4px | 4px | 4px | 4px |
| button-sm-height | 32px | 32dp | 32px | 32px | 32px | 32px | 32px | 32px | 32px | 28px | 30px |
| button-sm-icon-gap | 4px | 4dp | 4px | 4px | 4px | 4px | 4px | 4px | 4px | 4px | 4px |
| button-md-padding-h | 16px | 16dp | 16px | 16px | 16px | 16px | 16px | 16px | 16px | 12px | 16px |
| button-md-padding-v | 8px | 8dp | 8px | 8px | 8px | 8px | 8px | 8px | 8px | 6px | 8px |
| button-md-height | 44px | 40dp | 44px | 44px | 44px | 44px | 44px | 44px | 44px | 32px | 44px |
| button-md-icon-gap | 8px | 8dp | 8px | 8px | 8px | 8px | 8px | 8px | 8px | 8px | 8px |
| button-lg-padding-h | 24px | 24dp | 24px | 24px | 24px | 24px | 24px | 24px | 24px | 20px | 20px |
| button-lg-padding-v | 12px | 12dp | 12px | 12px | 12px | 12px | 12px | 12px | 12px | 8px | 10px |
| button-lg-height | 52px | 48dp | 52px | 52px | 52px | 52px | 52px | 52px | 52px | 40px | 48px |
| button-lg-icon-gap | 8px | 8dp | 8px | 8px | 8px | 8px | 8px | 8px | 8px | 8px | 8px |
| button-full-width-padding-h | 16px | 16dp | 16px | 16px | 16px | 16px | 16px | 16px | 16px | 16px | 16px |

### 卡片组件间距

| 间距属性 | iOS | Android | One UI | HarmonyOS | HyperOS | MagicOS | ColorOS | OriginOS | Flyme | Fluent | WeUI |
|----------|-----|---------|--------|-----------|---------|---------|---------|----------|-------|--------|------|
| card-padding | 16px | 16dp | 16px | 16px | 16px | 16px | 16px | 16px | 16px | 16px | 16px |
| card-padding-sm | 12px | 12dp | 12px | 12px | 12px | 12px | 12px | 12px | 12px | 12px | 12px |
| card-padding-lg | 20px | 20dp | 20px | 20px | 20px | 20px | 20px | 20px | 20px | 20px | 20px |
| card-gap | 12px | 12dp | 12px | 12px | 12px | 12px | 12px | 12px | 12px | 12px | 12px |
| card-header-padding-b | 12px | 12dp | 12px | 12px | 12px | 12px | 12px | 12px | 12px | 12px | 12px |
| card-footer-padding-t | 12px | 12dp | 12px | 12px | 12px | 12px | 12px | 12px | 12px | 12px | 12px |
| card-media-padding | 0px | 0dp | 0px | 0px | 0px | 0px | 0px | 0px | 0px | 0px | 0px |
| card-media-gap | 12px | 12dp | 12px | 12px | 12px | 12px | 12px | 12px | 12px | 12px | 12px |

### 列表项间距

| 间距属性 | iOS | Android | One UI | HarmonyOS | HyperOS | MagicOS | ColorOS | OriginOS | Flyme | Fluent | WeUI |
|----------|-----|---------|--------|-----------|---------|---------|---------|----------|-------|--------|------|
| list-item-padding-h | 16px | 16dp | 16px | 16px | 16px | 16px | 16px | 16px | 16px | 16px | 16px |
| list-item-padding-v | 12px | 12dp | 12px | 12px | 12px | 12px | 12px | 12px | 12px | 12px | 12px |
| list-item-height | 48px | 48dp | 48px | 48px | 48px | 48px | 48px | 48px | 48px | 48px | 48px |
| list-item-height-dense | 36px | 36dp | 36px | 36px | 36px | 36px | 36px | 36px | 36px | 36px | 36px |
| list-item-height-three | 72px | 72dp | 72px | 72px | 72px | 72px | 72px | 72px | 72px | 72px | 72px |
| list-item-icon-gap | 16px | 16dp | 16px | 16px | 16px | 16px | 16px | 16px | 16px | 16px | 16px |
| list-item-avatar-gap | 12px | 12dp | 12px | 12px | 12px | 12px | 12px | 12px | 12px | 12px | 12px |
| list-item-divider-inset | 56px | 56dp | 56px | 56px | 56px | 56px | 56px | 56px | 56px | 56px | 56px |
| list-section-gap | 24px | 24dp | 24px | 24px | 24px | 24px | 24px | 24px | 24px | 24px | 24px |

### 输入框间距

| 间距属性 | iOS | Android | One UI | HarmonyOS | HyperOS | MagicOS | ColorOS | OriginOS | Flyme | Fluent | WeUI |
|----------|-----|---------|--------|-----------|---------|---------|---------|----------|-------|--------|------|
| input-padding-h | 16px | 16dp | 16px | 16px | 16px | 16px | 16px | 16px | 16px | 12px | 12px |
| input-padding-v | 12px | 12dp | 12px | 12px | 12px | 12px | 12px | 12px | 12px | 8px | 10px |
| input-height | 44px | 48dp | 44px | 44px | 44px | 44px | 44px | 44px | 44px | 32px | 44px |
| input-label-gap | 4px | 4dp | 4px | 4px | 4px | 4px | 4px | 4px | 4px | 4px | 4px |
| input-icon-gap | 8px | 8dp | 8px | 8px | 8px | 8px | 8px | 8px | 8px | 8px | 8px |
| input-error-gap | 4px | 4dp | 4px | 4px | 4px | 4px | 4px | 4px | 4px | 4px | 4px |
| input-helper-gap | 4px | 4dp | 4px | 4px | 4px | 4px | 4px | 4px | 4px | 4px | 4px |

### 导航栏/标签栏间距

| 间距属性 | iOS | Android | One UI | HarmonyOS | HyperOS | MagicOS | ColorOS | OriginOS | Flyme | Fluent | WeUI |
|----------|-----|---------|--------|-----------|---------|---------|---------|----------|-------|--------|------|
| navbar-height | 44px | 56dp | 56px | 56px | 56px | 56px | 56px | 56px | 56px | 48px | 44px |
| navbar-padding-h | 16px | 16dp | 16px | 16px | 16px | 16px | 16px | 16px | 16px | 16px | 16px |
| navbar-icon-gap | 8px | 8dp | 8px | 8px | 8px | 8px | 8px | 8px | 8px | 8px | 8px |
| tabbar-height | 49px | 56dp | 56px | 56px | 56px | 56px | 56px | 56px | 56px | 48px | 50px |
| tabbar-padding-h | 0px | 0dp | 0px | 0px | 0px | 0px | 0px | 0px | 0px | 0px | 0px |
| tabbar-padding-v | 8px | 8dp | 8px | 8px | 8px | 8px | 8px | 8px | 8px | 4px | 6px |
| tabbar-icon-gap | 4px | 4dp | 4px | 4px | 4px | 4px | 4px | 4px | 4px | 4px | 4px |

---

## 页面布局间距

### 页面边距对照

| 间距属性 | iOS | Android | One UI | HarmonyOS | HyperOS | MagicOS | ColorOS | OriginOS | Flyme | Fluent | WeUI |
|----------|-----|---------|--------|-----------|---------|---------|---------|----------|-------|--------|------|
| page-margin-phone | 16px | 16dp | 16px | 16px | 16px | 16px | 16px | 16px | 16px | 16px | 16px |
| page-margin-fold | 24px | 24dp | 24px | 24px | 24px | 24px | 24px | 24px | 24px | 24px | 24px |
| page-margin-tablet | 32px | 32dp | 32px | 32px | 32px | 32px | 32px | 32px | 32px | 32px | 32px |
| page-margin-desktop | 48px | 48dp | 48px | 48px | 48px | 48px | 48px | 48px | 48px | 48px | 48px |
| page-max-width | 960px | 840dp | 840px | 840px | 840px | 840px | 840px | 840px | 840px | 1200px | 750px |

### 内容区间距

| 间距属性 | 手机 | 折叠屏 | 平板 | 桌面 | 说明 |
|----------|------|--------|------|------|------|
| section-gap | 32px | 36px | 40px | 48px | 页面主区块间距 |
| group-gap | 16px | 20px | 24px | 32px | 分组间距 |
| element-gap | 8px | 12px | 16px | 20px | 元素间距 |
| inline-gap | 4px | 4px | 8px | 8px | 行内元素间距 |
| card-content-padding | 16px | 20px | 24px | 32px | 卡片内容区内边距 |
| form-content-padding | 16px | 20px | 24px | 32px | 表单内容区内边距 |
| dialog-content-padding | 20px | 24px | 32px | 40px | 弹窗内容区内边距 |
| bottom-action-padding | 16px | 20px | 24px | 32px | 底部操作区内边距 |

### iOS特殊布局间距

| 场景 | 间距值 | 说明 |
|------|--------|------|
| 大标题页面顶部间距 | 0px | 大标题紧贴导航栏 |
| 普通页面顶部间距 | 20px | 导航栏下方内容起始 |
| 搜索栏下方间距 | 12px | 搜索栏与内容区间距 |
| Section Header | 32px | 分组标题上方间距 |
| Section Footer | 32px | 分组底部间距 |
| TableView Grouped间距 | 20px | 分组表格左右边距 |
| TableView Inset Grouped间距 | 20px | 圆角分组表格边距 |

### Android特殊布局间距

| 场景 | 间距值 | 说明 |
|------|--------|------|
| TopAppBar下方间距 | 16dp | 应用栏与内容区间距 |
| FAB距边缘 | 16dp | 浮动按钮距屏幕边缘 |
| BottomSheet顶部圆角 | 28dp | 底部抽屉圆角半径 |
| Navigation Rail宽度 | 80dp | 侧边导航栏宽度 |
| Navigation Drawer宽度 | 360dp | 侧边抽屉宽度 |
| Snackbar距底部 | 16dp | 消息条距底部导航栏 |

---

## 栅格系统

### 各平台栅格详细参数

| 平台 | 手机列数 | 平板列数 | 桌面列数 | 槽宽(手机) | 槽宽(平板) | 槽宽(桌面) | 边距(手机) | 边距(平板) | 边距(桌面) |
|------|---------|---------|---------|-----------|-----------|-----------|-----------|-----------|-----------|
| iOS | 4列 | 8列 | 12列 | 16px | 20px | 24px | 16px | 24px | 48px |
| Android | 4列 | 8列 | 12列 | 16dp | 20dp | 24dp | 16dp | 24dp | 48dp |
| One UI | 4列 | 8列 | 12列 | 16px | 20px | 24px | 16px | 24px | 48px |
| HarmonyOS | 4列 | 8列 | 12列 | 16px | 20px | 24px | 16px | 24px | 48px |
| HyperOS | 4列 | 8列 | 12列 | 16px | 20px | 24px | 16px | 24px | 48px |
| MagicOS | 4列 | 8列 | 12列 | 16px | 20px | 24px | 16px | 24px | 48px |
| ColorOS | 4列 | 8列 | 12列 | 16px | 20px | 24px | 16px | 24px | 48px |
| OriginOS | 4列 | 8列 | 12列 | 16px | 20px | 24px | 16px | 24px | 48px |
| Flyme | 4列 | 8列 | 12列 | 16px | 20px | 24px | 16px | 24px | 48px |
| Fluent | 4列 | 8列 | 12列 | 16px | 20px | 24px | 16px | 24px | 48px |
| WeUI | 4列 | 8列 | 8列 | 16px | 20px | 24px | 16px | 24px | 48px |

### 栅格CSS实现

```css
/* 栅格Token */
--grid-columns-phone: 4;
--grid-columns-tablet: 8;
--grid-columns-desktop: 12;
--grid-gutter-phone: 16px;
--grid-gutter-tablet: 20px;
--grid-gutter-desktop: 24px;
--grid-margin-phone: 16px;
--grid-margin-tablet: 24px;
--grid-margin-desktop: 48px;

/* 栅格布局 */
.grid {
  display: grid;
  gap: var(--grid-gutter-phone);
  grid-template-columns: repeat(var(--grid-columns-phone), 1fr);
  padding: 0 var(--grid-margin-phone);
}

@media (min-width: 840px) {
  .grid {
    gap: var(--grid-gutter-tablet);
    grid-template-columns: repeat(var(--grid-columns-tablet), 1fr);
    padding: 0 var(--grid-margin-tablet);
  }
}

@media (min-width: 1280px) {
  .grid {
    gap: var(--grid-gutter-desktop);
    grid-template-columns: repeat(var(--grid-columns-desktop), 1fr);
    padding: 0 var(--grid-margin-desktop);
  }
}
```

---

## 安全区域间距

### 刘海屏/挖孔屏避让间距

| 区域 | iOS(刘海屏) | iOS(Dynamic Island) | Android(挖孔屏) | HarmonyOS(挖孔屏) | 说明 |
|------|------------|--------------------|-----------------|--------------------|------|
| 顶部安全区高度 | 44px | 59px | 24px-48px | 24px-48px | 状态栏+刘海/挖孔 |
| 刘海宽度 | 209px | 126px | 80px-120px | 80px-120px | 横屏时左右避让宽度 |
| 横屏左侧避让 | 44px | 59px | 0px-24px | 0px-24px | 横屏时刘海侧避让 |
| 横屏右侧避让 | 44px | 59px | 0px-24px | 0px-24px | 横屏时对侧避让 |

### 底部Home Indicator避让

| 区域 | iOS | Android(手势导航) | HarmonyOS(手势) | 说明 |
|------|-----|-------------------|-----------------|------|
| Home指示器高度 | 34px | 48px | 48px | 底部手势区域高度 |
| Home指示器条高度 | 5px | - | - | 底部小横条高度 |
| Home指示器条宽度 | 134px | - | - | 底部小横条宽度 |
| 内容底部最小避让 | 34px | 0px | 0px | iOS强制避让34px |

### 各机型安全区域详细数值

#### iOS机型安全区域

| 机型 | 顶部安全区 | 底部安全区 | 左侧安全区(横屏) | 右侧安全区(横屏) |
|------|-----------|-----------|-----------------|-----------------|
| iPhone 15 Pro Max | 59px | 34px | 59px | 59px |
| iPhone 15 Pro | 59px | 34px | 59px | 59px |
| iPhone 15 | 59px | 34px | 59px | 59px |
| iPhone 14 Pro Max | 59px | 34px | 59px | 59px |
| iPhone 14 Pro | 59px | 34px | 59px | 59px |
| iPhone 14 | 44px | 34px | 44px | 44px |
| iPhone SE (3rd) | 20px | 0px | 0px | 0px |
| iPad Pro 12.9" | 24px | 20px | 24px | 24px |
| iPad Pro 11" | 24px | 20px | 24px | 24px |
| iPad Air | 20px | 0px | 0px | 0px |

#### Android主流机型安全区域

| 机型 | 顶部安全区 | 底部安全区 | 说明 |
|------|-----------|-----------|------|
| Samsung S24 Ultra | 40px | 48px | 挖孔屏+手势导航 |
| Samsung S24 | 36px | 48px | 挖孔屏+手势导航 |
| Pixel 8 Pro | 32px | 48px | 挖孔屏+手势导航 |
| Xiaomi 14 Pro | 36px | 48px | 挖孔屏+手势导航 |
| Huawei Mate 60 Pro | 36px | 48px | 挖孔屏+手势导航 |
| OPPO Find X7 | 36px | 48px | 挖孔屏+手势导航 |
| vivo X100 Pro | 36px | 48px | 挖孔屏+手势导航 |

### 安全区域CSS实现

```css
/* iOS安全区域 - env()函数 */
--safe-area-inset-top: env(safe-area-inset-top, 0px);
--safe-area-inset-bottom: env(safe-area-inset-bottom, 0px);
--safe-area-inset-left: env(safe-area-inset-left, 0px);
--safe-area-inset-right: env(safe-area-inset-right, 0px);

/* 顶部导航栏适配 */
.navbar {
  padding-top: var(--safe-area-inset-top);
  height: calc(44px + var(--safe-area-inset-top));
}

/* 底部操作区适配 */
.bottom-action {
  padding-bottom: var(--safe-area-inset-bottom);
  min-height: calc(49px + var(--safe-area-inset-bottom));
}

/* 横屏适配 */
@media (orientation: landscape) {
  .page-content {
    padding-left: var(--safe-area-inset-left);
    padding-right: var(--safe-area-inset-right);
  }
}

/* 全屏内容适配 */
.fullscreen-content {
  padding-top: var(--safe-area-inset-top);
  padding-bottom: var(--safe-area-inset-bottom);
  padding-left: var(--safe-area-inset-left);
  padding-right: var(--safe-area-inset-right);
}

/* Android安全区域 - windowInsets */
/* Android通过ViewCompat.setOnApplyWindowInsetsListener实现 */
/* Web端通过viewport-fit=cover + env()实现 */

/* viewport设置 */
/* <meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover"> */

/* 微信小程序安全区域 */
.wx-safe-area-top {
  padding-top: calc(var(--status-bar-height, 20px) + 44px);
}

.wx-safe-area-bottom {
  padding-bottom: env(safe-area-inset-bottom, 0px);
}
```
