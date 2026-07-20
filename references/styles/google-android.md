# Google Android Material Design 3 设计规范

> @author aitool.plus

---

## 1. 设计哲学

### 1.1 三大核心原则

| 原则 | 英文 | 含义 |
|------|------|------|
| 表达力 | Expressive | 色彩大胆、动效丰富、组件富有个性与情感表达 |
| 个性化 | Personal | Material You动态取色，用户壁纸生成专属色板，设备自适应 |
| 适应性 | Adaptive | 跨设备跨尺寸自适应布局，手机/平板/折叠屏/桌面统一体验 |

### 1.2 设计准则

- 动态色彩：基于用户壁纸seed color自动生成完整色板，实现千人千面
- 组件化：原子组件组合构建复杂界面，保持一致性与可预测性
- 运动叙事：转场动画承载空间关系与逻辑关系，不仅是视觉装饰
- 无障碍：满足WCAG 2.1 AA标准，色彩对比度、触控尺寸、语义化全面覆盖

---

## 2. 色彩体系

### 2.1 Material You 动态取色机制

- 用户选择壁纸中的Seed Color，系统通过HCT色彩空间算法生成Tonal Palette
- Tonal Palette包含13个色调档位（0-1000，步长100），每个色调档位有浅色/深色两套映射
- 12个语义色彩角色从Tonal Palette中取值，确保色彩和谐统一

### 2.2 语义色彩角色（浅色模式）

| 色彩角色 | Hex值 | 用途 |
|----------|-------|------|
| Primary | #6750A4 | 主操作色、FAB、高亮态 |
| On Primary | #FFFFFF | Primary上的文字/图标 |
| Primary Container | #EADDFF | 主色容器背景 |
| On Primary Container | #21005D | Primary Container上的文字 |
| Secondary | #625B71 | 次级操作、辅助元素 |
| On Secondary | #FFFFFF | Secondary上的文字 |
| Secondary Container | #E8DEF8 | 次色容器背景 |
| On Secondary Container | #1D192B | Secondary Container上的文字 |
| Tertiary | #7D5260 | 三级色、特殊标记 |
| On Tertiary | #FFFFFF | Tertiary上的文字 |
| Tertiary Container | #FFD8E4 | 三级色容器背景 |
| On Tertiary Container | #31111D | Tertiary Container上的文字 |
| Error | #B3261E | 错误、危险操作 |
| On Error | #FFFFFF | Error上的文字 |
| Error Container | #F9DEDC | 错误容器背景 |
| On Error Container | #410E0B | Error Container上的文字 |
| Surface | #FFFBFE | 主表面背景 |
| On Surface | #1C1B1F | Surface上的主文字 |
| Surface Variant | #E7E0EC | 变体表面背景 |
| On Surface Variant | #49454F | Surface Variant上的文字 |
| Outline | #79747E | 边框、轮廓线 |
| Outline Variant | #CAC4D0 | 次级边框、分隔线 |
| Inverse Surface | #313033 | 反转表面 |
| Inverse On Surface | #F4EFF4 | Inverse Surface上的文字 |
| Surface Container Lowest | #FFFFFF | 最低层容器 |
| Surface Container Low | #F7F2FA | 低层容器 |
| Surface Container | #F3EDF7 | 标准容器 |
| Surface Container High | #ECE6F0 | 高层容器 |
| Surface Container Highest | #E6E0E9 | 最高层容器 |

### 2.3 语义色彩角色（深色模式）

