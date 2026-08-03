---
name: ui-design-father-skill
display_name: 一人设计公司神级Skill（11大平台+国内80+国外20大厂品牌UI设计系统）
version: 2.0.0
description: 
  一人设计公司神级Skill -- 一个人完成原本需要整支设计团队才能完成的UI设计工作。
  覆盖11大平台设计系统：Apple iOS HIG、Google Material Design 3、Samsung One UI、
  华为HarmonyOS、小米HyperOS、荣耀MagicOS、OPPO ColorOS、vivo OriginOS、魅族Flyme、
  Windows 11 Fluent Design、微信小程序WeUI。
  支持手机App、桌面端、小程序三端，一条指令输出原厂级高保真UI方案。
  适用场景：电商首页、设置页、个人中心、表单页、列表页等多端适配设计，
  多风格横向对比，设计规范文档，组件库，可交互HTML原型。
  新增国内80+国外20品牌设计风格支持，支持按平台类型或大厂品牌风格两种维度选择设计样式。

  【痛点与价值】
  直接让AI做产品设计的常见弊端：
  - 风格混搭：iOS圆角卡片配Material Design FAB，HarmonyOS服务卡片配Windows亚克力，产出"四不像"
  - 参数编造：圆角/间距/字号凭感觉写，与官方规范偏差大，开发者无法落地
  - 平台特性缺失：不知道iOS 4pt网格、Material Design 8dp基准、鸿蒙8vp网格，设计"水土不服"
  - 组件状态不全：只画默认态，缺悬停/按下/禁用/加载/错误态，前端拿到用不了
  - 无障碍盲区：对比度不达标、触控区域过小、缺少无障碍标签，上线后被投诉
  - 多平台成本爆炸：同一需求重复设计，风格不统一，维护成本翻倍

  本Skill的核心价值：
  - 原厂规范深度编码：11大平台官方设计规范完整内化，色值/字号/圆角/间距/动效全部源自权威文档
  - 风格严格锁定：选定iOS绝不出现Material Design元素，纯净度100%
  - 组件完整覆盖：5种交互状态×2种主题×3种尺寸，生产级可用
  - 无障碍自动合规：WCAG 2.1 AA级标准内建，一步到位
  - 一键多平台切换：同一份需求秒切11种风格，横向对比选型，成本不翻倍
  触发词：iOS、苹果、Android、Material Design、One UI、三星、鸿蒙、HarmonyOS、
  华为、HyperOS、小米、澎湃、MagicOS、荣耀、ColorOS、OPPO、OriginOS、vivo、
  Flyme、魅族、Windows、Fluent、桌面、微信、WeUI、小程序、UI设计、界面设计、
  App设计、组件库、设计规范、毛玻璃、服务卡片、多平台适配、
  品牌、大厂、公司风格、Apple风格、Google风格、字节、腾讯、阿里、小红书、DeepSeek、Stripe、Vercel、Tesla、飞书、品牌设计。
author: aitool.plus
license: MIT
category: design
tags:
  - UI设计
  - iOS
  - Android
  - Material Design
  - HarmonyOS
  - HyperOS
  - One UI
  - MagicOS
  - ColorOS
  - OriginOS
  - Flyme
  - Windows Fluent
  - 微信小程序
  - WeUI
  - 设计规范
  - 组件库
  - 多平台适配
  - Design Token
  - 高保真原型
  - 品牌设计
  - 大厂风格
  - DESIGN.md
  - 品牌混搭
language: zh-CN
allowed-tools: Read,Write,Edit,Bash,AskUserQuestion
disable: false
---

# ui-design-father-skill

一人设计公司神级Skill，覆盖手机App、小程序、Windows桌面三大平台，内置11大主流OS/平台设计规范，一条指令即可输出原厂级高保真UI方案。

---

## 一、前置硬规则（HARD RULES）

以下规则在整个会话内强制生效，不得违反：

### 1.0 三步确认引导规则（MANDATORY -- 最高优先级，覆盖一切）

