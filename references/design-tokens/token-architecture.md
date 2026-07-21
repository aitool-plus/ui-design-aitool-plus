> @author aitool.plus

# Token 三层架构

## 架构概述

Token体系采用三层架构：Primitive Token（原始令牌）-> Semantic Token（语义令牌）-> Component Token（组件令牌），实现从原始值到语义角色再到具体组件的逐层映射。

---

## Primitive Token（原始令牌）

### 定义

Primitive Token是设计系统中最基础的数值定义，包含色值、字号、间距、圆角、阴影等原始值。

### 11大平台原始值对照表

#### 颜色原始值

| Token名称 | Apple iOS | Google Android | Samsung One UI | Huawei HarmonyOS | Xiaomi HyperOS | Honor MagicOS | OPPO ColorOS | vivo OriginOS | Meizu Flyme | Windows Fluent | WeChat WeUI |
|-----------|-----------|----------------|----------------|------------------|----------------|---------------|--------------|---------------|-------------|----------------|-------------|
| blue | #007AFF | #6750A4 | #1259C3 | #007DFF | #4A90D9 | #0066FF | #1BA784 | #415FFF | #00B4FF | #0078D4 | #07C160 |
| green | #34C759 | #4CAF50 | #00A86B | #00C853 | #00B050 | #00C853 | #2ECC71 | #00C853 | #00E676 | #107C10 | #07C160 |
| red | #FF3B30 | #F44336 | #E53935 | #CF0A2C | #FF6900 | #FF4444 | #E74C3C | #FF4444 | #FF5252 | #D13438 | #FA5151 |
| yellow | #FFCC00 | #FFC107 | #FFB300 | #FFB300 | #FFC107 | #FFC107 | #F1C40F | #FFC107 | #FFD740 | #FFB900 | #FFC300 |
| orange | #FF9500 | #FF9800 | #FF9800 | #FF9800 | #FF6900 | #FF9800 | #E67E22 | #FF9800 | #FFAB40 | #FF8C00 | #FF9500 |
| purple | #AF52DE | #9C27B0 | #7B1FA2 | #9C27B0 | #9C27B0 | #AF52DE | #8E44AD | #9C27B0 | #E040FB | #881798 | #9C27B0 |
| gray-100 | #F2F2F7 | #F5F5F5 | #F5F5F5 | #F5F5F5 | #F5F5F5 | #F5F5F5 | #F5F5F5 | #F5F5F5 | #F5F5F5 | #F3F2F1 | #F5F5F5 |
| gray-200 | #E5E5EA | #EEEEEE | #EEEEEE | #EEEEEE | #EEEEEE | #EEEEEE | #EEEEEE | #EEEEEE | #EEEEEE | #E1DFDD | #EEEEEE |
| gray-300 | #C7C7CC | #E0E0E0 | #E0E0E0 | #E0E0E0 | #E0E0E0 | #E0E0E0 | #E0E0E0 | #E0E0E0 | #E0E0E0 | #C8C6C4 | #E0E0E0 |
| gray-400 | #8E8E93 | #BDBDBD | #BDBDBD | #BDBDBD | #BDBDBD | #BDBDBD | #BDBDBD | #BDBDBD | #BDBDBD | #A19F9D | #BDBDBD |
| gray-500 | #636366 | #9E9E9E | #9E9E9E | #9E9E9E | #9E9E9E | #9E9E9E | #9E9E9E | #9E9E9E | #9E9E9E | #8A8886 | #9E9E9E |
| gray-600 | #48484A | #757575 | #757575 | #757575 | #757575 | #757575 | #757575 | #757575 | #757575 | #605E5C | #757575 |
| gray-700 | #3A3A3C | #616161 | #616161 | #616161 | #616161 | #616161 | #616161 | #616161 | #616161 | #3B3A39 | #616161 |
| gray-800 | #2C2C2E | #424242 | #424242 | #424242 | #424242 | #424242 | #424242 | #424242 | #424242 | #323130 | #424242 |
| gray-900 | #1C1C1E | #212121 | #212121 | #212121 | #212121 | #212121 | #212121 | #212121 | #212121 | #201F1E | #212121 |

#### 字号原始值（单位：px）

| Token名称 | Apple iOS | Google Android | Samsung One UI | Huawei HarmonyOS | Xiaomi HyperOS | Honor MagicOS | OPPO ColorOS | vivo OriginOS | Meizu Flyme | Windows Fluent | WeChat WeUI |
|-----------|-----------|----------------|----------------|------------------|----------------|---------------|--------------|---------------|-------------|----------------|-------------|
| text-xs | 11 | 12 | 11 | 11 | 11 | 11 | 11 | 11 | 11 | 12 | 11 |
| text-sm | 13 | 14 | 13 | 13 | 13 | 13 | 13 | 13 | 13 | 14 | 13 |
| text-base | 15 | 16 | 15 | 15 | 15 | 15 | 15 | 15 | 15 | 16 | 14 |
| text-lg | 17 | 18 | 17 | 17 | 17 | 17 | 17 | 17 | 17 | 18 | 16 |
| text-xl | 20 | 22 | 20 | 20 | 20 | 20 | 20 | 20 | 20 | 22 | 18 |
| text-2xl | 24 | 28 | 24 | 24 | 24 | 24 | 24 | 24 | 24 | 28 | 20 |
| text-3xl | 32 | 36 | 32 | 32 | 32 | 32 | 32 | 32 | 32 | 36 | 24 |

#### 间距原始值（单位：px）

| Token名称 | Apple iOS | Google Android | Samsung One UI | Huawei HarmonyOS | Xiaomi HyperOS | Honor MagicOS | OPPO ColorOS | vivo OriginOS | Meizu Flyme | Windows Fluent | WeChat WeUI |
|-----------|-----------|----------------|----------------|------------------|----------------|---------------|--------------|---------------|-------------|----------------|-------------|
| space-1 | 4 | 4 | 4 | 4 | 4 | 4 | 4 | 4 | 4 | 4 | 4 |
| space-2 | 8 | 8 | 8 | 8 | 8 | 8 | 8 | 8 | 8 | 8 | 8 |
| space-3 | 12 | 12 | 12 | 12 | 12 | 12 | 12 | 12 | 12 | 12 | 12 |
| space-4 | 16 | 16 | 16 | 16 | 16 | 16 | 16 | 16 | 16 | 16 | 16 |
| space-5 | 20 | 20 | 20 | 20 | 20 | 20 | 20 | 20 | 20 | 20 | 20 |
| space-6 | 24 | 24 | 24 | 24 | 24 | 24 | 24 | 24 | 24 | 24 | 24 |
| space-8 | 32 | 32 | 32 | 32 | 32 | 32 | 32 | 32 | 32 | 32 | 32 |
| space-10 | 40 | 40 | 40 | 40 | 40 | 40 | 40 | 40 | 40 | 40 | 40 |
| space-12 | 48 | 48 | 48 | 48 | 48 | 48 | 48 | 48 | 48 | 48 | 48 |

#### 圆角原始值（单位：px）

| Token名称 | Apple iOS | Google Android | Samsung One UI | Huawei HarmonyOS | Xiaomi HyperOS | Honor MagicOS | OPPO ColorOS | vivo OriginOS | Meizu Flyme | Windows Fluent | WeChat WeUI |
|-----------|-----------|----------------|----------------|------------------|----------------|---------------|--------------|---------------|-------------|----------------|-------------|
| radius-sm | 4 | 4 | 4 | 4 | 4 | 4 | 4 | 4 | 4 | 2 | 4 |
| radius-md | 8 | 8 | 8 | 8 | 8 | 8 | 8 | 8 | 8 | 4 | 8 |
| radius-lg | 12 | 12 | 12 | 12 | 12 | 12 | 12 | 12 | 12 | 8 | 12 |
| radius-xl | 16 | 16 | 16 | 16 | 16 | 16 | 16 | 16 | 16 | 8 | 16 |
| radius-full | 9999 | 9999 | 9999 | 9999 | 9999 | 9999 | 9999 | 9999 | 9999 | 9999 | 9999 |

---

## Semantic Token（语义令牌）

### 定义

Semantic Token将Primitive Token映射为具有语义角色的变量，描述颜色/间距等在UI中的用途。

### 颜色语义映射

```css
/* 主色 */
--color-primary: var(--primitive-blue);
--color-primary-hover: var(--primitive-blue-dark);
--color-primary-active: var(--primitive-blue-darker);
--color-primary-disabled: var(--primitive-blue-light);

/* 次色 */
--color-secondary: var(--primitive-purple);
--color-secondary-hover: var(--primitive-purple-dark);

/* 背景色 */
--color-background: var(--primitive-gray-100);
--color-background-surface: var(--primitive-white);
--color-background-elevated: var(--primitive-white);

/* 文字色 */
--color-text-primary: var(--primitive-gray-900);
--color-text-secondary: var(--primitive-gray-500);
--color-text-tertiary: var(--primitive-gray-400);
--color-text-disabled: var(--primitive-gray-300);

/* 功能色 */
--color-success: var(--primitive-green);
--color-warning: var(--primitive-yellow);
--color-error: var(--primitive-red);
--color-info: var(--primitive-blue);

/* 分隔线 */
--color-border: var(--primitive-gray-200);
--color-border-strong: var(--primitive-gray-300);
```

