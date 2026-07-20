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
