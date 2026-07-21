> @author aitool.plus

# 字体排版体系

## 概述

本字体排版体系覆盖11大操作系统平台，包含字体族、字号阶梯、行高、字重、字间距等完整规范。

---

## 字体族

### 各OS系统字体栈

#### Apple iOS

```css
--font-family-ios: -apple-system, BlinkMacSystemFont, "SF Pro Text", "SF Pro Display", "Helvetica Neue", "PingFang SC", "Hiragino Sans GB", "Microsoft YaHei", sans-serif;
```

#### Google Android

```css
--font-family-android: "Roboto", "Noto Sans", "Noto Sans SC", "PingFang SC", "Microsoft YaHei", sans-serif;
```

#### Samsung One UI

```css
--font-family-samsung: "SamsungOne", "Roboto", "Noto Sans SC", "PingFang SC", "Microsoft YaHei", sans-serif;
```

#### Huawei HarmonyOS

```css
--font-family-huawei: "HarmonyOS Sans", "PingFang SC", "Microsoft YaHei", sans-serif;
```

#### Xiaomi HyperOS

```css
--font-family-xiaomi: "MiSans", "PingFang SC", "Microsoft YaHei", sans-serif;
```

#### Honor MagicOS

```css
--font-family-honor: "Honor Sans", "PingFang SC", "Microsoft YaHei", sans-serif;
```

#### OPPO ColorOS

```css
--font-family-oppo: "OPPO Sans", "PingFang SC", "Microsoft YaHei", sans-serif;
```

#### vivo OriginOS

```css
--font-family-vivo: "vivo Sans", "PingFang SC", "Microsoft YaHei", sans-serif;
```

#### Meizu Flyme

```css
--font-family-meizu: "Flyme Sans", "PingFang SC", "Microsoft YaHei", sans-serif;
```

#### Windows 11 Fluent

```css
--font-family-windows: "Segoe UI Variable", "Segoe UI", "Microsoft YaHei", "PingFang SC", sans-serif;
```

#### WeChat WeUI

```css
--font-family-wechat: "PingFang SC", "Hiragino Sans GB", "Microsoft YaHei", sans-serif;
```

---

## 字号阶梯

### 各OS完整字号表

| Token名称 | Apple iOS | Google Android | Samsung One UI | Huawei HarmonyOS | Xiaomi HyperOS | Honor MagicOS | OPPO ColorOS | vivo OriginOS | Meizu Flyme | Windows Fluent | WeChat WeUI |
|-----------|-----------|----------------|----------------|------------------|----------------|---------------|--------------|---------------|-------------|----------------|-------------|
| text-xs | 11px | 12px | 11px | 11px | 11px | 11px | 11px | 11px | 11px | 12px | 11px |
| text-sm | 13px | 14px | 13px | 13px | 13px | 13px | 13px | 13px | 13px | 14px | 13px |
| text-base | 15px | 16px | 15px | 15px | 15px | 15px | 15px | 15px | 15px | 16px | 14px |
| text-lg | 17px | 18px | 17px | 17px | 17px | 17px | 17px | 17px | 17px | 18px | 16px |
| text-xl | 20px | 22px | 20px | 20px | 20px | 20px | 20px | 20px | 20px | 22px | 18px |
| text-2xl | 24px | 28px | 24px | 24px | 24px | 24px | 24px | 24px | 24px | 28px | 20px |
| text-3xl | 32px | 36px | 32px | 32px | 32px | 32px | 32px | 32px | 32px | 36px | 24px |
| text-4xl | 40px | 45px | 40px | 40px | 40px | 40px | 40px | 40px | 40px | 45px | 28px |
| text-5xl | 48px | 56px | 48px | 48px | 48px | 48px | 48px | 48px | 48px | 56px | 32px |

### CSS rem换算

```css
/* 基准字号 16px = 1rem */
--text-xs: 0.6875rem;    /* 11px */
--text-sm: 0.8125rem;    /* 13px */
--text-base: 0.9375rem;  /* 15px */
--text-lg: 1.0625rem;    /* 17px */
--text-xl: 1.25rem;      /* 20px */
--text-2xl: 1.5rem;      /* 24px */
--text-3xl: 2rem;        /* 32px */
--text-4xl: 2.5rem;      /* 40px */
--text-5xl: 3rem;        /* 48px */
```

---

## 行高

### 各OS行高规范