| 色彩角色 | Hex值 | 用途 |
|----------|-------|------|
| Primary | #D0BCFF | 主操作色（深色模式提亮） |
| On Primary | #381E72 | Primary上的文字 |
| Primary Container | #4F378B | 主色容器背景 |
| On Primary Container | #EADDFF | Primary Container上的文字 |
| Secondary | #CCC2DC | 次级操作 |
| On Secondary | #332D41 | Secondary上的文字 |
| Secondary Container | #4A4458 | 次色容器背景 |
| On Secondary Container | #E8DEF8 | Secondary Container上的文字 |
| Tertiary | #EFB8C8 | 三级色 |
| On Tertiary | #492532 | Tertiary上的文字 |
| Tertiary Container | #633B48 | 三级色容器背景 |
| On Tertiary Container | #FFD8E4 | Tertiary Container上的文字 |
| Error | #F2B8B5 | 错误色 |
| On Error | #601410 | Error上的文字 |
| Error Container | #8C1D18 | 错误容器背景 |
| On Error Container | #F9DEDC | Error Container上的文字 |
| Surface | #1C1B1F | 主表面背景 |
| On Surface | #E6E1E5 | Surface上的主文字 |
| Surface Variant | #49454F | 变体表面背景 |
| On Surface Variant | #CAC4D0 | Surface Variant上的文字 |
| Outline | #938F99 | 边框 |
| Outline Variant | #49454F | 次级边框 |
| Inverse Surface | #E6E1E5 | 反转表面 |
| Inverse On Surface | #313033 | Inverse Surface上的文字 |
| Surface Container Lowest | #0F0D13 | 最低层容器 |
| Surface Container Low | #1D1B20 | 低层容器 |
| Surface Container | #211F26 | 标准容器 |
| Surface Container High | #2B2930 | 高层容器 |
| Surface Container Highest | #36343B | 最高层容器 |

---

## 3. 字体排版

### 3.1 字体族

| 用途 | 字体名称 | 说明 |
|------|---------|------|
| 系统界面 | Roboto Flex | 可变字体，支持宽度/重量轴调整 |
| 展示标题 | Google Sans | 品牌标题、大展示文字 |
| 等宽代码 | Roboto Mono | 代码、数字对齐 |

### 3.2 字号阶梯（MD3 Typography Scale）

| 样式名称 | 字号 (sp) | 字重 | 行高 (sp) | 字间距 (sp) | 用途 |
|----------|----------|------|----------|------------|------|
| Display Large | 57 | Regular (400) | 64 | -0.25 | 超大展示标题 |
| Display Medium | 45 | Regular (400) | 52 | 0 | 大展示标题 |
| Display Small | 36 | Regular (400) | 44 | 0 | 小展示标题 |
| Headline Large | 32 | Regular (400) | 40 | 0 | 大标题 |
| Headline Medium | 28 | Regular (400) | 36 | 0 | 中标题 |
| Headline Small | 24 | Regular (400) | 32 | 0 | 小标题 |
| Title Large | 22 | Regular (400) | 28 | 0 | 大区域标题 |
| Title Medium | 16 | Medium (500) | 24 | 0.15 | 中区域标题、卡片标题 |
| Title Small | 14 | Medium (500) | 20 | 0.1 | 小区域标题 |
| Body Large | 16 | Regular (400) | 24 | 0.5 | 大正文 |
| Body Medium | 14 | Regular (400) | 20 | 0.25 | 标准正文 |
| Body Small | 12 | Regular (400) | 16 | 0.4 | 小正文 |
| Label Large | 14 | Medium (500) | 20 | 0.1 | 按钮文字 |
| Label Medium | 12 | Medium (500) | 16 | 0.5 | 标签、小按钮 |
| Label Small | 11 | Medium (500) | 16 | 0.5 | 极小标签 |

### 3.3 字重定义

| 字重名称 | 数值 | 用途 |
|---------|------|------|
| Regular | 400 | 正文、标题 |
| Medium | 500 | 标签、按钮、小标题 |
| Bold | 700 | 强调（极少使用） |

---

## 4. 间距与布局

### 4.1 基础间距网格

| 参数 | 数值 | 说明 |
|------|------|------|
| 基础网格单位 | 4dp | 所有间距为4的倍数 |
| 次级网格单位 | 8dp | 大间距使用8的倍数 |
| 水平边距 (Margin) | 16dp | 内容区左右边距 |
| 大屏水平边距 | 24dp | 平板/桌面边距 |
| 列表项高度 | 48dp | 标准列表行最小高度 |
| 三行列表项高度 | 88dp | 含主副标题+辅助 |
| 紧凑列表项高度 | 32dp | 极简信息行 |

### 4.2 间距阶梯

| 间距名称 | 数值 (dp) | 用途 |
|----------|----------|------|
| 4dp | 4dp | 4 | 极小间距、图标与文字间距 |
| 8dp | 8 | 小间距、组件内间距 |
| 12dp | 12 | 中小间距、卡片内边距 |
| 16dp | 16 | 标准间距、页面边距 |
| 24dp | 24 | 大间距、区块间距 |
| 32dp | 32 | 超大间距、模块间距 |