### 各平台语义映射对照

| 语义Token | Apple iOS | Google Android | Samsung One UI | Huawei HarmonyOS | Xiaomi HyperOS | Honor MagicOS | OPPO ColorOS | vivo OriginOS | Meizu Flyme | Windows Fluent | WeChat WeUI |
|-----------|-----------|----------------|----------------|------------------|----------------|---------------|--------------|---------------|-------------|----------------|-------------|
| --color-primary | #007AFF | #6750A4 | #1259C3 | #007DFF | #4A90D9 | #0066FF | #1BA784 | #415FFF | #00B4FF | #0078D4 | #07C160 |
| --color-secondary | #5856D6 | #03DAC6 | #00A86B | #00C853 | #00B050 | #00C853 | #2ECC71 | #00C853 | #00E676 | #107C10 | #07C160 |
| --color-background | #F2F2F7 | #F5F5F5 | #F5F5F5 | #F5F5F5 | #F5F5F5 | #F5F5F5 | #F5F5F5 | #F5F5F5 | #F5F5F5 | #F3F2F1 | #F5F5F5 |
| --color-text-primary | #000000 | #212121 | #212121 | #212121 | #212121 | #212121 | #212121 | #212121 | #212121 | #201F1E | #212121 |
| --color-text-secondary | #8E8E93 | #757575 | #757575 | #757575 | #757575 | #757575 | #757575 | #757575 | #757575 | #605E5C | #757575 |
| --color-success | #34C759 | #4CAF50 | #00A86B | #00C853 | #00B050 | #00C853 | #2ECC71 | #00C853 | #00E676 | #107C10 | #07C160 |
| --color-warning | #FFCC00 | #FFC107 | #FFB300 | #FFB300 | #FFC107 | #FFC107 | #F1C40F | #FFC107 | #FFD740 | #FFB900 | #FFC300 |
| --color-error | #FF3B30 | #F44336 | #E53935 | #CF0A2C | #FF6900 | #FF4444 | #E74C3C | #FF4444 | #FF5252 | #D13438 | #FA5151 |
| --color-border | #E5E5EA | #EEEEEE | #EEEEEE | #EEEEEE | #EEEEEE | #EEEEEE | #EEEEEE | #EEEEEE | #EEEEEE | #E1DFDD | #EEEEEE |

---

## Component Token（组件令牌）

### 定义

Component Token将Semantic Token映射到具体组件，定义组件各部分的样式值。

### 按钮组件Token

```css
/* 主按钮 */
--button-primary-bg: var(--color-primary);
--button-primary-text: var(--color-white);
--button-primary-border: none;
--button-primary-radius: var(--radius-md);
--button-primary-padding: var(--space-3) var(--space-5);
--button-primary-font-size: var(--text-base);
--button-primary-font-weight: var(--font-weight-medium);
--button-primary-height: 48px;

/* 次按钮 */
--button-secondary-bg: var(--color-background);
--button-secondary-text: var(--color-primary);
--button-secondary-border: 1px solid var(--color-primary);

/* 文字按钮 */
--button-text-text: var(--color-primary);
--button-text-bg: transparent;

/* 禁用状态 */
--button-disabled-bg: var(--color-background);
--button-disabled-text: var(--color-text-disabled);
--button-disabled-border: 1px solid var(--color-border);
```

### 输入框组件Token

```css
--input-bg: var(--color-background-surface);
--input-text: var(--color-text-primary);
--input-placeholder: var(--color-text-tertiary);
--input-border: 1px solid var(--color-border);
--input-border-focus: 1px solid var(--color-primary);
--input-border-error: 1px solid var(--color-error);
--input-radius: var(--radius-md);
--input-padding: var(--space-3) var(--space-4);
--input-font-size: var(--text-base);
--input-height: 48px;
```

### 卡片组件Token

```css
--card-bg: var(--color-background-surface);
--card-text: var(--color-text-primary);
--card-border: none;
--card-radius: var(--radius-lg);
--card-padding: var(--space-5);
--card-shadow: var(--shadow-sm);
--card-shadow-hover: var(--shadow-md);
```

---

## 深色模式覆盖规则

### 覆盖策略

深色模式下，Primitive Token保持不变，Semantic Token和Component Token通过CSS变量覆盖实现切换。

### 深色模式映射表

| 语义Token | 浅色模式值 | 深色模式值 |
|-----------|-----------|-----------|
| --color-background | #F2F2F7 | #1C1C1E |
| --color-background-surface | #FFFFFF | #2C2C2E |
| --color-background-elevated | #FFFFFF | #3A3A3C |
| --color-text-primary | #000000 | #FFFFFF |
| --color-text-secondary | #8E8E93 | #8E8E93 |
| --color-text-tertiary | #C7C7CC | #636366 |
| --color-border | #E5E5EA | #3A3A3C |
| --color-border-strong | #C7C7CC | #48484A |

### CSS实现方式

```css
:root {
  /* 浅色模式默认值 */
  --color-background: #F2F2F7;
  --color-background-surface: #FFFFFF;
  --color-text-primary: #000000;
  /* ... */
}

@media (prefers-color-scheme: dark) {
  :root {
    --color-background: #1C1C1E;
    --color-background-surface: #2C2C2E;
    --color-text-primary: #FFFFFF;
    /* ... */
  }
}

/* 手动切换类名 */
[data-theme="dark"] {
  --color-background: #1C1C1E;
  --color-background-surface: #2C2C2E;
  --color-text-primary: #FFFFFF;
  /* ... */
}
```

---

## Token命名规范

### 命名格式

```
--{category}-{property}-{variant}-{state}
```

### 命名规则

- **category**：颜色/间距/字体/圆角/阴影等大类
- **property**：具体属性（bg/text/border/padding等）
- **variant**：变体（primary/secondary/success等）
- **state**：状态（hover/active/disabled/focus等）

### 命名示例

```css
/* 颜色Token */
--color-primary: #007AFF;
--color-primary-hover: #0051D5;
--color-primary-active: #0047B8;
--color-primary-disabled: #B3D7FF;

/* 间距Token */
--spacing-1: 4px;
--spacing-2: 8px;
--spacing-3: 12px;
--spacing-4: 16px;

/* 字体Token */
--font-size-sm: 13px;
--font-size-base: 15px;
--font-size-lg: 17px;
--font-weight-regular: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;

/* 圆角Token */
--radius-sm: 4px;
--radius-md: 8px;
--radius-lg: 12px;
--radius-xl: 16px;
--radius-full: 9999px;

/* 阴影Token */
--shadow-sm: 0 1px 2px rgba(0,0,0,0.05);
--shadow-md: 0 4px 6px rgba(0,0,0,0.1);
--shadow-lg: 0 10px 15px rgba(0,0,0,0.1);
--shadow-xl: 0 20px 25px rgba(0,0,0,0.15);
```

---

## CSS变量输出格式示例

### 完整CSS变量定义