| 字号 | Apple iOS | Google Android | Samsung One UI | Huawei HarmonyOS | Xiaomi HyperOS | Honor MagicOS | OPPO ColorOS | vivo OriginOS | Meizu Flyme | Windows Fluent | WeChat WeUI |
|------|-----------|----------------|----------------|------------------|----------------|---------------|--------------|---------------|-------------|----------------|-------------|
| text-xs | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 |
| text-sm | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 |
| text-base | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 |
| text-lg | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 |
| text-xl | 1.3 | 1.3 | 1.3 | 1.3 | 1.3 | 1.3 | 1.3 | 1.3 | 1.3 | 1.3 | 1.3 |
| text-2xl | 1.25 | 1.25 | 1.25 | 1.25 | 1.25 | 1.25 | 1.25 | 1.25 | 1.25 | 1.25 | 1.25 |
| text-3xl | 1.2 | 1.2 | 1.2 | 1.2 | 1.2 | 1.2 | 1.2 | 1.2 | 1.2 | 1.2 | 1.2 |
| text-4xl | 1.15 | 1.15 | 1.15 | 1.15 | 1.15 | 1.15 | 1.15 | 1.15 | 1.15 | 1.15 | 1.15 |
| text-5xl | 1.1 | 1.1 | 1.1 | 1.1 | 1.1 | 1.1 | 1.1 | 1.1 | 1.1 | 1.1 | 1.1 |

### CSS变量定义

```css
--line-height-tight: 1.25;
--line-height-normal: 1.5;
--line-height-relaxed: 1.75;
--line-height-loose: 2;
```

---

## 字重

### 各OS字重值

| 字重名称 | Apple iOS | Google Android | Samsung One UI | Huawei HarmonyOS | Xiaomi HyperOS | Honor MagicOS | OPPO ColorOS | vivo OriginOS | Meizu Flyme | Windows Fluent | WeChat WeUI |
|----------|-----------|----------------|----------------|------------------|----------------|---------------|--------------|---------------|-------------|----------------|-------------|
| Thin | 100 | - | - | - | - | - | - | - | - | - | - |
| Light | 300 | 300 | 300 | 300 | 300 | 300 | 300 | 300 | 300 | 300 | 300 |
| Regular | 400 | 400 | 400 | 400 | 400 | 400 | 400 | 400 | 400 | 400 | 400 |
| Medium | 500 | 500 | 500 | 500 | 500 | 500 | 500 | 500 | 500 | 500 | 500 |
| Semibold | 600 | 600 | 600 | 600 | 600 | 600 | 600 | 600 | 600 | 600 | 600 |
| Bold | 700 | 700 | 700 | 700 | 700 | 700 | 700 | 700 | 700 | 700 | 700 |
| Heavy | 800 | - | - | - | - | - | - | - | - | - | - |
| Black | 900 | 900 | 900 | 900 | 900 | 900 | 900 | 900 | 900 | 900 | 900 |

### CSS变量定义

```css
--font-weight-light: 300;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--font-weight-black: 900;
```

---

## 字间距

### 各OS字间距规范

| 字号 | Apple iOS | Google Android | Samsung One UI | Huawei HarmonyOS | Xiaomi HyperOS | Honor MagicOS | OPPO ColorOS | vivo OriginOS | Meizu Flyme | Windows Fluent | WeChat WeUI |
|------|-----------|----------------|----------------|------------------|----------------|---------------|--------------|---------------|-------------|----------------|-------------|
| text-xs | -0.01em | 0em | -0.01em | -0.01em | -0.01em | -0.01em | -0.01em | -0.01em | -0.01em | 0em | -0.01em |
| text-sm | -0.01em | 0em | -0.01em | -0.01em | -0.01em | -0.01em | -0.01em | -0.01em | -0.01em | 0em | -0.01em |
| text-base | -0.02em | 0em | -0.02em | -0.02em | -0.02em | -0.02em | -0.02em | -0.02em | -0.02em | 0em | -0.02em |
| text-lg | -0.02em | 0em | -0.02em | -0.02em | -0.02em | -0.02em | -0.02em | -0.02em | -0.02em | 0em | -0.02em |
| text-xl | -0.02em | 0em | -0.02em | -0.02em | -0.02em | -0.02em | -0.02em | -0.02em | -0.02em | 0em | -0.02em |
| text-2xl | -0.03em | 0em | -0.03em | -0.03em | -0.03em | -0.03em | -0.03em | -0.03em | -0.03em | 0em | -0.03em |
| text-3xl | -0.03em | 0em | -0.03em | -0.03em | -0.03em | -0.03em | -0.03em | -0.03em | -0.03em | 0em | -0.03em |
| text-4xl | -0.04em | 0em | -0.04em | -0.04em | -0.04em | -0.04em | -0.04em | -0.04em | -0.04em | 0em | -0.04em |
| text-5xl | -0.04em | 0em | -0.04em | -0.04em | -0.04em | -0.04em | -0.04em | -0.04em | -0.04em | 0em | -0.04em |

### CSS变量定义

```css
--letter-spacing-tight: -0.04em;
--letter-spacing-normal: -0.02em;
--letter-spacing-wide: 0em;
--letter-spacing-wider: 0.02em;
```

---

## 中文排版特殊规则

### 标点符号

- 中文标点使用全角字符
- 引号使用「」或『』
- 省略号使用……（两个全角点）
- 破折号使用——（两个全角横线）