### 4.3 布局断点

| 断点名称 | 宽度范围 | 布局列数 | 边距 |
|----------|---------|---------|------|
| Compact | 0-599dp | 4列 | 16dp |
| Medium | 600-839dp | 8列 | 24dp |
| Expanded | 840-1199dp | 12列 | 24dp |
| Large | 1200-1599dp | 12列 | 24dp |
| Extra Large | 1600dp+ | 12列 | 32dp |

---

## 5. 圆角体系

### 5.1 Shape系统

| Shape尺寸 | 圆角数值 (dp) | 用途 |
|-----------|-------------|------|
| Shape None | 0dp | 无圆角，全宽组件 |
| Shape Extra Small | 4dp | 极小圆角，Chip、小标签 |
| Shape Small | 8dp | 小圆角，Button、TextField |
| Shape Medium | 12dp | 中圆角，Card、Dialog |
| Shape Large | 16dp | 大圆角，FAB、BottomSheet |
| Shape Extra Large | 28dp | 超大圆角，SearchBar、Extended FAB |
| Shape Full | 50% | 完全圆形，圆形FAB、Avatar |

### 5.2 组件圆角映射

| 组件类型 | 圆角数值 (dp) | 说明 |
|----------|-------------|------|
| Filled Button | 20dp (Full) | 胶囊形按钮 |
| Outlined Button | 20dp (Full) | 胶囊形按钮 |
| Tonal Button | 20dp (Full) | 胶囊形按钮 |
| TextField | 4dp (Extra Small) | 输入框 |
| Card (Elevated) | 12dp (Medium) | 提升卡片 |
| Card (Filled) | 12dp (Medium) | 填充卡片 |
| Card (Outlined) | 12dp (Medium) | 描边卡片 |
| Dialog | 28dp (Extra Large) | 弹窗 |
| Bottom Sheet | 28dp (Extra Large) | 底部面板 |
| FAB | 16dp (Large) | 浮动操作按钮 |
| Extended FAB | 16dp (Large) | 扩展FAB |
| Chip | 8dp (Small) | 标签 |
| Navigation Bar | 0dp (None) | 底部导航 |
| Navigation Rail | 0dp (None) + Item 28dp | 侧边导航 |
| Search Bar | 28dp (Extra Large) | 搜索栏 |
| Switch | 16dp (Full) | 开关 |

---

## 6. 阴影与层级

### 6.1 Elevation层级

| 层级 | Elevation (dp) | 阴影参数 | 用途 |
|------|---------------|---------|------|
| Level 0 | 0dp | 无阴影 | 背景层、平面组件 |
| Level 1 | 1dp | 0dp 1dp 3dp rgba(0,0,0,0.12) + 0dp 1dp 2dp rgba(0,0,0,0.24) | Card (Elevated)、SearchBar |
| Level 2 | 3dp | 0dp 1dp 5dp rgba(0,0,0,0.12) + 0dp 2dp 4dp rgba(0,0,0,0.24) | FAB (Resting)、Snackbar |
| Level 3 | 6dp | 0dp 3dp 8dp rgba(0,0,0,0.12) + 0dp 4dp 6dp rgba(0,0,0,0.24) | FAB (Pressed)、Menu |
| Level 4 | 8dp | 0dp 4dp 12dp rgba(0,0,0,0.12) + 0dp 6dp 8dp rgba(0,0,0,0.24) | Dialog、Navigation Drawer |
| Level 5 | 12dp | 0dp 6dp 16dp rgba(0,0,0,0.12) + 0dp 8dp 10dp rgba(0,0,0,0.24) | Bottom Sheet (Modal) |

### 6.2 Tonal Elevation

- 深色模式下不使用阴影，改用Tonal Elevation（色调提升）
- 每提升1级Elevation，Surface色值在Tonal Palette中向浅色调偏移1-2档
- Level 0: Surface #1C1B1F
- Level 1: Surface Container Low #1D1B20
- Level 2: Surface Container #211F26
- Level 3: Surface Container High #2B2930
- Level 4: Surface Container Highest #36343B

### 6.3 状态层 (State Layer)