```css
:root {
  /* Primitive Tokens */
  --primitive-blue: #007AFF;
  --primitive-green: #34C759;
  --primitive-red: #FF3B30;
  --primitive-yellow: #FFCC00;
  --primitive-orange: #FF9500;
  --primitive-purple: #AF52DE;
  --primitive-gray-100: #F2F2F7;
  --primitive-gray-200: #E5E5EA;
  --primitive-gray-300: #C7C7CC;
  --primitive-gray-400: #8E8E93;
  --primitive-gray-500: #636366;
  --primitive-gray-600: #48484A;
  --primitive-gray-700: #3A3A3C;
  --primitive-gray-800: #2C2C2E;
  --primitive-gray-900: #1C1C1E;

  /* Semantic Tokens - 颜色 */
  --color-primary: var(--primitive-blue);
  --color-secondary: var(--primitive-purple);
  --color-background: var(--primitive-gray-100);
  --color-background-surface: #FFFFFF;
  --color-text-primary: #000000;
  --color-text-secondary: var(--primitive-gray-400);
  --color-text-tertiary: var(--primitive-gray-300);
  --color-text-disabled: var(--primitive-gray-300);
  --color-success: var(--primitive-green);
  --color-warning: var(--primitive-yellow);
  --color-error: var(--primitive-red);
  --color-info: var(--primitive-blue);
  --color-border: var(--primitive-gray-200);
  --color-border-strong: var(--primitive-gray-300);

  /* Semantic Tokens - 字体 */
  --font-family-base: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  --font-size-xs: 11px;
  --font-size-sm: 13px;
  --font-size-base: 15px;
  --font-size-lg: 17px;
  --font-size-xl: 20px;
  --font-size-2xl: 24px;
  --font-size-3xl: 32px;
  --font-weight-regular: 400;
  --font-weight-medium: 500;
  --font-weight-semibold: 600;
  --font-weight-bold: 700;
  --line-height-tight: 1.25;
  --line-height-normal: 1.5;
  --line-height-relaxed: 1.75;

  /* Semantic Tokens - 间距 */
  --spacing-1: 4px;
  --spacing-2: 8px;
  --spacing-3: 12px;
  --spacing-4: 16px;
  --spacing-5: 20px;
  --spacing-6: 24px;
  --spacing-8: 32px;
  --spacing-10: 40px;
  --spacing-12: 48px;

  /* Semantic Tokens - 圆角 */
  --radius-sm: 4px;
  --radius-md: 8px;
  --radius-lg: 12px;
  --radius-xl: 16px;
  --radius-full: 9999px;

  /* Semantic Tokens - 阴影 */
  --shadow-sm: 0 1px 2px rgba(0,0,0,0.05);
  --shadow-md: 0 4px 6px rgba(0,0,0,0.1);
  --shadow-lg: 0 10px 15px rgba(0,0,0,0.1);
  --shadow-xl: 0 20px 25px rgba(0,0,0,0.15);

  /* Component Tokens - 按钮 */
  --button-primary-bg: var(--color-primary);
  --button-primary-text: #FFFFFF;
  --button-primary-border: none;
  --button-primary-radius: var(--radius-md);
  --button-primary-padding: 12px 24px;
  --button-primary-font-size: var(--font-size-base);
  --button-primary-font-weight: var(--font-weight-medium);
  --button-primary-height: 48px;

  /* Component Tokens - 输入框 */
  --input-bg: var(--color-background-surface);
  --input-text: var(--color-text-primary);
  --input-placeholder: var(--color-text-tertiary);
  --input-border: 1px solid var(--color-border);
  --input-border-focus: 1px solid var(--color-primary);
  --input-border-error: 1px solid var(--color-error);
  --input-radius: var(--radius-md);
  --input-padding: 12px 16px;
  --input-font-size: var(--font-size-base);
  --input-height: 48px;

  /* Component Tokens - 卡片 */
  --card-bg: var(--color-background-surface);
  --card-text: var(--color-text-primary);
  --card-border: none;
  --card-radius: var(--radius-lg);
  --card-padding: 20px;
  --card-shadow: var(--shadow-sm);
  --card-shadow-hover: var(--shadow-md);
}
```

---

## Token命名规范详解

### 三层命名体系

Token命名遵循 Primitive -> Semantic -> Component 三层架构，每层有独立的命名规则和约束。

#### Primitive Token 命名规则

命名模板：

```
--{category}-{value-descriptor}
```

- category：颜色(color)、字号(font-size)、字重(font-weight)、行高(line-height)、间距(spacing)、圆角(radius)、阴影(shadow)
- value-descriptor：具体数值描述，如 blue、gray-500、12、md

命名示例：

```css
/* 颜色原始值 */
--color-blue: #007AFF;
--color-blue-50: #E3F2FD;
--color-blue-100: #BBDEFB;
--color-blue-200: #90CAF9;
--color-blue-300: #64B5F6;
--color-blue-400: #42A5F5;
--color-blue-500: #2196F3;
--color-blue-600: #1E88E5;
--color-blue-700: #1565C0;
--color-blue-800: #0D47A1;
--color-blue-900: #0A2472;
--color-gray-50: #FAFAFA;
--color-gray-100: #F5F5F5;
--color-gray-200: #EEEEEE;
--color-gray-300: #E0E0E0;
--color-gray-400: #BDBDBD;
--color-gray-500: #9E9E9E;
--color-gray-600: #757575;
--color-gray-700: #616161;
--color-gray-800: #424242;
--color-gray-900: #212121;

/* 字号原始值 */
--font-size-11: 11px;
--font-size-12: 12px;
--font-size-13: 13px;
--font-size-14: 14px;
--font-size-15: 15px;
--font-size-16: 16px;
--font-size-17: 17px;
--font-size-18: 18px;
--font-size-20: 20px;
--font-size-22: 22px;
--font-size-24: 24px;
--font-size-28: 28px;
--font-size-32: 32px;
--font-size-36: 36px;
--font-size-40: 40px;
--font-size-48: 48px;
--font-size-56: 56px;

/* 间距原始值 */
--spacing-0: 0px;
--spacing-4: 4px;
--spacing-8: 8px;
--spacing-12: 12px;
--spacing-16: 16px;
--spacing-20: 20px;
--spacing-24: 24px;
--spacing-32: 32px;
--spacing-40: 40px;
--spacing-48: 48px;
--spacing-64: 64px;
--spacing-80: 80px;
--spacing-96: 96px;

/* 圆角原始值 */
--radius-2: 2px;
--radius-4: 4px;
--radius-6: 6px;
--radius-8: 8px;
--radius-12: 12px;
--radius-16: 16px;
--radius-20: 20px;
--radius-24: 24px;
--radius-9999: 9999px;

/* 阴影原始值 */
--shadow-0: none;
--shadow-1: 0 1px 2px rgba(0,0,0,0.05);
--shadow-2: 0 4px 6px rgba(0,0,0,0.07);
--shadow-3: 0 10px 15px rgba(0,0,0,0.1);
--shadow-4: 0 20px 25px rgba(0,0,0,0.1);
--shadow-5: 0 25px 50px rgba(0,0,0,0.15);
```

#### Semantic Token 命名规则

命名模板：

```
--{category}-{property}-{variant}-{state}
```

- category：color、font、spacing、radius、shadow、motion
- property：bg(background)、text、border、padding、margin、size
- variant：primary、secondary、tertiary、success、warning、error、info
- state：default(可省略)、hover、active、focus、disabled、selected、pressed

完整命名示例：

```css
/* 颜色语义Token - 完整命名 */
--color-bg-primary: #FFFFFF;
--color-bg-secondary: #F5F5F5;
--color-bg-tertiary: #EEEEEE;
--color-bg-elevated: #FFFFFF;
--color-bg-inverse: #212121;

--color-text-primary: #212121;
--color-text-secondary: #757575;
--color-text-tertiary: #BDBDBD;
--color-text-disabled: #BDBDBD;
--color-text-inverse: #FFFFFF;
--color-text-link: #007AFF;

--color-border-primary: #E0E0E0;
--color-border-secondary: #EEEEEE;
--color-border-focus: #007AFF;
--color-border-error: #F44336;

--color-fill-primary: #007AFF;
--color-fill-primary-hover: #0051D5;
--color-fill-primary-active: #0047B8;
--color-fill-primary-disabled: #B3D7FF;
--color-fill-secondary: #5856D6;
--color-fill-tertiary: #8E8E93;

--color-functional-success: #34C759;
--color-functional-success-bg: #E8F5E9;
--color-functional-warning: #FFCC00;
--color-functional-warning-bg: #FFF8E1;
--color-functional-error: #FF3B30;
--color-functional-error-bg: #FFEBEE;
--color-functional-info: #007AFF;
--color-functional-info-bg: #E3F2FD;

/* 字体语义Token */
--font-text-primary: var(--font-size-15);
--font-text-secondary: var(--font-size-13);
--font-text-caption: var(--font-size-11);
--font-text-overline: var(--font-size-10);
--font-heading-1: var(--font-size-48);
--font-heading-2: var(--font-size-32);
--font-heading-3: var(--font-size-24);
--font-heading-4: var(--font-size-20);
--font-heading-5: var(--font-size-17);
--font-heading-6: var(--font-size-15);

/* 间距语义Token */
--spacing-page-horizontal: var(--spacing-16);
--spacing-page-vertical: var(--spacing-24);
--spacing-section: var(--spacing-32);
--spacing-group: var(--spacing-16);
--spacing-element: var(--spacing-8);
--spacing-inline: var(--spacing-4);

/* 圆角语义Token */
--radius-button: var(--radius-8);
--radius-card: var(--radius-12);
--radius-dialog: var(--radius-16);
--radius-input: var(--radius-8);
--radius-avatar: var(--radius-9999);
--radius-badge: var(--radius-9999);
--radius-tooltip: var(--radius-4);
--radius-chip: var(--radius-9999);
```

#### Component Token 命名规则

命名模板：

```
--{component}-{property}-{variant}-{state}
```

- component：button、input、card、dialog、list、nav、tab、badge、chip、avatar、alert、toast、tooltip、switch、checkbox、radio、slider、progress、tag
- property：bg、text、border、icon、padding、height、width、radius、shadow、font-size、font-weight
- variant：primary、secondary、text、outline、ghost、danger、success、small、medium、large
- state：default(可省略)、hover、active、focus、disabled、selected、pressed、loading、error

完整命名示例：