### 数字与字母

- 数字和英文字母与中文之间保留半角空格
- 例如：使用 iPhone 15 Pro 拍摄 4K 视频
- 例外：连续的英文单词间不额外加空格

### 行首行尾

- 行首避免出现标点符号
- 行尾避免出现孤字（单个汉字）
- 标题末尾不加标点符号

### 字体回退

- 优先使用系统字体
- 回退顺序：系统字体 -> PingFang SC -> Hiragino Sans GB -> Microsoft YaHei -> sans-serif

---

## Web安全字体回退方案

### 通用字体栈

```css
/* 中文通用 */
--font-family-chinese: "PingFang SC", "Hiragino Sans GB", "Microsoft YaHei", "Noto Sans SC", "Source Han Sans SC", sans-serif;

/* 英文通用 */
--font-family-english: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;

/* 混合通用 */
--font-family-universal: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", "PingFang SC", "Hiragino Sans GB", "Microsoft YaHei", Arial, sans-serif;
```

### 各平台字体加载优先级

| 平台 | 第一优先级 | 第二优先级 | 第三优先级 | 回退 |
|------|-----------|-----------|-----------|------|
| iOS/macOS | SF Pro | PingFang SC | Hiragino Sans GB | system-ui |
| Android | Roboto | Noto Sans SC | PingFang SC | sans-serif |
| Windows | Segoe UI | Microsoft YaHei | PingFang SC | sans-serif |
| Web通用 | system-ui | -apple-system | Segoe UI | sans-serif |

### 字体加载策略

1. 优先使用系统预装字体，避免额外加载
2. 如需自定义字体，使用 font-display: swap 避免 FOIT
3. 中文字体文件较大，建议使用子集化加载
4. 提供 woff2 格式优先加载

---

## 11大平台完整字体阶梯对照表

### Display层级

| Token | iOS | Android | One UI | HarmonyOS | HyperOS | MagicOS | ColorOS | OriginOS | Flyme | Fluent | WeUI |
|-------|-----|---------|--------|-----------|---------|---------|---------|----------|-------|--------|------|
| display-large-size | 48px/57sp | 57dp/57sp | 48px | 48fp | 48px | 48px | 48px | 48px | 48px | 68px | 32px |
| display-large-weight | 700 | 400 | 700 | 700 | 700 | 700 | 700 | 700 | 700 | 600 | 700 |
| display-large-lineHeight | 1.1 | 1.12 | 1.1 | 1.1 | 1.1 | 1.1 | 1.1 | 1.1 | 1.1 | 1.1 | 1.2 |
| display-large-tracking | -0.04em | -0.02em | -0.04em | -0.04em | -0.04em | -0.04em | -0.04em | -0.04em | -0.04em | -0.02em | -0.03em |
| display-medium-size | 40px/45sp | 45dp/45sp | 40px | 40fp | 40px | 40px | 40px | 40px | 40px | 48px | 28px |
| display-medium-weight | 700 | 400 | 700 | 700 | 700 | 700 | 700 | 700 | 700 | 600 | 700 |
| display-medium-lineHeight | 1.15 | 1.16 | 1.15 | 1.15 | 1.15 | 1.15 | 1.15 | 1.15 | 1.15 | 1.15 | 1.25 |
| display-medium-tracking | -0.04em | -0.02em | -0.04em | -0.04em | -0.04em | -0.04em | -0.04em | -0.04em | -0.04em | -0.02em | -0.03em |
| display-small-size | 32px/36sp | 36dp/36sp | 32px | 32fp | 32px | 32px | 32px | 32px | 32px | 40px | 24px |
| display-small-weight | 700 | 400 | 700 | 700 | 700 | 700 | 700 | 700 | 700 | 600 | 700 |
| display-small-lineHeight | 1.2 | 1.22 | 1.2 | 1.2 | 1.2 | 1.2 | 1.2 | 1.2 | 1.2 | 1.2 | 1.25 |
| display-small-tracking | -0.03em | -0.01em | -0.03em | -0.03em | -0.03em | -0.03em | -0.03em | -0.03em | -0.03em | -0.01em | -0.02em |

### Headline层级