| 状态 | 透明度 | 叠加色 |
|------|--------|-------|
| Hover | 8% | On Surface / On Primary |
| Focus | 12% | On Surface / On Primary |
| Pressed | 12% | On Surface / On Primary |
| Dragged | 16% | On Surface / On Primary |
| Disabled | 38% | On Surface (容器) + 38% On Surface (内容) |

---

## 7. 动效规范

### 7.1 动画时长

| 动画类型 | 时长 (ms) | 说明 |
|---------|----------|------|
| Emphasized (大幅) | 500 | 页面转场、容器变换 |
| Emphasized Decelerate | 500 | 减速进入（元素出现） |
| Emphasized Accelerate | 500 | 加速退出（元素消失） |
| Standard (标准) | 300 | 组件状态切换、展开收起 |
| Standard Decelerate | 300 | 标准减速进入 |
| Standard Accelerate | 300 | 标准加速退出 |
| Emphasized Short | 200 | 短强调动画 |
| Standard Short | 150 | 短标准动画 |

### 7.2 缓动曲线

| 曲线名称 | 参数 | 用途 |
|---------|------|------|
| Emphasized | cubic-bezier(0.2, 0, 0, 1) | 大幅转场 |
| Emphasized Decelerate | cubic-bezier(0.05, 0.7, 0.1, 1) | 元素出现 |
| Emphasized Accelerate | cubic-bezier(0.3, 0, 0.8, 0.15) | 元素消失 |
| Standard | cubic-bezier(0.2, 0, 0, 1) | 标准转场 |
| Standard Decelerate | cubic-bezier(0, 0, 0, 1) | 标准减速 |
| Standard Accelerate | cubic-bezier(0.3, 0, 1, 1) | 标准加速 |
| Linear | cubic-bezier(0, 0, 1, 1) | 线性（加载动画） |

### 7.3 转场模式 (Motion Patterns)

| 转场类型 | 描述 | 时长 |
|---------|------|------|
| Container Transform | 容器形态变换（如Card展开为页面） | 500ms |
| Shared Axis | 共享轴转场（同方向元素滑入滑出） | 300ms |
| Fade Through | 淡入淡出交叉（无空间关系元素） | 300ms |
| Fade | 简单淡入淡出（微交互） | 150-200ms |

### 7.4 共享轴方向

| 轴向 | 动画描述 | 用途 |
|------|---------|------|
| X轴 (水平) | 元素沿水平方向滑入/滑出 | 前进/后退导航 |
| Y轴 (垂直) | 元素沿垂直方向滑入/滑出 | 上下层级切换 |
| Z轴 (深度) | 元素缩放淡入/淡出 | 同级切换 |

---

## 8. 图标规范

### 8.1 Material Symbols 参数

| 图标用途 | 尺寸 (dp) | 线宽 (optical size) | 说明 |
|---------|----------|-------------------|------|
| Navigation Bar图标 | 24dp | 40 (Regular) | 底部导航 |
| TopAppBar图标 | 24dp | 40 (Regular) | 顶部导航 |
| FAB图标 | 24dp | 40 (Regular) | 浮动操作按钮 |
| 列表行图标 | 24dp | 40 (Regular) | 列表辅助图标 |
| 小型图标 | 20dp | 20 (Small) | 行内图标 |
| 超大图标 | 40dp | 48 (Large) | 空状态、引导 |
| App图标 | 48dp | - | 启动器图标 |

### 8.2 Material Symbols 线宽变体

| 变体名称 | 线宽 (dp) @ 24dp | 用途 |
|---------|-----------------|------|
| Thin | 0.5 | 极细线宽 |
| Light | 1.0 | 细线宽 |
| Regular | 1.5 | 标准线宽 |
| Medium | 2.0 | 中等线宽 |
| Bold | 2.5 | 粗线宽 |
| Filled | 填充 | 选中态 |

### 8.3 图标尺寸规格

| 参数 | 数值 (dp) | 说明 |
|------|----------|------|
| 图标网格 | 24x24dp | 标准图标画布 |
| 图标安全区 | 20x20dp | 图标内容区域 |
| 图标触控区域 | 48x48dp | 最小触控热区 |
| App图标画布 | 108x108dp | 启动器图标 |
| App图标安全区 | 80x80dp | 图标内容区域 |