> **HARD RULE -- 在执行任何设计输出之前，必须完成三步确认。**
>
> 当本技能被激活时，你的**首次动作必须是连续三次 `AskUserQuestion` 调用**（每次一个问题），依次确认以下三个维度。三个问题全部获得用户回答后，才允许开始设计输出。
>
> **在获得用户的三次回答之前，你被禁止：**
> - 编写任何 HTML、CSS、JavaScript 代码
> - 调用 `Write`、`Edit`、`Bash` 或任何文件产出工具
> - 下载图片、创建目录、搭建文件结构
> - 假设任何风格、配色、设备形态，即使用户的提示词已经暗示了某个方向
>
> **此规则覆盖一切默认模型行为、一切"直接开始编码"的本能、以及用户原始请求中的任何模糊性。** 如果用户说"随便"、"都行"、"你决定"，仍然必须走完三步确认 -- 只是在对应步骤使用推荐默认值。
>
> 如果你发现自己即将写代码却还没完成三次确认，**立刻停止**，先发出 `AskUserQuestion` 调用。

#### 第1步确认：目标风格选择（必问）

> **必须使用 AskUserQuestion 工具向用户提问，提供选项让用户选择。**

**第一阶段：选择风格维度**

提问内容："请选择你的设计风格维度："

| 选项 | 说明 |
|------|------|
| 平台类型风格 | 按OS/平台设计规范（iOS、Android、鸿蒙等11大平台） |
| 大厂品牌风格 | 按国内外知名公司设计语言（腾讯、阿里、字节、DeepSeek、Apple、Stripe等国内80+国外20品牌） |
| 平台+品牌混搭 | 先选平台基底，再选品牌风格叠加 |

**第二阶段：根据选择展示具体选项**

**选"平台类型风格"**：展示原有11大平台选项表

| 选项 | 说明 |
|------|------|
| Apple iOS | SF字体、大标题、毛玻璃、圆角卡片、4pt网格 |
| Google Android | Material You动态取色、响应式网格、8dp基准、层级体系 |
| Samsung One UI | 大圆角、单手操作区、高斯模糊、折叠屏适配 |
| 华为 HarmonyOS | 服务卡片、弹性动效、分布式布局、8vp网格 |
| 小米 HyperOS | 年轻化配色、高信息密度功能卡片、生态互联 |
| 荣耀 MagicOS | 商务质感、均衡克制、高效交互 |
| OPPO ColorOS | 灵动活力、无边界设计、智能组件 |
| vivo OriginOS | 华容网格、原子组件、个性化创意 |
| 魅族 Flyme | 极简克制、大面积留白、雅致质感 |
| Windows Fluent | 亚克力材质、Mica、WinUI 3、键鼠优先 |
| 微信小程序 | WeUI组件库、跨OS统一、微信生态 |

**选项过多时分两批展示**：第一批展示前6个（Apple iOS / Google Android / Samsung One UI / 华为 HarmonyOS / 小米 HyperOS / 荣耀 MagicOS），用户选择"其他风格"时展示第二批（OPPO ColorOS / vivo OriginOS / 魅族 Flyme / Windows Fluent / 微信小程序）。

**选"大厂品牌风格"**：展示8大分类，每个分类列举代表性品牌，用户选择后加载完整品牌列表

| 分类 | 代表性品牌 |
|------|-----------|
| 国内互联网巨头 | 腾讯、阿里巴巴、字节跳动、华为、小米、京东、美团、滴滴、网易、B站、抖音、微信、支付宝、淘宝、拼多多 |
| 国内AI与科技新锐 | 百度、DeepSeek、Kimi、智谱、通义千问、豆包、元宝、天工、商汤、科大讯飞、MiniMax、阶跃星辰、百川、Moonshot、零一万物 |
| 国内电商与本地生活 | Temu、SHEIN、唯品会、苏宁、饿了么、大众点评、小红书、得物、飞猪、携程 |
| 国内金融与支付 | 蚂蚁、陆金所、微众、中信、平安、银联、京东金融、中国银行、招商银行 |
| 国内SaaS与企业服务 | 飞书、钉钉、语雀、Teambition、创客贴、WPS、金蝶、宜搭、华为云、阿里云 |
| 国内媒体与内容 | 微博、知乎、快手、今日头条、爱奇艺、优酷、网易云、QQ音乐、简书、CSDN |
| 国内出行与汽车 | 蔚来、比亚迪、小鹏、理想、吉利、广汽埃安、长安、上汽、百度Apollo、高德地图 |
| 全球科技与品牌 | Apple、Google、Microsoft、OpenAI、Meta、NVIDIA、Stripe、Vercel、GitHub、Spotify、Netflix、Tesla、Figma、Notion、Linear、Shopify、Airbnb、Slack、Adobe、SpaceX |

