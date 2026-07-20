> @author aitool.plus

# 确认门控选项

## Round1 必选确认

### 1. 目标OS风格

- 类型：单选/多选
- 选项列表：
  - `apple-ios`：Apple iOS 风格
  - `google-android`：Google Android Material 风格
  - `samsung-one-ui`：Samsung One UI 风格
  - `huawei-harmonyos`：华为 HarmonyOS 风格
  - `xiaomi-hyperos`：小米 HyperOS 风格
  - `honor-magicos`：荣耀 MagicOS 风格
  - `oppo-coloros`：OPPO ColorOS 风格
  - `vivo-originos`：vivo OriginOS 风格
  - `meizu-flyme`：魅族 Flyme 风格
  - `windows-fluent`：Windows 11 Fluent 风格
  - `wechat-miniprogram`：微信小程序 WeUI 风格
- 默认值：`apple-ios`
- 说明：选择目标操作系统风格，可多选进行多平台对比

### 2. 页面类型

- 类型：单选/多选
- 选项列表：
  - `launch`：启动页
  - `home`：首页
  - `list`：列表页
  - `detail`：详情页
  - `form`：表单页
  - `settings`：设置页
  - `profile`：个人中心
  - `search`：搜索页
  - `cart`：购物车
  - `order`：订单页
- 默认值：`home`
- 说明：选择需要设计的页面类型

### 3. 核心功能模块

- 类型：多选
- 选项列表：
  - `navigation`：导航
  - `search`：搜索
  - `list`：列表
  - `card`：卡片
  - `modal`：弹窗
  - `tab-bar`：标签栏
  - `form`：表单
  - `map`：地图
  - `chart`：图表
- 默认值：`navigation`, `list`, `card`
- 说明：选择页面中包含的核心功能模块

### 4. 目标用户群体

- 类型：多选
- 选项列表：
  - `consumer`：消费者
  - `enterprise`：企业用户
  - `teenager`：青少年
  - `senior`：中老年
  - `professional`：专业人士
- 默认值：`consumer`
- 说明：选择目标用户群体

### 5. 适配形态

- 类型：单选
- 选项列表：
  - `phone-only`：仅手机
  - `phone-foldable`：手机+折叠屏
  - `all-devices`：全端
  - `desktop-only`：桌面端
  - `miniprogram`：小程序
- 默认值：`phone-only`
- 说明：选择适配的设备形态

---

## Round2 可选确认

### 1. 品牌色定制

- 类型：单选
- 选项列表：
  - `custom-hex`：自定义 Hex 值
  - `os-default`：使用OS默认
- 默认值：`os-default`
- 说明：选择是否使用自定义品牌色

### 2. 深色模式需求

- 类型：单选
- 选项列表：
  - `light-only`：仅浅色
  - `dark-only`：仅深色
  - `dual-mode`：双模式
  - `follow-system`：跟随系统
- 默认值：`follow-system`
- 说明：选择深色模式支持策略

### 3. 动效级别

- 类型：单选
- 选项列表：
  - `full`：完整动效
  - `reduced`：精简动效
  - `minimal`：最小化动效
  - `none`：无动效
- 默认值：`full`
- 说明：选择动效丰富程度

### 4. 交付格式

- 类型：多选
- 选项列表：
  - `html`：HTML原型
  - `markdown`：Markdown文档
  - `css`：CSS代码
  - `figma`：Figma标注
- 默认值：`html`
- 说明：选择输出交付格式

---

## Review 确认

### 1. 设计系统审查

- 选项列表：
  - `pass`：通过
  - `edit`：编辑
  - `regenerate`：重新生成
- 默认值：`pass`
- 说明：对设计系统进行审查确认

### 2. 组件规范审查

- 选项列表：
  - `pass`：通过
  - `edit`：编辑
  - `regenerate`：重新生成
- 默认值：`pass`
- 说明：对组件规范进行审查确认

### 3. 页面原型审查

- 选项列表：
  - `pass`：通过
  - `edit`：编辑
  - `regenerate`：重新生成
- 默认值：`pass`
- 说明：对页面原型进行审查确认