```css
/* 按钮组件Token */
--button-primary-bg: var(--color-fill-primary);
--button-primary-bg-hover: var(--color-fill-primary-hover);
--button-primary-bg-active: var(--color-fill-primary-active);
--button-primary-bg-disabled: var(--color-fill-primary-disabled);
--button-primary-text: #FFFFFF;
--button-primary-text-disabled: rgba(255,255,255,0.5);
--button-primary-border: none;
--button-primary-radius: var(--radius-button);
--button-primary-padding-horizontal: var(--spacing-16);
--button-primary-padding-vertical: var(--spacing-8);
--button-primary-height: 44px;
--button-primary-font-size: var(--font-size-15);
--button-primary-font-weight: 500;
--button-primary-icon-size: 20px;
--button-primary-icon-gap: var(--spacing-8);

--button-secondary-bg: transparent;
--button-secondary-bg-hover: rgba(0,122,255,0.08);
--button-secondary-text: var(--color-fill-primary);
--button-secondary-text-disabled: var(--color-fill-primary-disabled);
--button-secondary-border: 1px solid var(--color-fill-primary);
--button-secondary-border-disabled: 1px solid var(--color-fill-primary-disabled);

--button-text-bg: transparent;
--button-text-bg-hover: rgba(0,122,255,0.08);
--button-text-text: var(--color-fill-primary);
--button-text-text-disabled: var(--color-fill-primary-disabled);

--button-danger-bg: var(--color-functional-error);
--button-danger-bg-hover: #D32F2F;
--button-danger-text: #FFFFFF;

--button-small-height: 32px;
--button-small-padding-horizontal: var(--spacing-12);
--button-small-padding-vertical: var(--spacing-4);
--button-small-font-size: var(--font-size-13);

--button-large-height: 52px;
--button-large-padding-horizontal: var(--spacing-24);
--button-large-padding-vertical: var(--spacing-12);
--button-large-font-size: var(--font-size-17);

/* 输入框组件Token */
--input-bg: var(--color-bg-primary);
--input-bg-disabled: var(--color-bg-tertiary);
--input-text: var(--color-text-primary);
--input-text-disabled: var(--color-text-disabled);
--input-placeholder: var(--color-text-tertiary);
--input-border: 1px solid var(--color-border-primary);
--input-border-hover: 1px solid var(--color-text-secondary);
--input-border-focus: 2px solid var(--color-fill-primary);
--input-border-error: 2px solid var(--2px solid var(--color-functional-error));
--input-radius: var(--radius-input);
--input-padding-horizontal: var(--spacing-16);
--input-padding-vertical: var(--spacing-12);
--input-height: 44px;
--input-font-size: var(--font-size-15);
--input-label-font-size: var(--font-size-13);
--input-label-color: var(--color-text-secondary);
--input-error-text-font-size: var(--font-size-12);
--input-error-text-color: var(--color-functional-error);
--input-icon-size: 20px;
--input-icon-color: var(--color-text-tertiary);

/* 卡片组件Token */
--card-bg: var(--color-bg-primary);
--card-bg-hover: var(--color-bg-primary);
--card-text: var(--color-text-primary);
--card-text-secondary: var(--color-text-secondary);
--card-border: 1px solid var(--color-border-secondary);
--card-radius: var(--radius-card);
--card-padding: var(--spacing-16);
--card-padding-horizontal: var(--spacing-16);
--card-padding-vertical: var(--spacing-16);
--card-shadow: var(--shadow-1);
--card-shadow-hover: var(--shadow-2);
--card-header-font-size: var(--font-size-17);
--card-header-font-weight: 600;
--card-body-font-size: var(--font-size-15);
--card-footer-font-size: var(--font-size-13);

/* 对话框组件Token */
--dialog-bg: var(--color-bg-elevated);
--dialog-text: var(--color-text-primary);
--dialog-border: none;
--dialog-radius: var(--radius-dialog);
--dialog-padding: var(--spacing-24);
--dialog-shadow: var(--shadow-5);
--dialog-title-font-size: var(--font-size-20);
--dialog-title-font-weight: 600;
--dialog-body-font-size: var(--font-size-15);
--dialog-action-gap: var(--spacing-8);
--dialog-width: 320px;
--dialog-width-tablet: 560px;

/* 列表项组件Token */
--list-item-bg: var(--color-bg-primary);
--list-item-bg-hover: rgba(0,0,0,0.04);
--list-item-bg-active: rgba(0,0,0,0.08);
--list-item-text: var(--color-text-primary);
--list-item-text-secondary: var(--color-text-secondary);
--list-item-border: 1px solid var(--color-border-secondary);
--list-item-padding-horizontal: var(--spacing-16);
--list-item-padding-vertical: var(--spacing-12);
--list-item-height: 48px;
--list-item-height-dense: 36px;
--list-item-height-three-line: 72px;
--list-item-icon-size: 24px;
--list-item-icon-gap: var(--spacing-16);
--list-item-avatar-size: 40px;
--list-item-avatar-gap: var(--spacing-12);
```

### 命名约束规则

1. 全部使用小写字母，单词间以连字符(-)连接
2. 禁止使用缩写，除通用缩写外(bg、fg、btn、nav、tab、dlg、chk、rdo、sel)
3. 状态后缀统一：hover、active、focus、disabled、selected、pressed、loading、error
4. 尺寸后缀统一：xs、sm、md、lg、xl
5. 层级后缀统一：primary、secondary、tertiary
6. 同一组件的所有Token必须以组件名作为统一前缀
7. Component Token必须引用Semantic Token，禁止直接引用Primitive Token
8. Semantic Token必须引用Primitive Token，禁止硬编码数值

---

## 11大平台Token映射表

### 颜色语义Token跨平台映射

| 语义Token | iOS | Android | One UI | HarmonyOS | HyperOS | MagicOS | ColorOS | OriginOS | Flyme | Fluent | WeUI |
|-----------|-----|---------|--------|-----------|---------|---------|---------|----------|-------|--------|------|
| --color-primary | #007AFF | #6750A4 | #1259C3 | #007DFF | #4A90D9 | #0066FF | #1BA784 | #415FFF | #00B4FF | #0078D4 | #07C160 |
| --color-primary-hover | #0051D5 | #7965B3 | #3A7FDB | #3399FF | #6AA8E8 | #3385FF | #4DC9A3 | #6B7FFF | #33C5FF | #1A86D9 | #2FD66D |
| --color-primary-active | #0047B8 | #5A3D8A | #0D3F8F | #005CC8 | #3A7BC0 | #004FCC | #148F6E | #3247E0 | #0090D9 | #005A9E | #06A94E |
| --color-primary-disabled | #B3D7FF | #D0BCFF | #89B8E8 | #99CCFF | #A8C8E8 | #99C2FF | #8DD4BF | #A0ABFF | #80DAFF | #99CEF0 | #80E0B0 |
| --color-secondary | #5856D6 | #03DAC6 | #00A86B | #CF0A2C | #FF6900 | #C9A96E | #2ECC71 | #00C853 | #00E676 | #107C10 | #10AEFF |
| --color-bg-page | #F2F2F7 | #F5F5F5 | #F5F5F5 | #F5F5F5 | #F5F5F5 | #F5F5F5 | #F5F5F5 | #F5F5F5 | #F5F5F5 | #F3F2F1 | #F5F5F5 |
| --color-bg-card | #FFFFFF | #FFFFFF | #FFFFFF | #FFFFFF | #FFFFFF | #FFFFFF | #FFFFFF | #FFFFFF | #FFFFFF | #FFFFFF | #FFFFFF |
| --color-bg-elevated | #FFFFFF | #FFFFFF | #FFFFFF | #FFFFFF | #FFFFFF | #FFFFFF | #FFFFFF | #FFFFFF | #FFFFFF | #FFFFFF | #FFFFFF |
| --color-text-primary | #000000 | #212121 | #212121 | #212121 | #212121 | #212121 | #212121 | #212121 | #212121 | #201F1E | #212121 |
| --color-text-secondary | #8E8E93 | #757575 | #757575 | #757575 | #757575 | #757575 | #757575 | #757575 | #757575 | #605E5C | #757575 |
| --color-text-tertiary | #C7C7CC | #BDBDBD | #BDBDBD | #BDBDBD | #BDBDBD | #BDBDBD | #BDBDBD | #BDBDBD | #BDBDBD | #A19F9D | #BDBDBD |
| --color-text-disabled | #C7C7CC | #BDBDBD | #BDBDBD | #BDBDBD | #BDBDBD | #BDBDBD | #BDBDBD | #BDBDBD | #BDBDBD | #A19F9D | #BDBDBD |
| --color-border | #E5E5EA | #EEEEEE | #EEEEEE | #EEEEEE | #EEEEEE | #EEEEEE | #EEEEEE | #EEEEEE | #EEEEEE | #E1DFDD | #EEEEEE |
| --color-success | #34C759 | #4CAF50 | #00A86B | #00C853 | #00B050 | #00C853 | #2ECC71 | #00C853 | #00E676 | #107C10 | #07C160 |
| --color-warning | #FFCC00 | #FFC107 | #FFB300 | #FFB300 | #FFC107 | #FFB300 | #F1C40F | #FFC107 | #FFD740 | #FFB900 | #FFC300 |
| --color-error | #FF3B30 | #F44336 | #E53935 | #CF0A2C | #FF6900 | #FF4444 | #E74C3C | #FF4444 | #FF5252 | #D13438 | #FA5151 |
| --color-info | #007AFF | #2196F3 | #1259C3 | #1259C3 | #007DFF | #4A90D9 | #0066FF | #1BA784 | #415FFF | #00B4FF | #0078D4 | #10AEFF |