| Token | iOS | Android | One UI | HarmonyOS | HyperOS | MagicOS | ColorOS | OriginOS | Flyme | Fluent | WeUI |
|-------|-----|---------|--------|-----------|---------|---------|---------|----------|-------|--------|------|
| headline-large-size | 28px/32sp | 32dp/32sp | 28px | 28fp | 28px | 28px | 28px | 28px | 28px | 32px | 22px |
| headline-large-weight | 700 | 400 | 600 | 600 | 600 | 600 | 600 | 600 | 600 | 600 | 700 |
| headline-large-lineHeight | 1.25 | 1.25 | 1.25 | 1.25 | 1.25 | 1.25 | 1.25 | 1.25 | 1.25 | 1.3 | 1.3 |
| headline-large-tracking | -0.03em | -0.01em | -0.03em | -0.03em | -0.03em | -0.03em | -0.03em | -0.03em | -0.03em | -0.01em | -0.02em |
| headline-medium-size | 24px/28sp | 28dp/28sp | 24px | 24fp | 24px | 24px | 24px | 24px | 24px | 28px | 20px |
| headline-medium-weight | 700 | 400 | 600 | 600 | 600 | 600 | 600 | 600 | 600 | 600 | 700 |
| headline-medium-lineHeight | 1.25 | 1.29 | 1.25 | 1.25 | 1.25 | 1.25 | 1.25 | 1.25 | 1.25 | 1.3 | 1.3 |
| headline-medium-tracking | -0.03em | 0em | -0.03em | -0.03em | -0.03em | -0.03em | -0.03em | -0.03em | -0.03em | 0em | -0.02em |
| headline-small-size | 20px/24sp | 24dp/24sp | 20px | 20fp | 20px | 20px | 20px | 20px | 20px | 24px | 18px |
| headline-small-weight | 600 | 400 | 600 | 600 | 600 | 600 | 600 | 600 | 600 | 600 | 600 |
| headline-small-lineHeight | 1.3 | 1.33 | 1.3 | 1.3 | 1.3 | 1.3 | 1.3 | 1.3 | 1.3 | 1.3 | 1.35 |
| headline-small-tracking | -0.02em | 0em | -0.02em | -0.02em | -0.02em | -0.02em | -0.02em | -0.02em | -0.02em | 0em | -0.01em |

### Title层级

| Token | iOS | Android | One UI | HarmonyOS | HyperOS | MagicOS | ColorOS | OriginOS | Flyme | Fluent | WeUI |
|-------|-----|---------|--------|-----------|---------|---------|---------|----------|-------|--------|------|
| title-large-size | 17px/22sp | 22dp/22sp | 17px | 17fp | 17px | 17px | 17px | 17px | 17px | 20px | 17px |
| title-large-weight | 600 | 400 | 500 | 500 | 500 | 500 | 500 | 500 | 500 | 600 | 600 |
| title-large-lineHeight | 1.4 | 1.27 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 |
| title-large-tracking | -0.02em | 0em | -0.02em | -0.02em | -0.02em | -0.02em | -0.02em | -0.02em | -0.02em | 0em | -0.01em |
| title-medium-size | 15px/16sp | 16dp/16sp | 15px | 15fp | 15px | 15px | 15px | 15px | 15px | 16px | 16px |
| title-medium-weight | 500 | 500 | 500 | 500 | 500 | 500 | 500 | 500 | 500 | 600 | 500 |
| title-medium-lineHeight | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 |
| title-medium-tracking | -0.02em | 0.01em | -0.02em | -0.02em | -0.02em | -0.02em | -0.02em | -0.02em | -0.02em | 0em | -0.01em |
| title-small-size | 13px/14sp | 14dp/14sp | 13px | 13fp | 13px | 13px | 13px | 13px | 13px | 14px | 14px |
| title-small-weight | 500 | 500 | 500 | 500 | 500 | 500 | 500 | 500 | 500 | 600 | 500 |
| title-small-lineHeight | 1.5 | 1.43 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 |
| title-small-tracking | -0.01em | 0.01em | -0.01em | -0.01em | -0.01em | -0.01em | -0.01em | -0.01em | -0.01em | 0em | 0em |

### Body层级

| Token | iOS | Android | One UI | HarmonyOS | HyperOS | MagicOS | ColorOS | OriginOS | Flyme | Fluent | WeUI |
|-------|-----|---------|--------|-----------|---------|---------|---------|----------|-------|--------|------|
| body-large-size | 17px/16sp | 16dp/16sp | 17px | 17fp | 17px | 17px | 17px | 17px | 17px | 16px | 16px | 17px |
| body-large-weight | 400 | 400 | 400 | 400 | 400 | 400 | 400 | 400 | 400 | 400 | 400 |
| body-large-lineHeight | 1.4 | 1.5 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 | 1.5 | 1.5 | 1.5 |
| body-large-tracking | -0.02em | 0.02em | -0.02em | -0.02em | -0.02em | -0.02em | -0.02em | -0.02em | 0em | 0em | -0.01em |
| body-medium-size | 15px/14sp | 14dp/14sp | 15px | 15fp | 15px | 15px | 15px | 15px | 14px | 14px | 15px |
| body-medium-weight | 400 | 400 | 400 | 400 | 400 | 400 | 400 | 400 | 400 | 400 | 400 |
| body-medium-lineHeight | 1.5 | 1.43 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 |
| body-medium-tracking | -0.02em | 0.02em | -0.02em | -0.02em | -0.02em | -0.02em | -0.02em | -0.02em | 0em | 0em | -0.01em |
| body-small-size | 13px/12sp | 12dp/12sp | 13px | 13fp | 13px | 13px | 13px | 13px | 12px | 12px | 13px |
| body-small-weight | 400 | 400 | 400 | 400 | 400 | 400 | 400 | 400 | 400 | 400 | 400 |
| body-small-lineHeight | 1.5 | 1.33 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 |
| body-small-tracking | -0.01em | 0.03em | -0.01em | -0.01em | -0.01em | -0.01em | -0.01em | -0.01em | 0em | 0em | 0em |

