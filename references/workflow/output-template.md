> @author aitool.plus

# 输出模板

## 1. 高保真HTML原型

### 格式说明

单文件HTML+CSS+JS，可直接在浏览器中打开预览。

### 包含内容

- 完整HTML结构（语义化标签）
- 内嵌CSS样式（含Design Token变量）
- 内嵌JavaScript交互逻辑
- 响应式断点适配
- 浅色/深色模式切换
- 模拟数据填充

### 输出规范

- 文件命名：`{page-name}-{os-style}.html`
- 单文件完整，无外部依赖
- 支持 viewport 缩放
- 移动端触摸事件模拟
- 表单交互可点击

### 示例结构

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>页面标题 - OS风格</title>
  <style>
    /* CSS变量定义 */
    :root {
      --color-primary: #007AFF;
      /* ... */
    }
    /* 样式代码 */
  </style>
</head>
<body>
  <!-- HTML结构 -->
  <script>
    // 交互逻辑
  </script>
</body>
</html>
```

---

## 2. 设计规范Markdown文档

### 格式说明

结构化的设计规范文档，包含Token表、组件规范、页面规范和使用说明。

### 包含内容

#### 2.1 Token表

- 颜色Token：主色/次色/辅助色/背景色/文字色/功能色
- 字体Token：字体族/字号/行高/字重
- 间距Token：基础单位/间距阶梯/边距规范
- 圆角Token：组件圆角值
- 阴影Token：层级阴影定义

#### 2.2 组件规范

- 按钮组件：尺寸/状态/变体
- 输入框组件：尺寸/状态/验证
- 卡片组件：尺寸/阴影/间距
- 列表组件：间距/分隔线/空状态
- 导航组件：布局/交互/响应式

#### 2.3 页面规范

- 页面结构模板
- 布局网格系统
- 内容区域划分
- 安全区域规范

#### 2.4 使用说明

- 组件引入方式
- Token覆盖方法
- 主题切换配置
- 自定义扩展指南

---

## 3. CSS/SCSS样式代码

### 格式说明

可直接使用的CSS/SCSS代码，包含完整的Design Token变量和组件样式类。

### 包含内容

#### 3.1 Design Token变量

```scss
// 颜色Token
$color-primary: var(--color-primary);
$color-secondary: var(--color-secondary);
// ...

// 字体Token
$font-family-base: var(--font-family-base);
$font-size-base: var(--font-size-base);
// ...

// 间距Token
$spacing-unit: var(--spacing-unit);
$spacing-xs: var(--spacing-xs);
// ...
```

#### 3.2 组件样式类

```scss
// 按钮组件
.btn {
  // 基础样式
  &-primary { /* ... */ }
  &-secondary { /* ... */ }
  // 尺寸变体
  &-sm { /* ... */ }
  &-lg { /* ... */ }
}
```

#### 3.3 工具类

```scss
// 间距工具类
.mt-1 { margin-top: var(--spacing-1); }
.mb-1 { margin-bottom: var(--spacing-1); }
// ...

// 文字工具类
.text-primary { color: var(--color-primary); }
.font-bold { font-weight: var(--font-weight-bold); }
// ...
```

#### 3.4 响应式断点

```scss
$breakpoints: (
  'sm': 375px,
  'md': 600px,
  'lg': 840px,
  'xl': 1280px
);
```

---

## 4. Figma标注参数

### 格式说明

可直接复制到Figma的标注格式，包含组件尺寸、间距、色值、字号、圆角等参数。

### 标注格式

#### 4.1 组件尺寸标注

```
组件名称: Button - Primary
- 宽度: 自适应（最小 88px）
- 高度: 48px
- 内边距: 12px 24px
- 圆角: 8px
```

#### 4.2 间距标注

```
间距规范:
- 组件间间距: 16px
- 内容区内边距: 20px
- 页面边距: 16px（手机）/ 24px（平板）/ 32px（桌面）
```

#### 4.3 色值标注

```
颜色规范:
- Primary: #007AFF
- Secondary: #5856D6
- Background: #F2F2F7
- Text Primary: #000000
- Text Secondary: #8E8E93
```

#### 4.4 字号标注

```
字体规范:
- 标题: 17px / Semibold / -0.02em
- 正文: 15px / Regular / -0.02em
- 辅助文字: 13px / Regular / -0.01em
- 标签: 11px / Medium / 0em
```

#### 4.5 圆角标注

```
圆角规范:
- 按钮: 8px
- 卡片: 12px
- 输入框: 8px
- 弹窗: 16px
- 圆形图标: 50%
```

### 复制到Figma的方法

1. 在Figma中选中目标图层
2. 打开右侧属性面板
3. 将对应参数粘贴到对应字段
4. 或使用Figma插件批量导入