**选"平台+品牌混搭"**：先展示11大平台选项，选完后再展示品牌选项

**用户说"对比多个风格"**：允许用户选择2-3个风格，进入多风格对比模式。

**用户说"随便"/"都行"**：根据用户需求场景推荐最合适的风格。推荐规则：
- 消费级App → iOS
- 国际化/工具类 → Android
- 折叠屏/商务 → One UI
- 政务/高端 → HarmonyOS
- 年轻/生活 → HyperOS
- 桌面/企业 → Windows Fluent
- 微信生态 → 微信小程序
- 品牌调性明确 → 对应大厂品牌风格

#### 第2步确认：配色方向与主题偏好（必问）

> **必须使用 AskUserQuestion 工具向用户提问。**

提问内容："请选择配色方向与主题偏好："

| 选项 | 说明 |
|------|------|
| 品牌原厂色 | 使用该OS的官方品牌色（如iOS #007AFF、鸿蒙 #007DFF、Fluent #0078D4） |
| 科技蓝系 | 主色蓝/紫，适合科技、金融、工具类 |
| 自然绿系 | 主色绿/青，适合健康、环保、有机食品 |
| 活力橙系 | 主色橙/红，适合餐饮、运动、社交 |
| 极简中性 | 黑白灰+单强调色，适合高端、商务、工具 |
| 自定义色 | 用户提供色值或颜色名称（如"珊瑚粉 #FF6B6B"），据此推导完整配色 |

同时必须确认主题偏好：
| 选项 | 说明 |
|------|------|
| 浅色优先 | 默认浅色模式，附带深色模式 |
| 深色优先 | 默认深色模式，附带浅色模式 |
| 双模式并重 | 浅色/深色同等权重，均可作为默认 |

**用户说"随便"**：默认使用品牌原厂色 + 浅色优先。

#### 第3步确认：目标设备与适配范围（必问）

> **必须使用 AskUserQuestion 工具向用户提问。**

提问内容："请选择目标设备与适配范围："

| 选项 | 说明 |
|------|------|
| 仅手机 | 375-428dp，竖屏布局，触屏交互 |
| 手机+折叠屏 | 375-840dp，含折叠屏展开态适配 |
| 手机+平板 | 375-1280dp，含平板横竖屏布局 |
| 全端适配 | 375dp+，手机/折叠屏/平板/桌面全覆盖 |
| 仅桌面 | 1280dp+，键鼠交互，多列布局 |
| 仅小程序 | 375dp，微信小程序容器约束 |

**用户说"都可以"/"无所谓"**：默认"仅手机"。

#### 三步确认完成后的行为

确认完成后，锁定用户选择，整个会话内严格执行：
1. **风格锁定**：所有输出严格遵循用户选定的风格规范
2. **配色锁定**：使用用户选定的配色方向生成 Design Token
3. **设备锁定**：布局断点以用户选定的设备范围为基准

然后进入八步工作流的 Step 1（需求分析），继续执行。

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

### 1.7 图标拟真规则

Demo 与原型中的「功能入口网格 / 应用图标」必须使用**拟真原生系统应用图标**，禁止用字母、emoji 或纯色块占位。具体要求：

- 图标字形使用内联 SVG 绘制真实感的系统 App 图标（相机、照片、地图、天气、联系人、时钟、备忘录、计算器、设置等），完整 SVG 规范见 `references/components/app-icons.md`
- 真实渐变背景由图标容器提供（如 iOS 相机为深灰 `#54545A→#2C2C2E`、照片为白底、时钟为纯黑、备忘录为黄色、设置为灰色），**不得**套用平台主色统一染色——系统 App 图标有独立视觉身份
- 图标圆角随平台规范：iOS squircle≈12px、Android 16-20dp、One UI/HarmonyOS/OriginOS 16dp、Flyme 8px、Windows 4px、小程序 8px；容器需 `overflow:hidden` 以裁剪 SVG 方角
- 深色模式下背景与字形按平台规范微调，保持可识别（如时钟黑底在深色模式可降对比为深灰描边）

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

### 大厂品牌风格路由

当用户选择"大厂品牌风格"维度时，从品牌注册表匹配品牌并获取设计规范：