---

## 9. 核心组件规范

### 9.1 Top App Bar

| 参数 | 数值 (dp) | 说明 |
|------|----------|------|
| 标准高度 | 64dp | 含操作区域 |
| Small TopAppBar高度 | 64dp | 紧凑模式 |
| Medium TopAppBar高度 | 112dp | 含副标题区域 |
| Large TopAppBar高度 | 152dp | 含大标题区域 |
| 标题字号 | 22sp Regular (Title Large) | 标题文字 |
| 导航图标尺寸 | 24dp | 返回/菜单图标 |
| 操作图标尺寸 | 24dp | 右侧操作图标 |
| 操作图标间距 | 4dp | 图标间水平间距 |
| 操作触控区域 | 48x48dp | 最小触控热区 |
| 底部分隔线 | 1dp #CAC4D0 | 分隔线 |

### 9.2 Navigation Bar (底部导航)

| 参数 | 数值 (dp) | 说明 |
|------|----------|------|
| 高度 | 80dp | 含标签区域 |
| 图标尺寸 | 24dp | 导航图标 |
| 选中态图标 | Filled变体 24dp | 填充图标 |
| 未选中态图标 | Outlined变体 24dp | 线性图标 |
| 标签字号 | 12sp Medium (Label Medium) | 导航标签 |
| 选中态指示器 | 32x32dp圆角16dp #EADDFF | 选中态背景药丸背景 |
| 选中态图标色 | #6750A4 (浅) / #D0BCFF (深) | Primary色 |
| 未选中态图标色 | #49454F (浅) / #CAC4D0 (深) | On Surface Variant |
| 最多Tab数 | 5个 | 底部导航上限 |
| 最少Tab数 | 3个 | 底部导航下限 |

### 9.3 按钮 (Button)

| 按钮类型 | 高度 (dp) | 圆角 (dp) | 字号/字重 | 背景色 | 文字色 |
|---------|----------|----------|----------|-------|-------|
| Filled Button | 40dp | 20dp (Full) | 14sp Medium | #6750A4 | #FFFFFF |
| Filled Tonal Button | 40dp | 20dp (Full) | 14sp Medium | #EADDFF | #21005D |
| Outlined Button | 40dp | 20dp (Full) | 14sp Medium | 透明 | #6750A4 |
| Text Button | 40dp | 20dp (Full) | 14sp Medium | 透明 | #6750A4 |
| Elevated Button | 40dp | 20dp (Full) | 14sp Medium | #EADDFF + Elevation 1 | #21005D |
| FAB | 56dp | 16dp | - | #6750A4 | #FFFFFF |
| Small FAB | 40dp | 12dp | - | #6750A4 | #FFFFFF |
| Large FAB | 96dp | 28dp | - | #6750A4 | #FFFFFF |
| Extended FAB | 56dp | 16dp | 14sp Medium | #6750A4 | #FFFFFF |
| Icon Button | 48x48dp | - | - | 透明 | #49454F |

### 9.4 输入框 (Text Field)

| 参数 | 数值 (dp) | 说明 |
|------|----------|------|
| Filled TextField高度 | 56dp | 填充输入框 |
| Outlined TextField高度 | 56dp | 描边输入框 |
| 输入框圆角 | 4dp (Extra Small) | Outlined底部/Outlined全圆角 |
| 输入字号 | 16sp Regular (Body Large) | 正文输入 |
| 标签字号 | 12sp Medium (Label Small) | 浮动标签 |
| 占位文字字号 | 16sp Regular | 占位提示 |
| 输入框内边距 | 16dp水平 | 左右内边距 |
| 描边宽度 | 1dp (默认) / 2dp (聚焦) | Outlined边框 |
| 描边颜色 | #79747E (默认) / #6750A4 (聚焦) / #B3261E (错误) | 边框色 |
| SearchBar高度 | 56dp | 搜索栏 |
| SearchBar圆角 | 28dp (Extra Large) | 全圆角搜索栏 |

### 9.5 卡片 (Card)