### Label层级

| Token | iOS | Android | One UI | HarmonyOS | HyperOS | MagicOS | ColorOS | OriginOS | Flyme | Fluent | WeUI |
|-------|-----|---------|--------|-----------|---------|---------|---------|----------|-------|--------|------|
| label-large-size | 15px/14sp | 14dp/14sp | 15px | 15fp | 15px | 15px | 15px | 15px | 14px | 14px | 14px |
| label-large-weight | 500 | 500 | 500 | 500 | 500 | 500 | 500 | 500 | 500 | 600 | 500 |
| label-large-lineHeight | 1.5 | 1.43 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 |
| label-large-tracking | -0.02em | 0.01em | -0.02em | -0.02em | -0.02em | -0.02em | -0.02em | -0.02em | 0em | 0em | 0em |
| label-medium-size | 13px/12sp | 12dp/12sp | 13px | 13fp | 13px | 13px | 13px | 13px | 12px | 12px | 12px |
| label-medium-weight | 500 | 500 | 500 | 500 | 500 | 500 | 500 | 500 | 500 | 600 | 500 |
| label-medium-lineHeight | 1.5 | 1.33 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 | 1.5 |
| label-medium-tracking | -0.01em | 0.04em | -0.01em | -0.01em | -0.01em | -0.01em | -0.01em | -0.01em | 0em | 0em | 0em |
| label-small-size | 11px/11sp | 11dp/11sp | 11px | 11fp | 11px | 11px | 11px | 11px | 11px | 10px | 10px |
| label-small-weight | 500 | 500 | 500 | 500 | 500 | 500 | 500 | 500 | 500 | 600 | 500 |
| label-small-lineHeight | 1.4 | 1.45 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 |
| label-small-tracking | -0.01em | 0.04em | -0.01em | -0.01em | -0.01em | -0.01em | -0.01em | -0.01em | 0em | 0em | 0em |

### Caption/Overline层级

| Token | iOS | Android | One UI | HarmonyOS | HyperOS | MagicOS | ColorOS | OriginOS | Flyme | Fluent | WeUI |
|-------|-----|---------|--------|-----------|---------|---------|---------|----------|-------|--------|------|
| caption-size | 11px/12sp | 12dp/12sp | 11px | 11fp | 11px | 11px | 11px | 11px | 11px | 12px | 10px |
| caption-weight | 400 | 400 | 400 | 400 | 400 | 400 | 400 | 400 | 400 | 400 | 400 |
| caption-lineHeight | 1.4 | 1.33 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 |
| caption-tracking | -0.01em | 0.03em | -0.01em | -0.01em | -0.01em | -0.01em | -0.01em | -0.01em | 0em | 0em | 0em |
| overline-size | 10px/10sp | 10dp/10sp | 10px | 10fp | 10px | 10px | 10px | 10px | 10px | 10px | 10px |
| overline-weight | 500 | 500 | 500 | 500 | 500 | 500 | 500 | 500 | 500 | 600 | 500 |
| overline-lineHeight | 1.4 | 1.6 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 | 1.4 |
| overline-tracking | 0.02em | 0.08em | 0.02em | 0.02em | 0.02em | 0.02em | 0.02em | 0.02em | 0.02em | 0.04em | 0.02em |

---

## 字体族对照表

### 各平台推荐字体族完整对照

| 平台 | 英文主字体 | 英文回退 | 中文主字体 | 中文回退 | 等宽字体 |
|------|-----------|---------|-----------|---------|---------|
| iOS | SF Pro Text(<19pt)/SF Pro Display(>=19pt) | Helvetica Neue, Arial | PingFang SC | Hiragino Sans GB, STHeiti | SF Mono, Menlo |
| Android | Roboto | Noto Sans, Arial | Noto Sans SC | PingFang SC, Microsoft YaHei | Roboto Mono, Droid Sans Mono |
| One UI | SamsungOne | Roboto, Noto Sans | Noto Sans SC | Samsung Sans SC | SamsungOne Mono |
| HarmonyOS | HarmonyOS Sans | PingFang SC, Roboto | HarmonyOS Sans SC | PingFang SC, Noto Sans SC | HarmonyOS Sans Mono |
| HyperOS | MiSans | Roboto, Noto Sans | MiSans | PingFang SC, Noto Sans SC | MiSans Mono |
| MagicOS | Honor Sans | Roboto, Noto Sans | Honor Sans SC | PingFang SC, Noto Sans SC | Honor Sans Mono |
| ColorOS | OPPO Sans | Roboto, Noto Sans | OPPO Sans SC | PingFang SC, Noto Sans SC | OPPO Sans Mono |
| OriginOS | vivo Sans | Roboto, Noto Sans | vivo Sans SC | PingFang SC, Noto Sans SC | vivo Sans Mono |
| Flyme | Flyme Sans | Roboto, Noto Sans | Flyme Sans SC | PingFang SC, Noto Sans SC | Flyme Sans Mono |
| Fluent | Segoe UI Variable(>=12pt)/Segoe UI(<12pt) | Arial, Roboto | Microsoft YaHei | PingFang SC, Noto Sans SC | Cascadia Code, Consolas |
| WeUI | PingFang SC | Helvetica Neue, Arial | PingFang SC | Hiragino Sans GB, Microsoft YaHei | Menlo, Courier New |