### 字号语义Token跨平台映射

| 语义Token | iOS | Android | One UI | HarmonyOS | HyperOS | MagicOS | ColorOS | OriginOS | Flyme | Fluent | WeUI |
|-----------|-----|---------|--------|-----------|---------|---------|---------|----------|-------|--------|------|
| --font-display-large | 48px | 57px | 48px | 48px | 48px | 48px | 48px | 48px | 48px | 68px | 32px |
| --font-display-medium | 40px | 45px | 40px | 40px | 40px | 40px | 40px | 40px | 40px | 48px | 28px |
| --font-display-small | 32px | 36px | 32px | 32px | 32px | 32px | 32px | 32px | 32px | 40px | 24px |
| --font-headline-large | 28px | 32px | 28px | 28px | 28px | 28px | 28px | 28px | 28px | 32px | 22px |
| --font-headline-medium | 24px | 28px | 24px | 24px | 24px | 24px | 24px | 24px | 24px | 28px | 20px |
| --font-headline-small | 20px | 24px | 20px | 20px | 20px | 20px | 20px | 20px | 20px | 24px | 18px |
| --font-title-large | 17px | 22px | 17px | 17px | 17px | 17px | 17px | 17px | 17px | 20px | 17px |
| --font-title-medium | 15px | 16px | 15px | 15px | 15px | 15px | 15px | 15px | 15px | 16px | 16px |
| --font-title-small | 13px | 14px | 13px | 13px | 13px | 13px | 13px | 13px | 13px | 14px | 14px |
| --font-body-large | 17px | 16px | 17px | 17px | 17px | 17px | 17px | 17px | 17px | 16px | 17px |
| --font-body-medium | 15px | 14px | 15px | 15px | 15px | 15px | 15px | 15px | 15px | 14px | 15px |
| --font-body-small | 13px | 12px | 13px | 13px | 13px | 13px | 13px | 13px | 13px | 12px | 13px |
| --font-label-large | 15px | 14px | 15px | 15px | 15px | 15px | 15px | 15px | 15px | 14px | 14px |
| --font-label-medium | 13px | 12px | 13px | 13px | 13px | 13px | 13px | 13px | 13px | 12px | 12px |
| --font-label-small | 11px | 11px | 11px | 11px | 11px | 11px | 11px | 11px | 11px | 10px | 10px |
| --font-caption | 11px | 12px | 11px | 11px | 11px | 11px | 11px | 11px | 11px | 12px | 10px |
| --font-overline | 10px | 10px | 10px | 10px | 10px | 10px | 10px | 10px | 10px | 10px | 10px |

### 间距语义Token跨平台映射

| 语义Token | iOS | Android | One UI | HarmonyOS | HyperOS | MagicOS | ColorOS | OriginOS | Flyme | Fluent | WeUI |
|-----------|-----|---------|--------|-----------|---------|---------|---------|----------|-------|--------|------|
| --spacing-page-h | 16px | 16dp | 16px | 16px | 16px | 16px | 16px | 16px | 16px | 16px | 16px |
| --spacing-page-v | 24px | 24dp | 24px | 24px | 24px | 24px | 24px | 24px | 24px | 24px | 24px |
| --spacing-section | 32px | 32dp | 32px | 32px | 32px | 32px | 32px | 32px | 32px | 32px | 32px |
| --spacing-group | 16px | 16dp | 16px | 16px | 16px | 16px | 16px | 16px | 16px | 16px | 16px |
| --spacing-element | 8px | 8dp | 8px | 8px | 8px | 8px | 8px | 8px | 8px | 8px | 8px |
| --spacing-inline | 4px | 4dp | 4px | 4px | 4px | 4px | 4px | 4px | 4px | 4px | 4px |
| --spacing-card-padding | 16px | 16dp | 16px | 16px | 16px | 16px | 16px | 16px | 16px | 16px | 16px |
| --spacing-list-item-h | 16px | 16dp | 16px | 16px | 16px | 16px | 16px | 16px | 16px | 16px | 16px |
| --spacing-list-item-v | 12px | 12dp | 12px | 12px | 12px | 12px | 12px | 12px | 12px | 12px | 12px |

### 圆角语义Token跨平台映射

| 语义Token | iOS | Android | One UI | HarmonyOS | HyperOS | MagicOS | ColorOS | OriginOS | Flyme | Fluent | WeUI |
|-----------|-----|---------|--------|-----------|---------|---------|---------|----------|-------|--------|------|
| --radius-button | 8px | 8dp | 8px | 8px | 8px | 8px | 8px | 8px | 8px | 4px | 8px |
| --radius-card | 12px | 12dp | 12px | 16px | 12px | 12px | 12px | 12px | 12px | 8px | 12px |
| --radius-dialog | 16px | 28dp | 16px | 24px | 16px | 16px | 16px | 16px | 16px | 8px | 16px |
| --radius-input | 8px | 4dp | 8px | 8px | 8px | 8px | 8px | 8px | 8px | 4px | 4px |
| --radius-avatar | 9999px | 9999dp | 9999px | 9999px | 9999px | 9999px | 9999px | 9999px | 9999px | 9999px | 9999px |
| --radius-chip | 9999px | 8dp | 9999px | 9999px | 9999px | 9999px | 9999px | 9999px | 9999px | 9999px | 9999px |
| --radius-tooltip | 4px | 4dp | 4px | 4px | 4px | 4px | 4px | 4px | 4px | 4px | 4px |
| --radius-bottom-sheet | 16px | 28dp | 16px | 16px | 16px | 16px | 16px | 16px | 16px | 8px | 16px |

---

## Token导出格式

### CSS变量格式

```css
/* ============================================
   Design Tokens - CSS Custom Properties
   Version: 1.0.0
   Generated: 2026-07-20
   ============================================ */

:root {
  /* ---- Primitive Tokens ---- */
  --color-blue-50: #E3F2FD;
  --color-blue-100: #BBDEFB;
  --color-blue-200: #90CAF9;
  --color-blue-300: #64B5F6;
  --color-blue-400: #42A5F5;
  --color-blue-500: #2196F3;
  --color-blue-600: #1E88E5;
  --color-blue-700: #1565C0;
  --color-blue-800: #0D47A1;
  --color-blue-900: #0A2472;

  --color-gray-50: #FAFAFA;
  --color-gray-100: #F5F5F5;
  --color-gray-200: #EEEEEE;
  --color-gray-300: #E0E0E0;
  --color-gray-400: #BDBDBD;
  --color-gray-500: #9E9E9E;
  --color-gray-600: #757575;
  --color-gray-700: #616161;
  --color-gray-800: #424242;
  --color-gray-900: #212121;

  --color-green-500: #4CAF50;
  --color-red-500: #F44336;
  --color-yellow-500: #FFC107;
  --color-orange-500: #FF9800;
  --color-purple-500: #9C27B0;

  /* ---- Semantic Tokens ---- */
  --color-primary: var(--color-blue-500);
  --color-primary-hover: var(--color-blue-600);
  --color-primary-active: var(--color-blue-700);
  --color-primary-disabled: var(--color-blue-100);
  --color-secondary: var(--color-purple-500);
  --color-bg-page: var(--color-gray-100);
  --color-bg-card: #FFFFFF;
  --color-bg-elevated: #FFFFFF;
  --color-text-primary: var(--color-gray-900);
  --color-text-secondary: var(--color-gray-600);
  --color-text-tertiary: var(--color-gray-400);
  --color-text-disabled: var(--color-gray-300);
  --color-border: var(--color-gray-200);
  --color-success: var(--color-green-500);
  --color-warning: var(--color-yellow-500);
  --color-error: var(--color-red-500);
  --color-info: var(--color-blue-500);

  --font-size-xs: 11px;
  --font-size-sm: 13px;
  --font-size-base: 15px;
  --font-size-lg: 17px;
  --font-size-xl: 20px;
  --font-size-2xl: 24px;
  --font-size-3xl: 32px;
  --font-weight-regular: 400;
  --font-weight-medium: 500;
  --font-weight-semibold: 600;
  --font-weight-bold: 700;
  --line-height-tight: 1.25;
  --line-height-normal: 1.5;
  --line-height-relaxed: 1.75;

  --spacing-1: 4px;
  --spacing-2: 8px;
  --spacing-3: 12px;
  --spacing-4: 16px;
  --spacing-5: 20px;
  --spacing-6: 24px;
  --spacing-8: 32px;
  --spacing-10: 40px;
  --spacing-12: 48px;

  --radius-sm: 4px;
  --radius-md: 8px;
  --radius-lg: 12px;
  --radius-xl: 16px;
  --radius-full: 9999px;

  --shadow-sm: 0 1px 2px rgba(0,0,0,0.05);
  --shadow-md: 0 4px 6px rgba(0,0,0,0.1);
  --shadow-lg: 0 10px 15px rgba(0,0,0,0.1);
  --shadow-xl: 0 20px 25px rgba(0,0,0,0.15);

  /* ---- Component Tokens ---- */
  --button-primary-bg: var(--color-primary);
  --button-primary-text: #FFFFFF;
  --button-primary-radius: var(--radius-md);
  --button-primary-height: 44px;
  --button-primary-padding: 12px 24px;
  --button-primary-font-size: var(--font-size-base);
  --button-primary-font-weight: var(--font-weight-medium);

  --input-bg: var(--color-bg-card);
  --input-text: var(--color-text-primary);
  --input-placeholder: var(--color-text-tertiary);
  --input-border: 1px solid var(--color-border);
  --input-border-focus: 2px solid var(--color-primary);
  --input-radius: var(--radius-md);
  --input-height: 44px;
  --input-padding: 12px 16px;

  --card-bg: var(--color-bg-card);
  --card-text: var(--color-text-primary);
  --card-radius: var(--radius-lg);
  --card-padding: var(--spacing-4);
  --card-shadow: var(--shadow-sm);
}
```

