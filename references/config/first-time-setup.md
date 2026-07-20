> @author aitool.plus

# 首次使用设置

## 首次使用检测逻辑

### 检测条件

1. 检查工作目录下是否存在 `EXTEND.md` 文件
2. 若不存在，判定为首次使用
3. 若存在但内容为空或格式异常，判定为需要重新设置
4. 若存在且格式正确，跳过设置向导

### 检测代码示例

```javascript
function checkFirstTimeUse() {
  const fs = require('fs');
  const path = require('path');
  
  const extendPath = path.join(process.cwd(), 'EXTEND.md');
  
  try {
    const content = fs.readFileSync(extendPath, 'utf-8');
    if (!content || content.trim().length === 0) {
      return true; // 需要首次设置
    }
    // 检查是否包含必要的配置项
    const hasRequiredFields = content.includes('默认OS风格') && 
                               content.includes('默认主题');
    return !hasRequiredFields; // 缺少必要字段则需要重新设置
  } catch (error) {
    return true; // 文件不存在，需要首次设置
  }
}
```

---

## 设置向导流程

### 第一步：选择默认OS风格

**提示语**：请选择您最常用的操作系统设计风格：

**选项**：

1. Apple iOS（默认）
2. Google Android Material
3. Samsung One UI
4. 华为 HarmonyOS
5. 小米 HyperOS
6. 荣耀 MagicOS
7. OPPO ColorOS
8. vivo OriginOS
9. 魅族 Flyme
10. Windows 11 Fluent
11. 微信小程序 WeUI

**操作**：输入数字 1-11 选择，直接回车使用默认选项

**保存字段**：`default_os`

---

### 第二步：选择主题偏好

**提示语**：请选择您的默认主题模式：

**选项**：

1. 跟随系统（默认）
2. 浅色模式
3. 深色模式

**操作**：输入数字 1-3 选择，直接回车使用默认选项

**保存字段**：`default_theme`

---

### 第三步：选择输出格式

**提示语**：请选择您默认的输出格式：

**选项**：

1. HTML原型（默认）- 可直接在浏览器中打开预览
2. Markdown文档 - 设计规范文档
3. CSS代码 - 可直接使用的样式代码
4. Figma标注 - 可直接复制到Figma的标注参数

**操作**：输入数字 1-4 选择，直接回车使用默认选项

**保存字段**：`default_output_format`

---

### 设置完成

**提示语**：设置完成！您的偏好已保存到 EXTEND.md 文件中。您可以随时修改该文件来调整偏好设置。

**操作**：自动生成 EXTEND.md 文件

---

## EXTEND.md 文件创建指引

### 文件位置

```
{project-root}/EXTEND.md
```

### 文件内容模板

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

### 创建步骤

1. 在项目根目录下创建 `EXTEND.md` 文件
2. 复制上述模板内容到文件中
3. 根据用户选择修改对应的配置项
4. 保存文件

### 修改方法

#### 手动修改

直接编辑 `EXTEND.md` 文件，修改对应配置项的值。

#### 命令行修改

```bash
# 修改默认OS风格
sed -i 's/apple-ios/google-android/' EXTEND.md

# 修改默认主题
sed -i 's/auto/light/' EXTEND.md

# 修改默认输出格式
sed -i 's/html/markdown/' EXTEND.md
```

#### 脚本修改

```javascript
const fs = require('fs');

function updatePreference(key, value) {
  const path = './EXTEND.md';
  let content = fs.readFileSync(path, 'utf-8');
  
  // 根据key定位并替换值
  const patterns = {
    'default_os': /当前设置.*apple-ios/,
    'default_theme': /当前设置.*auto/,
    'default_output_format': /当前设置.*html/
  };
  
  if (patterns[key]) {
    content = content.replace(patterns[key], `当前设置：${value}`);
    fs.writeFileSync(path, content);
  }
}

// 使用示例
updatePreference('default_os', 'google-android');
```

---

## 常见问题FAQ

### Q1：如何修改已设置的偏好？

**A**：直接编辑项目根目录下的 `EXTEND.md` 文件，修改对应的配置项即可。修改后下次使用时自动生效。

### Q2：可以设置多个默认OS风格吗？

**A**：`default_os` 字段只支持单选。如需对比多个OS风格，可以在使用时通过参数指定多个OS。

### Q3：品牌色如何设置？

**A**：在 `EXTEND.md` 文件中找到品牌色配置项，将 `null` 替换为Hex色值（例如 `#007AFF`）。设置后所有使用该OS风格的设计都会自动应用此品牌色。

### Q4：动效级别如何理解？

**A**：

- `full`：完整动效，包含所有入场、离场、状态切换动画
- `reduced`：精简动效，保留关键动画，去除装饰性动画
- `minimal`：最小化动效，仅保留必要的反馈动画
- `none`：无动效，所有动画效果关闭

### Q5：自定义OS参数覆盖如何使用？

**A**：在 `custom_os_overrides` 中，以OS名称为键，以需要覆盖的参数对象作为值。例如：

```json
{
  "apple-ios": {
    "color-primary": "#FF0000",
    "border-radius": "8px"
  }
}
```

### Q6：常用组件偏好列表有什么作用？

**A**：设置常用组件偏好后，在创建设计时会优先展示这些组件，提高设计效率。可以添加任意组件名称到列表中。

### Q7：EXTEND.md 文件丢失了怎么办？

**A**：删除或丢失后，下次使用时会重新触发首次使用检测，并引导您重新设置。也可以手动创建该文件并填入默认配置。

### Q8：不同项目可以使用不同的偏好设置吗？

**A**：可以。每个项目的 `EXTEND.md` 文件是独立的，不同项目可以设置不同的偏好。

### Q9：如何恢复默认设置？

**A**：删除 `EXTEND.md` 文件，下次使用时会重新触发首次使用设置向导。或者直接编辑文件将所有配置恢复为默认值。

### Q10：设置后为什么没有立即生效？

**A**：部分设置需要重新启动或刷新才能生效。如果修改后未生效，请尝试重新加载项目或重启应用。