| 品牌Slug | 中文名 | 触发关键词 | 规范文件路径 | 核心特征 | 获取方式 |
|----------|--------|-----------|-------------|---------|---------|
| tencent | 腾讯 | 腾讯, 腾讯风格, QQ, 微信风格 | references/brands/tencent.md | 社交绿洲·连接万物·生态织网 | npx getdesign@latest add tencent |
| alibaba | 阿里巴巴 | 阿里, 阿里巴巴, 淘宝, 天猫 | references/brands/alibaba.md | 商业橙光·让天下没有难做的生意 | npx getdesign@latest add alibaba |
| bytedance | 字节跳动 | 字节, 字节跳动, 抖音, TikTok | references/brands/bytedance.md | 算法彩虹·内容宇宙·激发创造 | npx getdesign@latest add bytedance |
| xiaohongshu | 小红书 | 小红书, 种草, 红书 | references/brands/xiaohongshu.md | 种草红·标记生活·消费决策 | npx getdesign@latest add xiaohongshu |
| deepseek | DeepSeek | DeepSeek, 深度求索 | references/brands/deepseek.md | 深度蓝紫·开源先锋·推理之光 | npx getdesign@latest add deepseek |
| stripe | Stripe | Stripe, 支付, Stripe风格 | references/brands/stripe.md | 紫色优雅·金融数据·weight-300 | npx getdesign@latest add stripe |
| vercel | Vercel | Vercel, 部署, Vercel风格 | references/brands/vercel.md | 黑白精准·Geist字体·零配置部署 | npx getdesign@latest add vercel |
| apple | Apple | Apple, 苹果, 苹果风格 | references/brands/apple.md | 极简留白·像素完美·设计即哲学 | npx getdesign@latest add apple |
| tesla | Tesla | Tesla, 特斯拉, Tesla风格 | references/brands/tesla.md | 减法极致·电影摄影·电动革命 | npx getdesign@latest add tesla |
| feishu | 飞书 | 飞书, 协作, 飞书风格 | references/brands/feishu.md | 协作紫·先进协作·高效愉悦 | npx getdesign@latest add feishu |

（完整国内80+国外20品牌路由见 references/brands/registry.md）

**品牌路由规则：**
- 用户输入含品牌名称时，先在品牌注册表（references/brands/registry.md）中查找匹配的slug，然后加载对应品牌设计规范文件（references/brands/{slug}.md）
- 匹配成功后，执行 `npx getdesign@latest add <slug>` 获取 DESIGN.md 规范
- 获取失败时，降级使用品牌注册表中的一句话风格描述作为参考
- 多品牌混搭时，以第一个品牌为主品牌，其余品牌提取指定维度融合
- 品牌示例：腾讯/阿里/字节/小红书/DeepSeek/Stripe/Vercel/Apple/Tesla/飞书

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

当用户选择大厂品牌风格时，Step 3 的执行方式变更：
1. 执行 `npx getdesign@latest add <slug>` 获取 DESIGN.md
2. 从 DESIGN.md 解析6大维度：颜色系统、字体规范、组件样式、间距系统、圆角体系、阴影系统
3. 将品牌DESIGN.md的Token映射为CSS自定义属性格式
4. 严格使用品牌规范中的精确数值（如 rgba(0,0,0,0.95) 不用 #000000，-2.125px 不四舍五入），禁止近似替代
5. 当品牌风格与平台类型混搭时，以平台类型为基底，品牌风格覆盖配色/排版/组件维度

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

#### 7.1 输出格式选择（必须询问用户）

在输出交付包前，必须使用 `AskUserQuestion` 询问用户期望的输出格式：

**可选输出格式：**

| 格式 | 说明 | 适用场景 |
|------|------|---------|
| **HTML原型** | 单文件可交互高保真原型，含双主题+响应式 | 快速预览、开发参考、产品演示 |
| **Figma设计稿** | 生成Figma Plugin API脚本，可导入Figma | 专业设计协作、设计团队交付 |
| **MasterGo设计稿** | 生成MasterGo插件脚本，可导入MasterGo | 国内设计团队、国产设计工具 |
| **即时设计 JsDesign** | 生成JsDesign插件脚本，可导入即时设计 | 国内设计团队、在线设计工具 |
| **墨刀 MockingBot** | 生成墨刀可导入的交互原型格式 | 快速原型、产品经理协作 |
| **蓝湖 Lanhu** | 生成蓝湖可导入的设计标注格式 | 设计交付开发、设计标注 |
| **Pixso设计稿** | 生成Pixso插件脚本，可导入Pixso | 国内设计团队、国产设计工具 |
| **设计规范文档** | 纯Markdown文档（Design Token + 组件规范） | 文档归档、规范传递、无工具场景 |

