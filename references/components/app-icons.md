---
name: app-icons
title: 拟真原生应用图标库
description: 9 个真实感原生系统应用图标的 SVG 规范（相机/照片/地图/天气/联系人/时钟/备忘录/计算器/设置），用于 Demo 功能网格，禁止字母或 emoji 占位。
---

# 拟真原生应用图标库

> 本文件为 ui-design-aitool-plus 的图标资产。所有图标为单文件内联 SVG，透明背景，
> 真实渐变背景由容器 `grid-icon` 提供，圆角随平台规范（iOS 12px squircle / Android 16-20dp /
> Windows 4px / 小程序 8px）。禁止用字母、emoji 或纯色块占位。

## 图标清单（顺序即 Demo 功能网格顺序）

### 1. 相机

- **真实渐变背景**：`linear-gradient(135deg,#54545A,#2C2C2E)`
- **字形 SVG（透明背景，viewBox 0 0 48 48）**：

```html
<svg viewBox="0 0 48 48" style="width:100%;height:100%;display:block" xmlns="http://www.w3.org/2000/svg"><rect x="9" y="16" width="30" height="20" rx="5" fill="#ffffff"/><rect x="19" y="12" width="10" height="5" rx="2.5" fill="#ffffff"/><circle cx="24" cy="26" r="7.5" fill="#2C2C2E"/><circle cx="24" cy="26" r="5" fill="#3AA0E0"/><circle cx="24" cy="26" r="2.4" fill="#1C1C1E" opacity="0.55"/><circle cx="14" cy="21" r="1.7" fill="#FFCC00"/></svg>
```

### 2. 照片

- **真实渐变背景**：`linear-gradient(135deg,#FFFFFF,#F2F2F7)`
- **字形 SVG（透明背景，viewBox 0 0 48 48）**：

```html
<svg viewBox="0 0 48 48" style="width:100%;height:100%;display:block" xmlns="http://www.w3.org/2000/svg"><g><ellipse cx="24" cy="13" rx="4.2" ry="8" fill="#FF3B30" transform="rotate(0 24 24)"/><ellipse cx="24" cy="13" rx="4.2" ry="8" fill="#FF9500" transform="rotate(45 24 24)"/><ellipse cx="24" cy="13" rx="4.2" ry="8" fill="#FFCC00" transform="rotate(90 24 24)"/><ellipse cx="24" cy="13" rx="4.2" ry="8" fill="#34C759" transform="rotate(135 24 24)"/><ellipse cx="24" cy="13" rx="4.2" ry="8" fill="#30D158" transform="rotate(180 24 24)"/><ellipse cx="24" cy="13" rx="4.2" ry="8" fill="#00C7BE" transform="rotate(225 24 24)"/><ellipse cx="24" cy="13" rx="4.2" ry="8" fill="#007AFF" transform="rotate(270 24 24)"/><ellipse cx="24" cy="13" rx="4.2" ry="8" fill="#5856D6" transform="rotate(315 24 24)"/></g><circle cx="24" cy="24" r="5" fill="#ECECF0"/></svg>
```

### 3. 地图

- **真实渐变背景**：`linear-gradient(135deg,#34AADC,#007AFF)`
- **字形 SVG（透明背景，viewBox 0 0 48 48）**：

```html
<svg viewBox="0 0 48 48" style="width:100%;height:100%;display:block" xmlns="http://www.w3.org/2000/svg"><path d="M9 14 L20 11 L29 14 L39 11 L39 36 L29 39 L20 36 L9 39 Z" fill="#ffffff" opacity="0.95"/><path d="M20 11 L20 36 M29 14 L29 39" stroke="#C7C7CC" stroke-width="1.2"/><path d="M9 14 L39 11 M9 39 L39 36" stroke="#C7C7CC" stroke-width="1.2"/><path d="M30 27 c-3.2 0 -5.5 2.3 -5.5 5.4 c0 4 5.5 9.6 5.5 9.6 c0 0 5.5 -5.6 5.5 -9.6 c0 -3.1 -2.3 -5.4 -5.5 -5.4 z" fill="#FF3B30"/><circle cx="30" cy="32" r="2.1" fill="#ffffff"/></svg>
```

### 4. 天气

- **真实渐变背景**：`linear-gradient(135deg,#4BA3E8,#1A6FC4)`
- **字形 SVG（透明背景，viewBox 0 0 48 48）**：

```html
<svg viewBox="0 0 48 48" style="width:100%;height:100%;display:block" xmlns="http://www.w3.org/2000/svg"><circle cx="33" cy="17" r="6" fill="#FFD60A"/><g stroke="#FFD60A" stroke-width="2" stroke-linecap="round"><line x1="33" y1="6" x2="33" y2="9"/><line x1="33" y1="25" x2="33" y2="28"/><line x1="22" y1="17" x2="25" y2="17"/><line x1="41" y1="17" x2="44" y2="17"/><line x1="25" y1="9" x2="27" y2="11"/><line x1="39" y1="23" x2="41" y2="25"/><line x1="25" y1="25" x2="27" y2="23"/><line x1="39" y1="11" x2="41" y2="9"/></g><g fill="#ffffff"><circle cx="18" cy="30" r="6"/><circle cx="26" cy="27" r="7.5"/><circle cx="32" cy="31" r="5.5"/><rect x="16" y="30" width="18" height="7" rx="3.5"/></g></svg>
```

### 5. 联系人