### 完整字体族Fallback链

```css
/* iOS */
--font-family-ios: "SF Pro Text", "SF Pro Display", -apple-system, BlinkMacSystemFont, "Helvetica Neue", "PingFang SC", "Hiragino Sans GB", "Microsoft YaHei", "STHeiti", Arial, sans-serif;

/* Android */
--font-family-android: "Roboto", "Noto Sans", "Noto Sans SC", "PingFang SC", "Microsoft YaHei", Arial, sans-serif;

/* One UI */
--font-family-samsung: "SamsungOne", "Roboto", "Noto Sans SC", "PingFang SC", "Microsoft YaHei", Arial, sans-serif;

/* HarmonyOS */
--font-family-huawei: "HarmonyOS Sans", "HarmonyOS Sans SC", "PingFang SC", "Noto Sans SC", "Microsoft YaHei", Roboto, sans-serif;

/* HyperOS */
--font-family-xiaomi: "MiSans", "MiSans Mono", "PingFang SC", "Noto Sans SC", "Microsoft YaHei", Roboto, sans-serif;

/* MagicOS */
--font-family-honor: "Honor Sans", "Honor Sans SC", "PingFang SC", "Noto Sans SC", "Microsoft YaHei", Roboto, sans-serif;

/* ColorOS */
--font-family-oppo: "OPPO Sans", "OPPO Sans SC", "PingFang SC", "Noto Sans SC", "Microsoft YaHei", Roboto, sans-serif;

/* OriginOS */
--font-family-vivo: "vivo Sans", "vivo Sans SC", "PingFang SC", "Noto Sans SC", "Microsoft YaHei", Roboto, sans-serif;

/* Flyme */
--font-family-meizu: "Flyme Sans", "Flyme Sans SC", "PingFang SC", "Noto Sans SC", "Microsoft YaHei", Roboto, sans-serif;

/* Fluent */
--font-family-windows: "Segoe UI Variable", "Segoe UI", "Microsoft YaHei", "PingFang SC", "Noto Sans SC", Arial, sans-serif;

/* WeUI */
--font-family-wechat: "PingFang SC", "Hiragino Sans GB", "Microsoft YaHei", "Helvetica Neue", Arial, sans-serif;

/* 等宽字体 */
--font-family-mono-ios: "SF Mono", "Menlo", "Courier New", monospace;
--font-family-mono-android: "Roboto Mono", "Droid Sans Mono", "Courier New", monospace;
--font-family-mono-huawei: "HarmonyOS Sans Mono", "Menlo", "Courier New", monospace;
--font-family-mono-windows: "Cascadia Code", "Consolas", "Courier New", monospace;
--font-family-mono-universal: "SF Mono", "Roboto Mono", "Cascadia Code", "Menlo", "Consolas", "Courier New", monospace;
```

---

## 中文字体规范

### 标点挤压规则

| 规则 | iOS | Android | HarmonyOS | Windows | 说明 |
|------|-----|---------|-----------|---------|------|
| 行首标点挤压 | 全角标点压缩为半角 | 全角标点压缩为半角 | 全角标点压缩为半角 | 全角标点压缩为半角 | 逗号、句号、顿号等行首出现时压缩 |
| 行尾标点挤压 | 不压缩 | 不压缩 | 不压缩 | 不压缩 | 行尾标点保持全角 |
| 连续标点挤压 | 相邻标点间间距压缩50% | 标点间间距压缩50% | 标点间间距压缩50% | 标点间间距压缩50% | 如"），"中间距压缩 |
| 括号内标点 | 括号内标点正常 | 括号内标点正常 | 括号内标点正常 | 括号内标点正常 | 括号内标点不额外挤压 |

### 避头尾规则

| 禁止出现在行首的字符 | 禁止出现在行尾的字符 |
|---------------------|---------------------|
| ， 、 。 ！ ？ ： ； | （ 〔 〈 《 「 『 |
| ） 〕 〉 》 」 』 | - -- ...  ~ |
| ． ， ： ； ！ ？ |  |
| 」 』 】 〗 〉 》 |  |

