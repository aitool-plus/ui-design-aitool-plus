---
name: ui-design-father-skill
description: |
  One-Person Design Company God-Tier Skill. Covers 11 platform design systems: Apple iOS HIG, Google Material Design 3, Samsung One UI, Huawei HarmonyOS, Xiaomi HyperOS, Honor MagicOS, OPPO ColorOS, vivo OriginOS, Meizu Flyme, Windows 11 Fluent Design, WeChat Mini Program WeUI. Auto-activates when users need mobile app UI, desktop app UI, mini-program UI, multi-platform adaptation, component library design, or design system documentation. Supports keywords: iOS, Android, Material Design, One UI, HarmonyOS, HyperOS, MagicOS, ColorOS, OriginOS, Flyme, Windows, Fluent, WeChat, WeUI, mini-program.
version: 1.0.0
author: aitool.plus
---

# ui-design-father-skill

一人设计公司神级Skill，覆盖手机App、小程序、Windows桌面三大平台，内置11大主流OS/平台设计规范，一条指令即可输出原厂级高保真UI方案。

---

## 一、前置硬规则（HARD RULES）

以下规则在整个会话内强制生效，不得违反：

### 1.1 风格锁定规则

一旦用户选定目标风格，整个会话内所有输出必须严格遵循该风格的设计规范，不得混入其他风格元素。例如：选定iOS后禁止出现Material Design的FAB按钮或Fluent的Acrylic材质。

### 1.2 原厂规范优先规则

所有设计参数（圆角、间距、字号、色值、动效曲线等）必须引用对应平台官方设计规范中的标准值，禁止凭感觉编造。参数来源优先级：
1. 平台官方设计规范文档（Apple HIG / Material Design 3 / Fluent Design / WeUI / 各厂商规范）
2. 对应平台的 `references/styles/{style}.md` 文件
3. 仅在上述均无覆盖时，依据平台设计语言推导并标注"推导值"

### 1.3 组件完整性规则

每个组件必须覆盖以下状态与变体：

| 维度 | 必须覆盖项 |
|------|-----------|
| 交互状态 | 默认、悬停/按下、禁用、加载 |
| 主题变体 | 浅色模式、深色模式 |
| 尺寸变体 | 按对应平台规范（如iOS: Small/Default/Large；Windows: Small/Medium/Large） |

### 1.4 响应式适配规则

所有布局必须支持四种断点：

| 断点 | 宽度范围 | 典型设备 |
|------|---------|---------|
| 手机 | 375-428dp | iPhone 15 / 小米14 / 三星S24 |
| 折叠屏 | 600-840dp | Galaxy Z Fold / Mate X5 / Find N3 |
| 平板 | 840-1280dp | iPad Air / MatePad Pro / Galaxy Tab |
| 桌面 | 1280dp+ | Windows PC / Surface / 外接显示器 |

### 1.5 平台适配规则

根据目标平台强制遵循对应设计体系：
- 手机App：遵循对应OS规范（iOS/Android/HarmonyOS等）
- 微信小程序：遵循WeUI规范，跨OS统一视觉
- Windows桌面：遵循Fluent Design规范，适配键鼠交互

### 1.6 无障碍规则

所有组件必须满足WCAG 2.1 AA级标准：文本对比度不低于4.5:1，大文本对比度不低于3:1，交互元素最小触控区域44x44pt，必须提供无障碍标签。

---

## 二、风格路由表

根据用户输入的关键词自动匹配风格，加载对应规范文件：

| 风格名称 | 触发关键词 | 规范文件路径 | 核心特征 | 适用平台 |
|----------|-----------|-------------|---------|---------|
| Apple iOS | iOS, 苹果, iPhone, Apple HIG, iPad | references/styles/apple-ios.md | SF字体、大标题、毛玻璃、圆角卡片、4pt网格 | 手机App |
| Google Android | Android, Material, 谷歌, MD3, Material You | references/styles/google-android.md | Material You、动态取色、响应式网格、8dp基准 | 手机App |
| Samsung One UI | Samsung, One UI, 三星, 折叠屏 | references/styles/samsung-one-ui.md | 大圆角、单手操作区、高斯模糊、折叠屏适配 | 手机App |
| 华为 HarmonyOS | 鸿蒙, Harmony, 华为, 服务卡片 | references/styles/huawei-harmonyos.md | 服务卡片、弹性动效、分布式、8vp网格 | 手机App |
| 小米 HyperOS | 小米, HyperOS, 澎湃, MIUI | references/styles/xiaomi-hyperos.md | 年轻化、高信息密度、生态互联、渐变圆角 | 手机App |
| 荣耀 MagicOS | 荣耀, MagicOS, Honor | references/styles/honor-magicos.md | 商务质感、均衡克制、高效交互、圆润过渡 | 手机App |
| OPPO ColorOS | OPPO, ColorOS, 欧珀 | references/styles/oppo-coloros.md | 灵动活力、无边界、智能组件、水波纹动效 | 手机App |
| vivo OriginOS | vivo, OriginOS, 原子组件 | references/styles/vivo-originos.md | 华容网格、原子组件、个性化、3D景深 | 手机App |
| 魅族 Flyme | 魅族, Flyme, 极简 | references/styles/meizu-flyme.md | 极简克制、大面积留白、雅致、8px网格 | 手机App |
| Windows 11 Fluent | Windows, Fluent, Win11, 桌面, PC | references/styles/windows-fluent.md | 亚克力材质、Mica、揭示高亮、4px网格、键鼠优先 | Windows桌面 |
| 微信小程序 WeUI | 微信, WeChat, WeUI, 小程序 | references/styles/wechat-miniprogram.md | WeUI组件库、跨OS统一、微信生态色、4px基准 | 微信小程序 |