**选择逻辑：**
- 用户已明确指定格式 → 直接使用指定格式
- 用户未指定 → 展示上述8种选项供选择，默认推荐 HTML原型
- 用户选择多种格式 → 按优先级依次输出

#### 7.2 交付物内容

无论选择哪种输出格式，交付包均包含：

| 交付物 | 格式 | 说明 |
|--------|------|------|
| 设计规范文档 | Markdown | 完整Design Token + 组件规范 + 页面规范 |
| 组件库 | HTML/CSS | 可复用的组件代码片段 |
| 页面原型/设计稿 | 取决于7.1选择 | 高保真可交互原型或设计平台文件 |
| 前端样式参考 | CSS/SCSS | Design Token CSS变量 + 组件样式类 |

#### 7.3 各输出格式的具体要求

**HTML原型：**
- 单文件HTML，可直接浏览器打开
- 含浅色/深色主题切换
- 含响应式断点适配
- 含可交互组件演示

**Figma设计稿：**
- 生成Figma Plugin API代码（JavaScript），用户可在Figma中运行Plugins > Development > 插件名称 粘贴执行
- 包含Frame结构：375dp手机端/768dp平板端/1280dp桌面端
- 每个组件生成独立的Frame，命名遵循 `Component/类型/状态` 格式
- 使用Figma Auto Layout实现响应式
- 颜色使用Figma Variables定义
- 文字样式使用Figma Text Styles定义
- 包含浅色/深色两套Page

**MasterGo设计稿：**
- 生成MasterGo Plugin API代码，用户可在MasterGo中运行插件粘贴执行
- 输出格式与Figma类似，使用MasterGo API适配
- 支持MasterGo的组件变体（Variant）功能
- 支持MasterGo的自动布局

**即时设计 JsDesign：**
- 生成JsDesign Plugin API代码，用户可在即时设计中运行插件粘贴执行
- 支持JsDesign的响应式布局
- 支持JsDesign的组件状态管理

**墨刀 MockingBot：**
- 生成HTML格式原型，可通过墨刀的"导入HTML"功能导入
- 包含页面链接和交互热点标注
- 适合产品经理快速创建可点击原型

**蓝湖 Lanhu：**
- 生成设计标注格式的JSON + CSS变量文件
- 包含尺寸标注、间距标注、色值标注
- 可通过蓝湖的"上传设计稿"功能导入

**Pixso设计稿：**
- 生成Pixso Plugin API代码，用户可在Pixso中运行插件粘贴执行
- 输出格式与Figma API高度兼容
- 支持Pixso的组件库和设计令牌

### Step 8: Demo生成

为每个风格生成独立的可运行HTML Demo页面：
- 存放路径: `demo/{style-name}/index.html`
- 必须是单文件HTML，可直接浏览器打开
- 必须包含浅色/深色主题切换
- 必须展示该风格的核心组件和视觉特征
- 手机端Demo默认375dp视口，Windows端Demo默认1280dp视口，小程序Demo默认375dp视口
- 功能入口网格必须使用拟真原生应用图标（相机/照片/地图/天气/联系人/时钟/备忘录/计算器/设置），禁止字母或 emoji 占位，图标 SVG 规范见 `references/components/app-icons.md`
- 每个 Demo 的弹窗（Dialog/Alert）**必须包含右上角独立 X 关闭按钮**，并支持点击遮罩关闭与 `Esc` 键关闭、打开时自动聚焦关闭按钮（硬规范见 `references/components/feedback.md` 第 2.5 节，禁止仅用"取消/确认"按钮关闭）
- 每个 Demo 应额外演示高保真交互组件：动作面板(Action Sheet)、菜单(Menu)、分段控件(Segmented)、滑块(Slider)、步进器(Stepper)、提示气泡(Tooltip)、实时搜索(Live Search)，具体清单见 `references/components/feedback.md` 第 2.6 节

当用户选择大厂品牌风格时，Demo 的额外要求：
- Demo 顶部必须标注品牌来源（如 "Designed with Apple Design Language"）
- 品牌色必须作为CSS变量 --brand-primary 使用，禁止硬编码
- 品牌字体必须声明开源替代字体（如 SF Pro → Inter, Apple SD Gothic Neo → Noto Sans SC）
- 品牌设计中的 Do's and Don'ts 必须在 Demo 中体现

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