### 中英文混排间距

| 场景 | 间距规则 | CSS实现 | 说明 |
|------|----------|---------|------|
| 中文与英文之间 | 半角空格(约1/4em) | text-autospace: ideograph-alpha | 自动插入间距 |
| 中文与数字之间 | 半角空格(约1/4em) | text-autospace: ideograph-numeric | 自动插入间距 |
| 英文与中文标点之间 | 无额外间距 | 无需处理 | 标点本身已含间距 |
| 连续英文单词间 | 正常英文空格 | 正常空格 | 不额外处理 |
| 数字与单位之间 | 半角空格 | 手动插入 | 如"16 px" |

### 中文排版CSS实现

```css
/* 中文排版基础 */
--text-autospace: ideograph-alpha ideograph-numeric;
--text-spacing-normal: normal;

/* 标点挤压 */
--text-punctuation-trim: allow-end;

/* 避头尾 */
--text-line-break: strict;
--text-word-break: break-all;

/* 中文正文排版 */
.chinese-body {
  font-family: var(--font-family-base);
  font-size: var(--font-size-base);
  line-height: 1.75; /* 中文正文推荐1.75行高 */
  letter-spacing: 0.02em; /* 中文正文微加字间距 */
  text-autospace: ideograph-alpha ideograph-numeric;
  text-spacing: normal;
  line-break: strict;
  word-break: break-all;
  punctuation-trim: allow-end;
}

/* 中文标题排版 */
.chinese-heading {
  font-family: var(--font-family-base);
  line-height: 1.3;
  letter-spacing: -0.02em;
  line-break: strict;
  word-break: keep-all; /* 标题禁止词内断行 */
}
```

---

## 动态字号

### iOS Dynamic Type

iOS支持Dynamic Type，用户可在设置中调整字号缩放比例，应用需适配所有预设尺寸：

| 内容样式 | 默认字号 | xSmall | Small | Large | xLarge | xxLarge | xxxLarge | Accessibility | Accessibility5 |
|----------|---------|--------|-------|-------|--------|---------|----------|---------------|----------------|
| Body | 17px | 14px | 15px | 18px | 19px | 21px | 23px | 28px | 53px |
| Headline | 17px | 14px | 15px | 18px | 19px | 21px | 23px | 28px | 53px |
| Subheadline | 15px | 12px | 13px | 16px | 17px | 19px | 21px | 26px | 49px |
| Footnote | 13px | 11px | 12px | 14px | 15px | 16px | 18px | 22px | 41px |
| Caption1 | 12px | 10px | 11px | 13px | 14px | 15px | 16px | 20px | 38px |
| Caption2 | 11px | 10px | 10px | 12px | 12px | 13px | 14px | 18px | 34px |
| Title1 | 28px | 23px | 25px | 30px | 32px | 34px | 38px | 46px | 88px |
| Title2 | 22px | 18px | 20px | 24px | 25px | 27px | 30px | 36px | 69px |
| Title3 | 20px | 17px | 18px | 21px | 23px | 24px | 27px | 33px | 63px |
| Large Title | 34px | 28px | 31px | 36px | 39px | 42px | 46px | 56px | 106px |

### Android Font Scale

Android通过Font Scale缩放字号，用户可在设置中调整：

| 缩放级别 | 缩放系数 | 14sp基准 | 16sp基准 | 20sp基准 | 说明 |
|----------|---------|---------|---------|---------|------|
| Small | 0.85 | 12px | 14px | 17px | 小字号模式 |
| Default | 1.0 | 14px | 16px | 20px | 默认模式 |
| Large | 1.15 | 16px | 18px | 23px | 大字号模式 |
| Largest | 1.3 | 18px | 21px | 26px | 超大字号模式 |

### HarmonyOS Font Scale

| 缩放级别 | 缩放系数 | 14fp基准 | 16fp基准 | 20fp基准 | 说明 |
|----------|---------|---------|---------|---------|------|
| Small | 0.85 | 12px | 14px | 17px | 小字号模式 |
| Default | 1.0 | 14px | 16px | 20px | 默认模式 |
| Large | 1.15 | 16px | 18px | 23px | 大字号模式 |
| Extra Large | 1.3 | 18px | 21px | 26px | 超大字号模式 |

### Windows Text Scaling

Windows支持文本缩放，范围100%-225%：

| 缩放级别 | 缩放系数 | 12px基准 | 14px基准 | 16px基准 | 说明 |
|----------|---------|---------|---------|---------|------|
| 100% | 1.0 | 12px | 14px | 16px | 默认 |
| 125% | 1.25 | 15px | 18px | 20px | 轻度放大 |
| 150% | 1.5 | 18px | 21px | 24px | 中度放大 |
| 175% | 1.75 | 21px | 25px | 28px | 较大放大 |
| 200% | 2.0 | 24px | 28px | 32px | 大幅放大 |
| 225% | 2.25 | 27px | 32px | 36px | 最大放大 |

