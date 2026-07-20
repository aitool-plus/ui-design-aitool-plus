> @author aitool.plus

# EXTEND.md 偏好 Schema

## Schema 定义

### default_os

- **类型**：string
- **可选值**：
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
- **默认值**：`apple-ios`
- **说明**：设置默认的OS风格偏好

### default_theme

- **类型**：string
- **可选值**：
  - `light`：浅色主题
  - `dark`：深色主题
  - `auto`：跟随系统
- **默认值**：`auto`
- **说明**：设置默认的主题模式

### default_adaptation

- **类型**：string
- **可选值**：
  - `phone`：仅手机
  - `foldable`：手机+折叠屏
  - `tablet`：平板
  - `desktop`：桌面端
  - `miniprogram`：小程序
- **默认值**：`phone`
- **说明**：设置默认的适配形态

### default_output_format

- **类型**：string
- **可选值**：
  - `html`：HTML原型
  - `markdown`：Markdown文档
  - `css`：CSS代码
  - `figma`：Figma标注
- **默认值**：`html`
- **说明**：设置默认的输出格式

### brand_color

- **类型**：string | null
- **格式**：Hex 色值（例如 `#007AFF`）
- **默认值**：`null`
- **说明**：自定义品牌色，覆盖OS默认主色

### motion_level

- **类型**：string
- **可选值**：
  - `full`：完整动效
  - `reduced`：精简动效
  - `minimal`：最小化动效
  - `none`：无动效
- **默认值**：`full`
- **说明**：设置默认的动效级别

### custom_os_overrides

- **类型**：object
- **默认值**：`{}`
- **说明**：自定义OS参数覆盖，用于覆盖特定OS的默认参数
- **示例**：

```json
{
  "apple-ios": {
    "color-primary": "#FF0000",
    "border-radius": "8px"
  }
}
```

### preferred_components

- **类型**：array
- **默认值**：`[]`
- **说明**：常用组件偏好列表，用于快速选择常用组件
- **示例**：

```json
[
  "button",
  "input",
  "card",
  "list",
  "modal"
]
```

---

## EXTEND.md 文件格式示例

```markdown
# EXTEND.md

## 用户偏好设置

### 默认OS风格

- **当前设置**：apple-ios
- **说明**：使用 Apple iOS 风格作为默认设计系统

### 默认主题

- **当前设置**：auto
- **说明**：跟随系统自动切换浅色/深色模式

### 默认适配形态

- **当前设置**：phone
- **说明**：默认适配手机端

### 默认输出格式

- **当前设置**：html
- **说明**：默认输出高保真HTML原型

### 品牌色

- **当前设置**：null
- **说明**：使用OS默认主色

### 动效级别

- **当前设置**：full
- **说明**：使用完整动效

### 自定义OS参数覆盖

- **当前设置**：{}
- **说明**：无自定义覆盖

### 常用组件偏好

- **当前设置**：[]
- **说明**：无预设常用组件
```

---

## JSON 格式示例

```json
{
  "default_os": "apple-ios",
  "default_theme": "auto",
  "default_adaptation": "phone",
  "default_output_format": "html",
  "brand_color": null,
  "motion_level": "full",
  "custom_os_overrides": {},
  "preferred_components": []
}
```