### SCSS变量格式

```scss
// ============================================
// Design Tokens - SCSS Variables
// Version: 1.0.0
// Generated: 2026-07-20
// ============================================

// ---- Primitive Tokens ----
// Colors
$color-blue-50: #E3F2FD;
$color-blue-100: #BBDEFB;
$color-blue-200: #90CAF9;
$color-blue-300: #64B5F6;
$color-blue-400: #42A5F5;
$color-blue-500: #2196F3;
$color-blue-600: #1E88E5;
$color-blue-700: #1565C0;
$color-blue-800: #0D47A1;
$color-blue-900: #0A2472;

$color-gray-50: #FAFAFA;
$color-gray-100: #F5F5F5;
$color-gray-200: #EEEEEE;
$color-gray-300: #E0E0E0;
$color-gray-400: #BDBDBD;
$color-gray-500: #9E9E9E;
$color-gray-600: #757575;
$color-gray-700: #616161;
$color-gray-800: #424242;
$color-gray-900: #212121;

$color-green-500: #4CAF50;
$color-red-500: #F44336;
$color-yellow-500: #FFC107;
$color-orange-500: #FF9800;
$color-purple-500: #9C27B0;

// ---- Semantic Tokens ----
$color-primary: $color-blue-500;
$color-primary-hover: $color-blue-600;
$color-primary-active: $color-blue-700;
$color-primary-disabled: $color-blue-100;
$color-secondary: $color-purple-500;
$color-bg-page: $color-gray-100;
$color-bg-card: #FFFFFF;
$color-bg-elevated: #FFFFFF;
$color-text-primary: $color-gray-900;
$color-text-secondary: $color-gray-600;
$color-text-tertiary: $color-gray-400;
$color-text-disabled: $color-gray-300;
$color-border: $color-gray-200;
$color-success: $color-green-500;
$color-warning: $color-yellow-500;
$color-error: $color-red-500;
$color-info: $color-blue-500;

// Typography
$font-size-xs: 11px;
$font-size-sm: 13px;
$font-size-base: 15px;
$font-size-lg: 17px;
$font-size-xl: 20px;
$font-size-2xl: 24px;
$font-size-3xl: 32px;
$font-weight-regular: 400;
$font-weight-medium: 500;
$font-weight-semibold: 600;
$font-weight-bold: 700;
$line-height-tight: 1.25;
$line-height-normal: 1.5;
$line-height-relaxed: 1.75;

// Spacing
$spacing-1: 4px;
$spacing-2: 8px;
$spacing-3: 12px;
$spacing-4: 16px;
$spacing-5: 20px;
$spacing-6: 24px;
$spacing-8: 32px;
$spacing-10: 40px;
$spacing-12: 48px;

// Border Radius
$radius-sm: 4px;
$radius-md: 8px;
$radius-lg: 12px;
$radius-xl: 16px;
$radius-full: 9999px;

// Shadows
$shadow-sm: 0 1px 2px rgba(0,0,0,0.05);
$shadow-md: 0 4px 6px rgba(0,0,0,0.1);
$shadow-lg: 0 10px 15px rgba(0,0,0,0.1);
$shadow-xl: 0 20px 25px rgba(0,0,0,0.15);

// ---- Component Tokens ----
$button-primary-bg: $color-primary;
$button-primary-text: #FFFFFF;
$button-primary-radius: $radius-md;
$button-primary-height: 44px;
$button-primary-padding: 12px 24px;
$button-primary-font-size: $font-size-base;
$button-primary-font-weight: $font-weight-medium;

$input-bg: $color-bg-card;
$input-text: $color-text-primary;
$input-placeholder: $color-text-tertiary;
$input-border: 1px solid $color-border;
$input-border-focus: 2px solid $color-primary;
$input-radius: $radius-md;
$input-height: 44px;
$input-padding: 12px 16px;

$card-bg: $color-bg-card;
$card-text: $color-text-primary;
$card-radius: $radius-lg;
$card-padding: $spacing-4;
$card-shadow: $shadow-sm;

// ---- SCSS Mixins ----
@mixin token-override($theme: "light") {
  @if $theme == "dark" {
    --color-bg-page: #1C1C1E;
    --color-bg-card: #2C2C2E;
    --color-bg-elevated: #3A3A3C;
    --color-text-primary: #FFFFFF;
    --color-text-secondary: #8E8E93;
    --color-text-tertiary: #636366;
    --color-text-disabled: #48484A;
    --color-border: #3A3A3C;
    --color-border-strong: #48484A;
  }
}
```

### JSON格式