### Web端动态字号CSS实现

```css
/* 基于rem的动态字号 */
html {
  font-size: 16px; /* 基准字号 */
}

/* 用户偏好字号覆盖 */
@media (prefers-reduced-motion: no-preference) {
  html {
    font-size: clamp(14px, 1vw + 12px, 20px);
  }
}

/* 基于clamp的响应式字号 */
--font-size-fluid-sm: clamp(12px, 0.8rem + 0.2vw, 14px);
--font-size-fluid-base: clamp(14px, 0.9rem + 0.3vw, 18px);
--font-size-fluid-lg: clamp(16px, 1rem + 0.4vw, 22px);
--font-size-fluid-xl: clamp(20px, 1.2rem + 0.5vw, 28px);
--font-size-fluid-2xl: clamp(24px, 1.4rem + 0.6vw, 36px);
--font-size-fluid-3xl: clamp(28px, 1.6rem + 0.8vw, 48px);
```

---

## 排版禁忌

### 孤行/孤字处理

| 禁忌类型 | 定义 | 处理规则 | CSS实现 |
|----------|------|----------|---------|
| 孤行(Orphan) | 段落最后一行仅1-2个字符数<=2 | 调整行宽或字间距使最后一行至少3个字符 | `orphans: 3` |
| 寡行(Widow) | 段落第一行仅字符数<=2 | 调整行宽或字间距使首行至少3个字符 | `widows: 3` |
| 孤字 | 中文段落最后一行仅1个汉字 | 调整字间距或行宽避免孤字 | `widows: 2; orphans: 2` + 手动调整 |
| 标题孤行 | 标题与正文分离(标题在页底，正文在下一页) | 标题后至少跟随2行正文 | `break-after: avoid` |

### 最小字号限制

| 平台 | 正文最小字号 | 辅助文字最小字号 | 标注最小字号 | 说明 |
|------|-------------|----------------|------------|------|
| iOS | 15px | 13px | 11px | Apple HIG推荐正文不低于15px |
| Android | 14sp | 12sp | 10sp | Material Design推荐正文不低于14sp |
| One UI | 14px | 12px | 10px | 基于Android标准 |
| HarmonyOS | 14fp | 12fp | 10fp | 鸿蒙设计规范 |
| HyperOS | 14px | 12px | 10px | 基于Android标准 |
| MagicOS | 14px | 12px | 10px | 基于Android标准 |
| ColorOS | 14px | 12px | 10px | 基于Android标准 |
| OriginOS | 14px | 12px | 10px | 基于Android标准 |
| Flyme | 14px | 12px | 10px | 基于Android标准 |
| Fluent | 12px | 11px | 10px | Fluent Design允许较小字号 |
| WeUI | 14px | 12px | 10px | 微信小程序规范 |

### 最大行宽限制

| 内容类型 | 手机最大行宽 | 平板最大行宽 | 桌面最大行宽 | 说明 |
|----------|-------------|-------------|-------------|------|
| 中文正文 | 560px(约35em) | 640px(约40em) | 720px(约45em) | 超过此宽度阅读效率下降 |
| 英文正文 | 480px(约30em) | 560px(约35em) | 640px(约40em) | 英文行宽比中文更窄 |
| 标题 | 不限 | 不限 | 不限 | 标题通常单行显示 |
| 列表项 | 屏幕宽度-32px | 屏幕宽度-64px | 屏幕宽度-96px | 列表项占满可用宽度 |
| 代码块 | 屏幕宽度-32px | 屏幕宽度-64px | 960px | 代码块允许更宽 |

### 排版禁忌CSS实现

```css
/* 孤行寡行控制 */
--orphans: 3;
--widows: 3;

/* 行宽控制 */
--max-width-body-cn: 45em;   /* 中文正文最大行宽 */
--max-width-body-en: 35em;   /* 英文正文最大行宽 */
--max-width-code: 60em;      /* 代码块最大行宽 */

/* 最小字号控制 */
--min-font-size-body: 14px;
--min-font-size-caption: 11px;

/* 标题断行控制 */
h1, h2, h3, h4, h5, h6 {
  break-after: avoid;
  break-inside: avoid;
}

/* 段落排版 */
p {
  orphans: 3;
  widows: 3;
  max-width: var(--max-width-body-cn);
}

/* 中文正文 */
.chinese-body {
  max-width: 45em;
  line-height: 1.75;
  orphans: 3;
  widows: 3;
  text-spacing: normal;
  line-break: strict;
}

/* 英文正文 */
.english-body {
  max-width: 35em;
  line-height: 1.6;
  orphans: 3;
  widows: 3;
  hyphens: auto;
  word-break: break-word;
}
```