**路由规则：**
- 用户输入含多个风格关键词时，优先匹配第一个明确指定的风格
- 用户未指定时，根据"设备类型/品牌型号/App目标平台"推断
- 推断失败时，主动询问用户选择目标风格

---

## 三、八步工作流

### Step 1: 需求分析

引用: `references/workflow/analysis-framework.md`

解析用户需求，明确以下维度：
- **目标平台**: 手机App / 微信小程序 / Windows桌面
- **目标风格**: 从路由表匹配或主动询问
- **页面类型**: 启动页/首页/列表页/详情页/表单页/设置页/个人中心等
- **功能模块**: 导航/搜索/列表/卡片/弹窗/标签栏等
- **用户群体**: 消费者/企业/特定年龄段
- **适配形态**: 仅手机 / 手机+折叠屏 / 全端 / 桌面

同时检查是否存在 `EXTEND.md`，加载用户偏好配置。

### Step 2: 风格确认

引用: `references/workflow/confirmation.md`

向用户展示匹配的风格核心特征摘要，确认选择：
- **单风格模式**: 确认目标风格后锁定，后续输出严格遵循
- **多风格对比模式**: 用户可选择2-3个风格，对同一需求生成对比方案

确认信息包括：主色方向、主题偏好（浅/深/双模式）、设备优先级。

### Step 3: 设计系统生成

引用: `references/design-tokens/token-architecture.md` + `references/styles/{style}.md`

读取对应风格规范文件，生成完整的 Design Token 体系：

| Token类别 | 生成内容 |
|-----------|---------|
| 色彩 | 主色/辅助色/功能色/中性色/浅色模式/深色模式 |
| 字体 | 字体族/字号阶梯/字重/行高/字间距 |
| 间距 | 基准网格/内间距/外间距/组件间距 |
| 圆角 | 小/中/大/全圆角值 |
| 阴影 | 层级1-4阴影参数 |
| 动效 | 时长/缓动曲线/弹性参数 |

输出为CSS自定义属性格式，可直接嵌入HTML原型。

### Step 4: 组件规范输出

引用: `references/components/` 目录下对应文件

根据需求选择组件类型，输出组件规范：

| 组件类别 | 典型组件 |
|----------|---------|
| 导航 | 顶部导航栏/底部标签栏/侧边导航/面包屑 |
| 按钮 | 主按钮/次按钮/文字按钮/图标按钮 |
| 输入 | 文本框/搜索框/下拉选择/开关 |
| 展示 | 卡片/列表项/标签/徽标/头像 |
| 反馈 | 弹窗/Toast/进度条/空状态 |
| 容器 | 标签页/手风琴/折叠面板 |

每个组件必须包含：5种交互状态 + 浅/深色主题变体 + 响应式断点适配。

### Step 5: 页面原型生成

引用: `references/workflow/output-template.md`

组合设计系统 + 组件规范，生成高保真页面原型：
- 优先输出可交互的HTML/CSS单文件原型
- 原型必须包含双主题切换（浅色/深色）
- 原型必须包含至少一种响应式断点适配
- 所有图片使用本地文件或Unsplash，禁止空src

### Step 6: 审查与迭代

引用: `references/workflow/iteration-guide.md`

对照平台官方规范检查还原度，检查项：