```json
{
  "$schema": "https://design-tokens.github.io/community-group/format/",
  "metadata": {
    "version": "1.0.0",
    "generated": "2026-07-20",
    "author": "aitool.plus"
  },
  "primitive": {
    "color": {
      "blue": {
        "50":  { "$value": "#E3F2FD", "$type": "color" },
        "100": { "$value": "#BBDEFB", "$type": "color" },
        "200": { "$value": "#90CAF9", "$type": "color" },
        "300": { "$value": "#64B5F6", "$type": "color" },
        "400": { "$value": "#42A5F5", "$type": "color" },
        "500": { "$value": "#2196F3", "$type": "color" },
        "600": { "$value": "#1E88E5", "$type": "color" },
        "700": { "$value": "#1565C0", "$type": "color" },
        "800": { "$value": "#0D47A1", "$type": "color" },
        "900": { "$value": "#0A2472", "$type": "color" }
      },
      "gray": {
        "50":  { "$value": "#FAFAFA", "$type": "color" },
        "100": { "$value": "#F5F5F5", "$type": "color" },
        "200": { "$value": "#EEEEEE", "$type": "color" },
        "300": { "$value": "#E0E0E0", "$type": "color" },
        "400": { "$value": "#BDBDBD", "$type": "color" },
        "500": { "$value": "#9E9E9E", "$type": "color" },
        "600": { "$value": "#757575", "$type": "color" },
        "700": { "$value": "#616161", "$type": "color" },
        "800": { "$value": "#424242", "$type": "color" },
        "900": { "$value": "#212121", "$type": "color" }
      },
      "green": { "500": { "$value": "#4CAF50", "$type": "color" } },
      "red":   { "500": { "$value": "#F44336", "$type": "color" } },
      "yellow":{ "500": { "$value": "#FFC107", "$type": "color" } },
      "orange":{ "500": { "$value": "#FF9800", "$type": "color" } },
      "purple":{ "500": { "$value": "#9C27B0", "$type": "color" } }
    },
    "font": {
      "size": {
        "xs":   { "$value": "11px", "$type": "dimension" },
        "sm":   { "$value": "13px", "$type": "dimension" },
        "base": { "$value": "15px", "$type": "dimension" },
        "lg":   { "$value": "17px", "$type": "dimension" },
        "xl":   { "$value": "20px", "$type": "dimension" },
        "2xl":  { "$value": "24px", "$type": "dimension" },
        "3xl":  { "$value": "32px", "$type": "dimension" }
      },
      "weight": {
        "regular":  { "$value": 400, "$type": "number" },
        "medium":   { "$value": 500, "$type": "number" },
        "semibold": { "$value": 600, "$type": "number" },
        "bold":     { "$value": 700, "$type": "number" }
      }
    },
    "spacing": {
      "1":  { "$value": "4px",  "$type": "dimension" },
      "2":  { "$value": "8px",  "$type": "dimension" },
      "3":  { "$value": "12px", "$type": "dimension" },
      "4":  { "$value": "16px", "$type": "dimension" },
      "5":  { "$value": "20px", "$type": "dimension" },
      "6":  { "$value": "24px", "$type": "dimension" },
      "8":  { "$value": "32px", "$type": "dimension" },
      "10": { "$value": "40px", "$type": "dimension" },
      "12": { "$value": "48px", "$type": "dimension" }
    },
    "radius": {
      "sm":   { "$value": "4px",    "$type": "dimension" },
      "md":   { "$value": "8px",    "$type": "dimension" },
      "lg":   { "$value": "12px",   "$type": "dimension" },
      "xl":   { "$value": "16px",   "$type": "dimension" },
      "full": { "$value": "9999px", "$type": "dimension" }
    }
  },
  "semantic": {
    "color": {
      "primary":          { "$value": "{primitive.color.blue.500}", "$type": "color" },
      "primary-hover":    { "$value": "{primitive.color.blue.600}", "$type": "color" },
      "primary-active":   { "$value": "{primitive.color.blue.700}", "$type": "color" },
      "primary-disabled": { "$value": "{primitive.color.blue.100}", "$type": "color" },
      "secondary":        { "$value": "{primitive.color.purple.500}", "$type": "color" },
      "bg-page":          { "$value": "{primitive.color.gray.100}", "$type": "color" },
      "bg-card":          { "$value": "#FFFFFF", "$type": "color" },
      "bg-elevated":      { "$value": "#FFFFFF", "$type": "color" },
      "text-primary":     { "$value": "{primitive.color.gray.900}", "$type": "color" },
      "text-secondary":   { "$value": "{primitive.color.gray.600}", "$type": "color" },
      "text-tertiary":    { "$value": "{primitive.color.gray.400}", "$type": "color" },
      "text-disabled":    { "$value": "{primitive.color.gray.300}", "$type": "color" },
      "border":           { "$value": "{primitive.color.gray.200}", "$type": "color" },
      "success":          { "$value": "{primitive.color.green.500}", "$type": "color" },
      "warning":          { "$value": "{primitive.color.yellow.500}", "$type": "color" },
      "error":            { "$value": "{primitive.color.red.500}", "$type": "color" },
      "info":             { "$value": "{primitive.color.blue.500}", "$type": "color" }
    }
  },
  "component": {
    "button": {
      "primary": {
        "bg":         { "$value": "{semantic.color.primary}", "$type": "color" },
        "text":       { "$value": "#FFFFFF", "$type": "color" },
        "radius":     { "$value": "{primitive.radius.md}", "$type": "dimension" },
        "height":     { "$value": "44px", "$type": "dimension" },
        "padding-h":  { "$value": "24px", "$type": "dimension" },
        "padding-v":  { "$value": "12px", "$type": "dimension" },
        "font-size":  { "$value": "{primitive.font.size.base}", "$type": "dimension" },
        "font-weight":{ "$value": 500, "$type": "number" }
      }
    },
    "input": {
      "bg":            { "$value": "{semantic.color.bg-card}", "$type": "color" },
      "text":          { "$value": "{semantic.color.text-primary}", "$type": "color" },
      "placeholder":   { "$value": "{semantic.color.text-tertiary}", "$type": "color" },
      "border":        { "$value": "{semantic.color.border}", "$type": "color" },
      "border-focus":  { "$value": "{semantic.color.primary}", "$type": "color" },
      "radius":        { "$value": "{primitive.radius.md}", "$type": "dimension" },
      "height":        { "$value": "44px", "$type": "dimension" },
      "padding-h":     { "$value": "16px", "$type": "dimension" },
      "padding-v":     { "$value": "12px", "$type": "dimension" }
    },
    "card": {
      "bg":       { "$value": "{semantic.color.bg-card}", "$type": "color" },
      "text":     { "$value": "{semantic.color.text-primary}", "$type": "color" },
      "radius":   { "$value": "{primitive.radius.lg}", "$type": "dimension" },
      "padding":  { "$value": "{primitive.spacing.4}", "$type": "dimension" },
      "shadow":   { "$value": "{primitive.shadow.sm}", "$type": "shadow" }
    }
  }
}
```

### Tailwind配置格式

```javascript
// tailwind.config.js
// Design Tokens for Tailwind CSS
// Version: 1.0.0
// Generated: 2026-07-20
// @author aitool.plus

/** @type {import('tailwindcss').Config} */
module.exports = {
  theme: {
    colors: {
      // Primitive Colors
      blue: {
        50: '#E3F2FD',
        100: '#BBDEFB',
        200: '#90CAF9',
        300: '#64B5F6',
        400: '#42A5F5',
        500: '#2196F3',
        600: '#1E88E5',
        700: '#1565C0',
        800: '#0D47A1',
        900: '#0A2472',
      },
      gray: {
        50: '#FAFAFA',
        100: '#F5F5F5',
        200: '#EEEEEE',
        300: '#E0E0E0',
        400: '#BDBDBD',
        500: '#9E9E9E',
        600: '#757575',
        700: '#616161',
        800: '#424242',
        900: '#212121',
      },
      green: { 500: '#4CAF50' },
      red:   { 500: '#F44336' },
      yellow:{ 500: '#FFC107' },
      orange:{ 500: '#FF9800' },
      purple:{ 500: '#9C27B0' },

      // Semantic Colors
      primary: {
        DEFAULT: 'var(--color-primary)',
        hover: 'var(--color-primary-hover)',
        active: 'var(--color-primary-active)',
        disabled: 'var(--color-primary-disabled)',
      },
      secondary: 'var(--color-secondary)',
      success: 'var(--color-success)',
      warning: 'var(--color-warning)',
      error: 'var(--color-error)',
      info: 'var(--color-info)',
      surface: {
        page: 'var(--color-bg-page)',
        card: 'var(--color-bg-card)',
        elevated: 'var(--color-bg-elevated)',
      },
    },
    fontSize: {
      xs:   ['11px', { lineHeight: '1.4' }],
      sm:   ['13px', { lineHeight: '1.5' }],
      base: ['15px', { lineHeight: '1.5' }],
      lg:   ['17px', { lineHeight: '1.4' }],
      xl:   ['20px', { lineHeight: '1.3' }],
      '2xl': ['24px', { lineHeight: '1.25' }],
      '3xl': ['32px', { lineHeight: '1.2' }],
      '4xl': ['40px', { lineHeight: '1.15' }],
      '5xl': ['48px', { lineHeight: '1.1' }],
    },
    spacing: {
      1: '4px',
      2: '8px',
      3: '12px',
      4: '16px',
      5: '20px',
      6: '24px',
      8: '32px',
      10: '40px',
      12: '48px',
      16: '64px',
      20: '80px',
      24: '96px',
    },
    borderRadius: {
      sm: '4px',
      md: '8px',
      lg: '12px',
      xl: '16px',
      full: '9999px',
    },
    boxShadow: {
      sm: '0 1px 2px rgba(0,0,0,0.05)',
      md: '0 4px 6px rgba(0,0,0,0.1)',
      lg: '0 10px 15px rgba(0,0,0,0.1)',
      xl: '0 20px 25px rgba(0,0,0,0.15)',
    },
    extend: {
      textColor: {
        primary: 'var(--color-text-primary)',
        secondary: 'var(--color-text-secondary)',
        tertiary: 'var(--color-text-tertiary)',
        disabled: 'var(--color-text-disabled)',
        inverse: 'var(--color-text-inverse)',
      },
      borderColor: {
        primary: 'var(--color-border)',
        strong: 'var(--color-border-strong)',
        focus: 'var(--color-border-focus)',
      },
    },
  },
  // Dark mode support
  darkMode: ['class', '[data-theme="dark"]'],
};
```

---

## 主题切换Token覆盖机制

### 覆盖策略概述

主题切换采用CSS变量覆盖机制，不修改Primitive Token，仅覆盖Semantic Token和Component Token的值。切换通过 `data-theme` 属性实现，支持三种模式：

1. **浅色模式**（light）：默认值，无需额外覆盖
2. **深色模式**（dark）：通过 `[data-theme="dark"]` 选择器覆盖
3. **系统跟随**（system）：通过 `@media (prefers-color-scheme: dark)` 自动适配

### 浅色->深色切换时变化的Token清单

#### 颜色Token变化

