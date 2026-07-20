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