- **真实渐变背景**：`linear-gradient(135deg,#5E5CE6,#3A3A9E)`
- **字形 SVG（透明背景，viewBox 0 0 48 48）**：

```html
<svg viewBox="0 0 48 48" style="width:100%;height:100%;display:block" xmlns="http://www.w3.org/2000/svg"><circle cx="24" cy="19" r="7" fill="#ffffff"/><path d="M11 40 c0 -8.5 26 -8.5 26 0 z" fill="#ffffff"/></svg>
```

### 6. 时钟

- **真实渐变背景**：`linear-gradient(135deg,#1C1C1E,#000000)`
- **字形 SVG（透明背景，viewBox 0 0 48 48）**：

```html
<svg viewBox="0 0 48 48" style="width:100%;height:100%;display:block" xmlns="http://www.w3.org/2000/svg"><circle cx="24" cy="24" r="17" fill="none" stroke="#8E8E93" stroke-width="2"/><g stroke="#C7C7CC" stroke-width="1.6" stroke-linecap="round"><line x1="24" y1="9" x2="24" y2="12"/><line x1="24" y1="36" x2="24" y2="39"/><line x1="9" y1="24" x2="12" y2="24"/><line x1="36" y1="24" x2="39" y2="24"/></g><line x1="24" y1="24" x2="24" y2="14" stroke="#ffffff" stroke-width="2.6" stroke-linecap="round"/><line x1="24" y1="24" x2="33" y2="24" stroke="#ffffff" stroke-width="2.6" stroke-linecap="round"/><line x1="24" y1="24" x2="24" y2="33" stroke="#FF3B30" stroke-width="1.6" stroke-linecap="round"/><circle cx="24" cy="24" r="1.8" fill="#ffffff"/></svg>
```

### 7. 备忘录

- **真实渐变背景**：`linear-gradient(135deg,#FFE07A,#FFCC00)`
- **字形 SVG（透明背景，viewBox 0 0 48 48）**：

```html
<svg viewBox="0 0 48 48" style="width:100%;height:100%;display:block" xmlns="http://www.w3.org/2000/svg"><rect x="11" y="8" width="26" height="32" rx="3" fill="#ffffff"/><rect x="11" y="8" width="26" height="7" rx="3" fill="#FF9500"/><g stroke="#D9D9DE" stroke-width="1.4"><line x1="15" y1="20" x2="33" y2="20"/><line x1="15" y1="25" x2="33" y2="25"/><line x1="15" y1="30" x2="33" y2="30"/><line x1="15" y1="35" x2="28" y2="35"/></g><line x1="18" y1="8" x2="18" y2="40" stroke="#FF3B30" stroke-width="1.2" opacity="0.6"/></svg>
```

### 8. 计算器

- **真实渐变背景**：`linear-gradient(135deg,#3A3A3C,#1C1C1E)`
- **字形 SVG（透明背景，viewBox 0 0 48 48）**：

```html
<svg viewBox="0 0 48 48" style="width:100%;height:100%;display:block" xmlns="http://www.w3.org/2000/svg"><rect x="10" y="7" width="28" height="34" rx="4" fill="#48484A"/><rect x="13" y="10" width="22" height="7" rx="2" fill="#1C1C1E"/><g fill="#9A9AA0"><circle cx="16" cy="23" r="2.4"/><circle cx="24" cy="23" r="2.4"/><circle cx="32" cy="23" r="2.4"/><circle cx="16" cy="30" r="2.4"/><circle cx="24" cy="30" r="2.4"/><circle cx="32" cy="30" r="2.4"/><circle cx="16" cy="37" r="2.4"/><circle cx="24" cy="37" r="2.4"/></g><circle cx="32" cy="37" r="2.4" fill="#FF9500"/></svg>
```

### 9. 设置

- **真实渐变背景**：`linear-gradient(135deg,#B0B0B5,#8A8A8E)`
- **字形 SVG（透明背景，viewBox 0 0 48 48）**：

```html
<svg viewBox="0 0 48 48" style="width:100%;height:100%;display:block" xmlns="http://www.w3.org/2000/svg"><g fill="#ffffff"><circle cx="24" cy="24" r="8.5"/><rect x="22.2" y="10" width="3.6" height="5.5" rx="1" transform="rotate(0 24 24)"/><rect x="22.2" y="10" width="3.6" height="5.5" rx="1" transform="rotate(45 24 24)"/><rect x="22.2" y="10" width="3.6" height="5.5" rx="1" transform="rotate(90 24 24)"/><rect x="22.2" y="10" width="3.6" height="5.5" rx="1" transform="rotate(135 24 24)"/><rect x="22.2" y="10" width="3.6" height="5.5" rx="1" transform="rotate(180 24 24)"/><rect x="22.2" y="10" width="3.6" height="5.5" rx="1" transform="rotate(225 24 24)"/><rect x="22.2" y="10" width="3.6" height="5.5" rx="1" transform="rotate(270 24 24)"/><rect x="22.2" y="10" width="3.6" height="5.5" rx="1" transform="rotate(315 24 24)"/></g><circle cx="24" cy="24" r="3.6" fill="#8A8A8E"/></svg>
```

## 使用方式

在 Demo 的 `grid-section > grid-container` 中，按上方顺序渲染 9 个 `grid-item`，
每个 `grid-icon` 设置对应渐变背景，内部直接放入上述 SVG（宽度高度 100%）。
需为 `.grid-icon` 添加 `overflow:hidden` 以保证 SVG 在圆角容器内被正确裁剪。