| 语义Token | 浅色值 | 深色值 | 变化类型 |
|-----------|--------|--------|----------|
| --color-primary | #007AFF | #0A84FF | 色值调整(提亮) |
| --color-primary-hover | #0051D5 | #409CFF | 色值调整(提亮) |
| --color-primary-active | #0047B8 | #5EB0FF | 色值调整(提亮) |
| --color-primary-disabled | #B3D7FF | #3A5070 | 色值调整(暗化) |
| --color-secondary | #5856D6 | #5E5CE6 | 色值微调 |
| --color-bg-page | #F2F2F7 | #1C1C1E | 反转 |
| --color-bg-card | #FFFFFF | #2C2C2E | 反转 |
| --color-bg-elevated | #FFFFFF | #3A3A3C | 反转 |
| --color-bg-inverse | #212121 | #F5F5F5 | 反转 |
| --color-text-primary | #000000 | #FFFFFF | 反转 |
| --color-text-secondary | #8E8E93 | #8E8E93 | 不变 |
| --color-text-tertiary | #C7C7CC | #636366 | 反转 |
| --color-text-disabled | #C7C7CC | #48484A | 暗化 |
| --color-text-inverse | #FFFFFF | #000000 | 反转 |
| --color-border | #E5E5EA | #3A3A3C | 反转 |
| --color-border-strong | #C7C7CC | #48484A | 反转 |
| --color-success | #34C759 | #30D158 | 提亮 |
| --color-warning | #FFCC00 | #FFD60A | 提亮 |
| --color-error | #FF3B30 | #FF453A | 提亮 |
| --color-info | #007AFF | #0A84FF | 提亮 |
| --color-success-bg | #E8F5E9 | #1B3A1B | 反转 |
| --color-warning-bg | #FFF8E1 | #3D3520 | 反转 |
| --color-error-bg | #FFEBEE | #3D2020 | 反转 |
| --color-info-bg | #E3F2FD | #1A2A3D | 反转 |

#### 阴影Token变化

| 语义Token | 浅色值 | 深色值 | 变化类型 |
|-----------|--------|--------|----------|
| --shadow-sm | 0 1px 2px rgba(0,0,0,0.05) | 0 1px 2px rgba(0,0,0,0.2) | 透明度增加 |
| --shadow-md | 0 4px 6px rgba(0,0,0,0.1) | 0 4px 6px rgba(0,0,0,0.3) | 透明度增加 |
| --shadow-lg | 0 10px 15px rgba(0,0,0,0.1) | 0 10px 15px rgba(0,0,0,0.4) | 透明度增加 |
| --shadow-xl | 0 20px 25px rgba(0,0,0,0.15) | 0 20px 25px rgba(0,0,0,0.5) | 透明度增加 |

#### 不变化的Token

以下Token在深色模式下保持不变：
- 所有Primitive Token（原始色值、原始字号、原始间距等）
- 所有间距Token（spacing系列）
- 所有圆角Token（radius系列）
- 所有字号Token（font-size系列）
- 所有字重Token（font-weight系列）
- 所有行高Token（line-height系列）

### data-theme属性覆盖实现

```css
/* ============================================
   主题切换 - data-theme 属性覆盖
   ============================================ */

/* 浅色模式（默认） */
:root,
[data-theme="light"] {
  --color-primary: #007AFF;
  --color-primary-hover: #0051D5;
  --color-primary-active: #0047B8;
  --color-primary-disabled: #B3D7FF;
  --color-secondary: #5856D6;
  --color-bg-page: #F2F2F7;
  --color-bg-card: #FFFFFF;
  --color-bg-elevated: #FFFFFF;
  --color-bg-inverse: #212121;
  --color-text-primary: #000000;
  --color-text-secondary: #8E8E93;
  --color-text-tertiary: #C7C7CC;
  --color-text-disabled: #C7C7CC;
  --color-text-inverse: #FFFFFF;
  --color-border: #E5E5EA;
  --color-border-strong: #C7C7CC;
  --color-success: #34C759;
  --color-warning: #FFCC00;
  --color-error: #FF3B30;
  --color-info: #007AFF;
  --color-success-bg: #E8F5E9;
  --color-warning-bg: #FFF8E1;
  --color-error-bg: #FFEBEE;
  --color-info-bg: #E3F2FD;
  --shadow-sm: 0 1px 2px rgba(0,0,0,0.05);
  --shadow-md: 0 4px 6px rgba(0,0,0,0.1);
  --shadow-lg: 0 10px 15px rgba(0,0,0,0.1);
  --shadow-xl: 0 20px 25px rgba(0,0,0,0.15);
}

/* 深色模式 */
[data-theme="dark"] {
  --color-primary: #0A84FF;
  --color-primary-hover: #409CFF;
  --color-primary-active: #5EB0FF;
  --color-primary-disabled: #3A5070;
  --color-secondary: #5E5CE6;
  --color-bg-page: #1C1C1E;
  --color-bg-card: #2C2C2E;
  --color-bg-elevated: #3A3A3C;
  --color-bg-inverse: #F5F5F5;
  --color-text-primary: #FFFFFF;
  --color-text-secondary: #8E8E93;
  --color-text-tertiary: #636366;
  --color-text-disabled: #48484A;
  --color-text-inverse: #000000;
  --color-border: #3A3A3C;
  --color-border-strong: #48484A;
  --color-success: #30D158;
  --color-warning: #FFD60A;
  --color-error: #FF453A;
  --color-info: #0A84FF;
  --color-success-bg: #1B3A1B;
  --color-warning-bg: #3D3520;
  --color-error-bg: #3D2020;
  --color-info-bg: #1A2A3D;
  --shadow-sm: 0 1px 2px rgba(0,0,0,0.2);
  --shadow-md: 0 4px 6px rgba(0,0,0,0.3);
  --shadow-lg: 0 10px 15px rgba(0,0,0,0.4);
  --shadow-xl: 0 20px 25px rgba(0,0,0,0.5);
}

/* 系统跟随 */
@media (prefers-color-scheme: dark) {
  :root:not([data-theme="light"]) {
    --color-primary: #0A84FF;
    --color-primary-hover: #409CFF;
    --color-primary-active: #5EB0FF;
    --color-primary-disabled: #3A5070;
    --color-secondary: #5E5CE6;
    --color-bg-page: #1C1C1E;
    --color-bg-card: #2C2C2E;
    --color-bg-elevated: #3A3A3C;
    --color-bg-inverse: #F5F5F5;
    --color-text-primary: #FFFFFF;
    --color-text-secondary: #8E8E93;
    --color-text-tertiary: #636366;
    --color-text-disabled: #48484A;
    --color-text-inverse: #000000;
    --color-border: #3A3A3C;
    --color-border-strong: #48484A;
    --color-success: #30D158;
    --color-warning: #FFD60A;
    --color-error: #FF453A;
    --color-info: #0A84FF;
    --color-success-bg: #1B3A1B;
    --color-warning-bg: #3D3520;
    --color-error-bg: #3D2020;
    --color-info-bg: #1A2A3D;
    --shadow-sm: 0 1px 2px rgba(0,0,0,0.2);
    --shadow-md: 0 4px 6px rgba(0,0,0,0.3);
    --shadow-lg: 0 10px 15px rgba(0,0,0,0.4);
    --shadow-xl: 0 20px 25px rgba(0,0,0,0.5);
  }
}
```

### JavaScript主题切换实现

```javascript
/**
 * 主题切换控制器
 * @author aitool.plus
 */
const ThemeManager = {
  STORAGE_KEY: 'app-theme',

  init() {
    const saved = localStorage.getItem(this.STORAGE_KEY);
    if (saved) {
      this.setTheme(saved);
    } else {
      const prefersDark = window.matchMedia('(prefers-color-scheme: dark)');
      this.setTheme(prefersDark.matches ? 'dark' : 'light');
      prefersDark.addEventListener('change', (e) => {
        if (!localStorage.getItem(this.STORAGE_KEY)) {
          this.setTheme(e.matches ? 'dark' : 'light');
        }
      });
    }
  },

  setTheme(theme) {
    document.documentElement.setAttribute('data-theme', theme);
    localStorage.setItem(this.STORAGE_KEY, theme);
  },

  toggle() {
    const current = document.documentElement.getAttribute('data-theme');
    this.setTheme(current === 'dark' ? 'light' : 'dark');
  },

  getTheme() {
    return document.documentElement.getAttribute('data-theme') || 'light';
  }
};
```

### 各平台深色模式Token覆盖对照

| 语义Token | iOS深色 | Android深色 | HarmonyOS深色 | Windows深色 | WeUI深色 |
|-----------|---------|-------------|---------------|-------------|----------|
| --color-primary | #0A84FF | #D0BCFF | #3399FF | #4CC2FF | #2FD66D |
| --color-bg-page | #1C1C1E | #121212 | #121212 | #201F1E | #121212 |
| --color-bg-card | #2C2C2E | #1E1E1E | #1E1E1E | #292827 | #1E1E1E |
| --color-bg-elevated | #3A3A3C | #2C2C2C | #2C2C2C | #323130 | #2C2C2C |
| --color-text-primary | #FFFFFF | #FFFFFF | #FFFFFF | #FFFFFF | #FFFFFF |
| --color-text-secondary | #8E8E93 | #A0A0A0 | #A0A0A0 | #A19F9D | #A0A0A0 |
| --color-text-tertiary | #636366 | #666666 | #666666 | #605E5C | #666666 |
| --color-border | #3A3A3C | #333333 | #333333 | #3B3A39 | #333333 |
| --color-success | #30D158 | #69F0AE | #69F0AE | #6CCB5F | #2FD66D |
| --color-warning | #FFD60A | #FFD740 | #FFD740 | #FFD740 | #FFD740 |
| --color-error | #FF453A | #CF6679 | #FF4D6D | #FF8C8C | #FF5252 |