| 检查维度 | 检查内容 |
|----------|---------|
| 色彩还原 | 是否使用平台标准色值/色板体系 |
| 字体还原 | 是否使用平台规范字体族与字号阶梯 |
| 间距还原 | 是否遵循平台基准网格 |
| 圆角还原 | 是否符合平台圆角规范 |
| 动效还原 | 是否使用平台标准缓动曲线 |
| 交互还原 | 是否符合平台交互范式 |
| 组件还原 | 是否覆盖平台规范要求的所有组件状态 |
| 平台适配 | 是否符合目标平台特有规范（键鼠/手势/导航等） |

输出还原度评分（0-100）及具体迭代建议。

### Step 7: 交付输出

输出完整交付包，包含：

| 交付物 | 格式 | 说明 |
|--------|------|------|
| 设计规范文档 | Markdown | 完整Design Token + 组件规范 + 页面规范 |
| 组件库 | HTML/CSS | 可复用的组件代码片段 |
| 页面原型 | HTML单文件 | 可交互高保真原型，含双主题+响应式 |
| 前端样式参考 | CSS/SCSS | Design Token CSS变量 + 组件样式类 |

### Step 8: Demo生成

为每个风格生成独立的可运行HTML Demo页面：
- 存放路径: `demo/{style-name}/index.html`
- 必须是单文件HTML，可直接浏览器打开
- 必须包含浅色/深色主题切换
- 必须展示该风格的核心组件和视觉特征
- 手机端Demo默认375dp视口，Windows端Demo默认1280dp视口，小程序Demo默认375dp视口

---

## 四、References 引用表

### 4.1 风格规范文件

| 文件路径 | 用途 | 加载时机 |
|----------|------|---------|
| references/styles/apple-ios.md | Apple iOS设计规范 | Step 3，匹配iOS时加载 |
| references/styles/google-android.md | Material Design 3规范 | Step 3，匹配Android时加载 |
| references/styles/samsung-one-ui.md | Samsung One UI设计规范 | Step 3，匹配One UI时加载 |
| references/styles/huawei-harmonyos.md | 华为HarmonyOS设计规范 | Step 3，匹配鸿蒙时加载 |
| references/styles/xiaomi-hyperos.md | 小米HyperOS设计规范 | Step 3，匹配澎湃时加载 |
| references/styles/honor-magicos.md | 荣耀MagicOS设计规范 | Step 3，匹配荣耀时加载 |
| references/styles/oppo-coloros.md | OPPO ColorOS设计规范 | Step 3，匹配ColorOS时加载 |
| references/styles/vivo-originos.md | vivo OriginOS设计规范 | Step 3，匹配OriginOS时加载 |
| references/styles/meizu-flyme.md | 魅族Flyme设计规范 | Step 3，匹配Flyme时加载 |
| references/styles/windows-fluent.md | Windows 11 Fluent Design规范 | Step 3，匹配Windows时加载 |
| references/styles/wechat-miniprogram.md | 微信小程序WeUI规范 | Step 3，匹配微信小程序时加载 |

### 4.2 设计Token架构

| 文件路径 | 用途 | 加载时机 |
|----------|------|---------|
| references/design-tokens/token-architecture.md | Token分层架构与命名规范 | Step 3，生成Design Token时加载 |

### 4.3 组件规范

| 文件路径 | 用途 | 加载时机 |
|----------|------|---------|
| references/components/navigation.md | 导航类组件规范 | Step 4，涉及导航组件时加载 |
| references/components/input-controls.md | 输入控件规范（按钮/输入框/开关/滑块/复选框/下拉选择） | Step 4，涉及输入控件时加载 |
| references/components/data-display.md | 数据展示组件规范（列表/卡片/标签/表格/头像） | Step 4，涉及展示组件时加载 |
| references/components/feedback.md | 反馈组件规范（弹窗/Toast/进度条/空状态/骨架屏） | Step 4，涉及反馈组件时加载 |
| references/components/media.md | 媒体组件规范（图片/头像组/图标/插画/横幅） | Step 4，涉及媒体组件时加载 |

### 4.4 工作流辅助

| 文件路径 | 用途 | 加载时机 |
|----------|------|---------|
| references/workflow/analysis-framework.md | 需求分析框架 | Step 1，每次启动时加载 |
| references/workflow/confirmation.md | 风格确认流程 | Step 2，确认风格时加载 |
| references/workflow/output-template.md | 输出模板与格式规范 | Step 5，生成原型时加载 |
| references/workflow/iteration-guide.md | 审查标准与迭代指引 | Step 6，审查还原度时加载 |

### 4.5 用户偏好

| 文件路径 | 用途 | 加载时机 |
|----------|------|---------|
| EXTEND.md | 用户自定义偏好与扩展配置 | Step 1，每次启动时检查 |

---

## 五、多风格对比模式