| 参数 | 数值 (dp) | 说明 |
|------|----------|------|
| 卡片圆角 | 12dp (Medium) | 标准卡片 |
| 卡片内边距 | 16dp | 内容区边距 |
| Elevated Card背景色 | #F7F2FA (浅) / #1D1B20 (深) | 提升卡片 |
| Filled Card背景色 | #E7E0EC (浅) / #49454F (深) | 填充卡片 |
| Outlined Card背景色 | #FFFBFE (浅) / #1C1B1F (深) | 描边卡片 |
| Outlined Card描边 | 1dp #CAC4D0 | 描边宽度 |
| 卡片间距 | 8dp | 卡片间垂直间距 |
| Elevated Card Elevation | 1dp | 提升阴影 |
| 卡片标题字号 | 16sp Medium (Title Medium) | 卡片标题 |
| 卡片副标题字号 | 14sp Regular (Body Medium) | 卡片副标题 |

### 9.6 弹窗 (Dialog / Bottom Sheet)

| 参数 | 数值 (dp) | 说明 |
|------|----------|------|
| Dialog圆角 | 28dp (Extra Large) | 弹窗圆角 |
| Dialog最小宽度 | 280dp | 弹窗最小宽度 |
| Dialog最大宽度 | 560dp | 弹窗最大宽度 |
| Dialog标题字号 | 24sp Regular (Headline Small) | 标题 |
| Dialog内容字号 | 14sp Regular (Body Medium) | 描述文字 |
| Dialog按钮高度 | 40dp | 操作按钮 |
| Dialog按钮字号 | 14sp Medium (Label Large) | 按钮文字 |
| Dialog Elevation | 6dp (浅色) / Tonal (深色) | 弹窗层级 |
| Bottom Sheet圆角 | 28dp (顶部) | 底部面板 |
| Bottom Sheet拖拽指示器 | 32x4dp | 顶部横条 |
| Bottom Sheet Elevation | 0dp (浅色) / Tonal (深色) | 底部面板层级 |

### 9.7 开关 (Switch)

| 参数 | 数值 (dp) | 说明 |
|------|----------|------|
| 宽度 | 52dp | 开关总宽 |
| 高度 | 32dp | 开关总高 |
| 选中态滑块尺寸 | 24dp | 选中态圆形滑块 |
| 未选中态滑块尺寸 | 16dp | 未选中态小滑块 |
| 选中态轨道色 | #6750A4 (浅) / #D0BCFF (深) | Primary色 |
| 未选中态轨道色 | #E7E0EC (浅) / #49454F (深) | Surface Variant |
| 选中态滑块色 | #FFFFFF (浅) / #381E72 (深) | On Primary |
| 未选中态滑块色 | #79747E (浅) / #938F99 (深) | Outline |
| 选中态边框 | 0dp | 无边框 |
| 未选中态边框 | 2dp #79747E | 描边 |

---

## 10. 设计禁忌

### 10.1 绝对禁止

1. **禁止使用固定色值**：必须使用Material You动态取色系统，不得硬编码色值，确保用户壁纸主题色生效
2. **禁止使用iOS风格组件**：不得使用iOS风格的导航栏、TabBar、返回按钮等，必须遵循Material Design组件规范
3. **禁止忽略Tonal Elevation**：深色模式下不得使用阴影，必须使用色调提升区分层级
4. **禁止自定义系统控件**：Switch、Slider、ProgressBar等必须使用Material 3标准组件
5. **禁止忽略状态层**：所有可交互组件必须包含Hover/Focus/Pressed状态层反馈
6. **禁止使用非标准圆角**：组件圆角必须从Shape系统取值，不得自定义非标准圆角数值
7. **禁止忽略断点适配**：必须支持Compact/Medium/Expanded三档布局，不得仅适配手机尺寸
8. **禁止使用线性动画**：转场动画必须使用Emphasized/Standard曲线，不得使用linear

### 10.2 强烈不建议

1. 不建议在深色模式下使用纯白(#FFFFFF)背景
2. 不建议在Navigation Bar中使用超过5个Tab
3. 不建议忽略无障碍对比度要求（文字与背景对比度不低于4.5:1）
4. 不建议使用小于48dp的触控热区
5. 不建议在FAB中使用文字而非图标
6. 不建议忽略Window Insets适配
7. 不建议使用自定义转场动画替代Material Motion
8. 不建议在Card中使用超过2级嵌套