### 4.1b 品牌风格规范

| 文件路径 | 用途 | 加载时机 |
|----------|------|---------|
| references/brands/registry.md | 国内80+国外20品牌注册表（slug+中英文名+风格描述+主色+获取方式） | Step 2，用户选择大厂品牌风格时加载 |
| references/brands/{slug}.md | 各品牌独立设计规范文件（9大章节完整约束） | Step 3，生成品牌Design Token时加载 |
| /tmp/design-md-tmp/DESIGN.md | 运行时获取的品牌设计规范（npx getdesign@latest add <slug>） | Step 3，生成品牌Design Token时加载 |

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
| references/components/app-icons.md | 拟真原生应用图标库（9 个系统 App 图标 SVG 规范） | Step 8，生成 Demo 功能网格时加载 |

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
1. 平台判定: 微信小程序 -> 路由匹配WeUI -> 加载 `references/styles/wechat-miniprogram.md`
2. 确认: 主色方向(品牌绿)、WeUI组件范围
3. 生成Design Token: WeUI色彩、字体、4px基准间距
4. 输出组件: WeUI风格商品列表、购物车栏、分类标签、下单按钮
5. 生成原型: 单HTML文件，375dp视口，模拟小程序容器
6. 审查: 对照WeUI规范检查还原度
7. 交付: 完整设计规范 + 组件库 + 可交互原型
8. Demo: 生成 `demo/wechat-miniprogram/index.html`

### 示例4: 小红书风格美妆种草社区

用户输入: "用小红书风格设计一个美妆种草社区首页"

执行流程:
1. 风格判定: 大厂品牌风格 -> 路由匹配小红书 -> 加载 `references/brands/registry.md` 中xiaohongshu条目
2. 获取设计规范: 执行 `npx getdesign@latest add xiaohongshu` 获取DESIGN.md，解析种草红#FF2442配色、瀑布流双列布局、笔记卡片样式
3. 生成Design Token: 小红书品牌色、圆角图片排版、双列瀑布流网格
4. 输出组件: 瀑布流笔记卡片(图片+标题+用户头像+点赞数)、红色发布按钮、搜索框、分类标签
5. 生成原型: 单HTML文件，375dp视口，双列瀑布流布局，浅/深色切换
6. 审查: 对照小红书视觉风格检查还原度
7. 交付: 完整设计规范 + 组件库 + 可交互原型
8. Demo: 生成 `demo/brand-xiaohongshu/index.html`

### 示例5: Stripe风格支付确认页

用户输入: "用Stripe风格设计一个支付确认页面"

执行流程:
1. 风格判定: 大厂品牌风格 -> 路由匹配Stripe -> 加载 `references/brands/registry.md` 中stripe条目
2. 获取设计规范: 执行 `npx getdesign@latest add stripe` 获取DESIGN.md，解析紫色优雅#635BFF、weight-300轻量排版、金融数据表格样式
3. 生成Design Token: Stripe紫色渐变、Inter字体weight-300、精确到小数的间距
4. 输出组件: 支付信息卡片、金额展示、确认按钮(紫色渐变)、安全徽章
5. 生成原型: 单HTML文件，金融级精准排版，浅/深色切换
6. 审查: 对照Stripe设计语言检查还原度
7. 交付: 完整设计规范 + 组件库 + 可交互原型
8. Demo: 生成 `demo/brand-stripe/index.html`

### 示例6: iOS平台风格+飞书品牌风格混搭团队协作App

用户输入: "用iOS平台风格+飞书品牌风格混搭设计一个团队协作App"

执行流程:
1. 风格判定: 平台+品牌混搭 -> 平台基底iOS + 品牌风格飞书
2. 加载双规范: `references/styles/apple-ios.md`(平台基底) + `npx getdesign@latest add feishu`(品牌风格)
3. 混搭规则: iOS提供布局系统(4pt网格/毛玻璃导航/圆角卡片) + 飞书提供配色方案(协作紫#7B67EE)和组件风格(频道列表/消息气泡)
4. 生成Design Token: iOS布局+飞书配色混合Token
5. 输出组件: iOS风格导航栏+飞书紫色频道列表+混合消息气泡
6. 生成原型: 代码注释标注每个元素的来源平台/品牌
7. 交付: 混搭设计方案 + 双来源Token文档
8. Demo: 生成混合风格原型

---