当用户选择多风格对比时（如"帮我对比iOS和鸿蒙的首页设计"），执行以下流程：

1. 对同一需求分别按各风格规范独立生成设计方案
2. 输出横向对比表，维度包括：

| 对比维度 | 说明 |
|----------|------|
| 色彩体系 | 主色/辅助色/中性色差异 |
| 字体排版 | 字体族/字号阶梯差异 |
| 间距与网格 | 基准网格与间距规律差异 |
| 圆角规范 | 圆角大小层级差异 |
| 组件风格 | 同一组件在不同平台下的视觉差异 |
| 交互范式 | 导航/返回/弹窗等交互差异 |
| 动效特征 | 缓动曲线/时长/弹性参数差异 |
| 平台特性 | 各平台独有能力（如鸿蒙卡片/Fluent亚克力/WeUI微信能力） |

3. 每个风格独立输出原型，可分别预览
4. 提供选型建议，基于：目标市场/用户习惯/开发成本/品牌调性/平台生态

---

## 六、输出格式

支持以下四种输出格式，根据用户需求选择：

| 格式 | 适用场景 | 说明 |
|------|---------|------|
| 高保真HTML原型 | 交互演示、视觉评审 | 单文件HTML，含CSS/JS，可直接浏览器打开 |
| 设计规范Markdown文档 | 开发交接、团队协作 | 完整Token + 组件规范 + 使用说明 |
| CSS/SCSS样式代码 | 前端开发集成 | Design Token变量 + 组件样式类 + 工具类 |
| Figma标注参数 | 设计师协作 | 各组件的精确参数值（字号/色值/间距/圆角） |

---

## 七、示例

### 示例1: iOS电商首页

用户输入: "用iOS风格设计一个电商App首页"

执行流程:
1. 平台判定: 手机App -> 路由匹配iOS -> 加载 `references/styles/apple-ios.md`
2. 确认: 主色方向(科技蓝/活力橙/自定义)、设备(Mobile优先)
3. 生成Design Token: SF Pro字体、iOS系统色、4pt网格、iOS圆角阶梯
4. 输出组件: iOS风格导航栏、标签栏、商品卡片、搜索框、Banner
5. 生成原型: 单HTML文件，含浅/深色切换，375dp基准
6. 审查: 对照Apple HIG检查还原度，输出评分与建议
7. 交付: 完整设计规范 + 组件库 + 可交互原型
8. Demo: 生成 `demo/apple-ios/index.html`

### 示例2: iOS vs 鸿蒙 vs Windows设置页三端对比

用户输入: "对比iOS、鸿蒙和Windows的设置页设计"

执行流程:
1. 平台判定: 手机App + 手机App + Windows桌面 -> 分别加载三个规范文件
2. 确认: 确认三个风格均需输出
3. 分别生成三套Design Token
4. 分别输出三套组件规范（iOS分组列表/鸿蒙卡片列表/Fluent导航视图）
5. 生成三个独立原型 + 横向对比表
6. 审查: 分别评分 + 差异分析
7. 交付: 三方案交付包 + 对比分析报告 + 选型建议
8. Demo: 分别生成 `demo/apple-ios/index.html`、`demo/huawei-harmonyos/index.html`、`demo/windows-fluent/index.html`

### 示例3: 微信小程序点餐页面

用户输入: "用微信小程序风格设计一个奶茶点餐页面"

执行流程:
1. 平台判定: 微信小程序 -> 路由匹配WeUI -> 加载 `references/styles/wechat-weui.md`
2. 确认: 主色方向(品牌绿)、WeUI组件范围
3. 生成Design Token: WeUI色彩、字体、4px基准间距
4. 输出组件: WeUI风格商品列表、购物车栏、分类标签、下单按钮
5. 生成原型: 单HTML文件，375dp视口，模拟小程序容器
6. 审查: 对照WeUI规范检查还原度
7. 交付: 完整设计规范 + 组件库 + 可交互原型
8. Demo: 生成 `demo/wechat-miniprogram/index.html`

---

## 八、Demo生成规则

1. 每个风格必须生成独立的HTML Demo页面
2. Demo存放路径: `demo/{style-name}/index.html`（style-name见路由表风格名称列对应英文标识）
3. Demo必须是单文件HTML（含内联CSS/JS），可直接浏览器打开
4. Demo必须包含浅色/深色主题切换按钮
5. Demo必须展示该风格的核心组件和视觉特征
6. 手机端Demo默认375dp视口，Windows桌面端Demo默认1280dp视口
7. 微信小程序Demo需模拟小程序顶部导航栏和底部安全区域
8. Demo中使用的所有Design Token必须与Step 3生成的Token体系完全一致
