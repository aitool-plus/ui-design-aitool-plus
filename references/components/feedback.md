> @author aitool.plus

# 反馈组件规范

## 1. 组件概述

反馈组件用于向用户传达系统状态、操作结果或引导用户决策，涵盖弹窗/对话框、Toast/Snackbar、进度条、空状态、加载骨架屏五大核心组件。本规范确保反馈信息的及时性、清晰度与一致性。

## 2. 通用规范

### 2.1 结构描述

所有反馈组件遵循统一的结构分层：
- **触发层**：定义反馈出现的时机与条件（用户操作、系统事件、定时触发）
- **容器层**：定义反馈载体的大小、位置、层级（z-index）
- **内容层**：承载图标、文本、进度、操作按钮等核心信息
- **退出层**：定义反馈消失的机制（自动消失、用户关闭、操作完成）

### 2.2 尺寸参数

| 组件类型 | 宽度 | 高度 | 圆角 | 显示位置 |
|---------|------|------|------|---------|
| 弹窗/对话框 | 280-320dp | 自适应 | 12-24dp | 屏幕中央 |
| Toast | 自适应 | 40-56dp | 4-12dp | 屏幕底部或中央 |
| Snackbar | 自适应或全宽 | 48-56dp | 4-8dp | 屏幕底部 |
| 进度条 | 全宽或固定 | 2-8dp | 1-4dp | 顶部或嵌入 |
| 空状态 | 自适应 | 自适应 | 0-16dp | 内容区域中央 |
| 骨架屏 | 全宽 | 自适应 | 4-8dp | 内容区域 |

### 2.3 状态变体

| 状态 | 视觉表现 | 适用组件 |
|-----|---------|---------|
| 信息 | 蓝色图标/主色文本 | 弹窗、Toast、Snackbar |
| 成功 | 绿色对勾图标 | 弹窗、Toast、Snackbar、进度条 |
| 警告 | 黄色感叹号图标 | 弹窗、Toast、Snackbar |
| 错误 | 红色叉号图标 | 弹窗、Toast、Snackbar |
| 加载中 | 旋转指示器或骨架屏 | 弹窗、Toast、进度条、骨架屏 |
| 完成 | 100%进度+对勾 | 进度条 |

### 2.4 无障碍

- 弹窗/对话框必须自动聚焦到主按钮或关闭按钮，支持Esc键关闭
- Toast/Snackbar必须支持屏幕阅读器朗读，设置适当的aria-live属性（polite/assertive）
- 进度条必须提供aria-valuenow、aria-valuemin、aria-valuemax属性
- 空状态必须提供明确的操作引导，不可仅为静态提示
- 骨架屏必须设置aria-busy="true"，加载完成后通知内容变化
- 所有反馈组件的显示/消失必须有平滑过渡动画，时长200-300ms

## 3. 9大OS风格差异对比表

### 3.1 弹窗/对话框(Dialog)

| 系统 | 宽度 | 圆角 | 背景 | 按钮排列 | 标题字重 | 阴影 |
|-----|------|------|------|---------|---------|------|
| iOS | 270pt | 13pt | #FFFFFF | 垂直堆叠 | Semibold | 0 10pt 20pt rgba(0,0,0,0.15) |
| Android | 280dp | 28dp | #FFFBFE | 水平排列(右对齐) | Medium | 0 4dp 12dp rgba(0,0,0,0.12) |
| One UI | 320dp | 20dp | #FFFFFF | 水平排列(居中) | Bold | 0 4dp 16dp rgba(0,0,0,0.1) |
| HarmonyOS | 280vp | 16vp | #FFFFFF | 水平排列(右对齐) | Medium | 0 4vp 12vp rgba(0,0,0,0.1) |
| HyperOS | 300dp | 16dp | #FFFFFF | 水平排列(右对齐) | Medium | 0 4dp 12dp rgba(0,0,0,0.08) |
| MagicOS | 320dp | 16dp | #FFFFFF | 水平排列(右对齐) | Medium | 0 4dp 16dp rgba(0,0,0,0.1) |
| ColorOS | 320dp | 24dp | #FFFFFF | 水平排列(居中) | Medium | 0 4dp 16dp rgba(0,0,0,0.08) |
| OriginOS | 300dp | 20dp | #FFFFFF | 水平排列(居中) | Medium | 0 4dp 16dp rgba(0,0,0,0.1) |
| Flyme | 280dp | 12dp | #FFFFFF | 水平排列(右对齐) | Medium | 0 2dp 8dp rgba(0,0,0,0.08) |

### 3.2 Toast/Snackbar

| 系统 | 高度 | 圆角 | 背景色 | 文字色 | 显示时长 | 位置 |
|-----|------|------|--------|--------|---------|------|
| iOS | 40pt | 8pt | #000000(80%) | #FFFFFF | 2-4s | 屏幕中央偏上 |
| Android | 48dp | 4dp | #322F35 | #FFFFFF | 2-4s | 屏幕底部 |
| One UI | 48dp | 8dp | #323232 | #FFFFFF | 2-4s | 屏幕底部 |
| HarmonyOS | 48vp | 8vp | #000000(75%) | #FFFFFF | 2-4s | 屏幕中央 |
| HyperOS | 48dp | 8dp | #333333 | #FFFFFF | 2-4s | 屏幕底部 |
| MagicOS | 48dp | 8dp | #333333 | #FFFFFF | 2-4s | 屏幕底部 |
| ColorOS | 48dp | 12dp | #333333 | #FFFFFF | 2-4s | 屏幕底部 |
| OriginOS | 48dp | 8dp | #333333 | #FFFFFF | 2-4s | 屏幕底部 |
| Flyme | 40dp | 4dp | #000000(80%) | #FFFFFF | 2-4s | 屏幕中央 |

### 3.3 进度条(Progress)

| 系统 | 高度 | 圆角 | 激活色 | 未激活色 | 缓冲色 | 动画 |
|-----|------|------|--------|---------|--------|------|
| iOS | 4pt | 2pt | #007AFF | #E5E5EA | 无 | 线性匀速 |
| Android | 4dp | 2dp | #6750A4 | #E8DEF8 | #D0BCFF | 线性带缓冲动画 |
| One UI | 6dp | 3dp | #1259C3 | #E0E0E0 | #BDBDBD | 线性匀速 |
| HarmonyOS | 4vp | 2vp | #007DFF | #E5E5E5 | #D9D9D9 | 线性带缓冲动画 |
| HyperOS | 4dp | 2dp | #FF6900 | #F0F0F0 | #E0E0E0 | 线性匀速 |
| MagicOS | 6dp | 3dp | #0066FF | #E8E8E8 | #DCDEE0 | 线性匀速 |
| ColorOS | 4dp | 2dp | #1BA784 | #E6E6E6 | #D9D9D9 | 线性带缓冲动画 |
| OriginOS | 4dp | 2dp | #415FFF | #E8E8E8 | #E0E0E0 | 线性匀速 |
| Flyme | 2dp | 1dp | #00B4FF | #E0E0E0 | 无 | 线性匀速 |

### 3.4 空状态(EmptyState)

| 系统 | 插画尺寸 | 标题字号 | 描述字号 | 按钮高度 | 插画风格 |
|-----|---------|---------|---------|---------|---------|
| iOS | 160pt | 20pt Semibold | 15pt Regular | 44pt | 线性简约 |
| Android | 160dp | 20sp Medium | 14sp Regular | 40dp | 填充扁平 |
| One UI | 180dp | 20sp Bold | 14sp Regular | 48dp | 填充渐变 |
| HarmonyOS | 160vp | 20fp Medium | 14fp Regular | 48vp | 线性简约 |
| HyperOS | 160dp | 18sp Medium | 14sp Regular | 44dp | 填充扁平 |
| MagicOS | 180dp | 20sp Medium | 14sp Regular | 48dp | 填充渐变 |
| ColorOS | 180dp | 20sp Medium | 14sp Regular | 48dp | 填充扁平 |
| OriginOS | 180dp | 20sp Medium | 14sp Regular | 48dp | 线性渐变 |
| Flyme | 140dp | 18sp Medium | 14sp Regular | 40dp | 线性简约 |

### 3.5 加载骨架屏(Skeleton)

| 系统 | 脉冲周期 | 圆角 | 基础色 | 高亮色 | 行高 | 动画类型 |
|-----|---------|------|--------|--------|------|---------|
| iOS | 1.5s | 4pt | #F2F2F7 | #E5E5EA | 8pt | 渐变扫光 |
| Android | 2s | 4dp | #E8DEF8 | #D0BCFF | 8dp | 渐变扫光 |
| One UI | 1.8s | 8dp | #F5F5F5 | #E0E0E0 | 8dp | 渐变扫光 |
| HarmonyOS | 1.5s | 4vp | #F5F5F5 | #E5E5E5 | 8vp | 渐变扫光 |
| HyperOS | 1.5s | 4dp | #F8F8F8 | #F0F0F0 | 8dp | 渐变扫光 |
| MagicOS | 1.8s | 4dp | #F8F9FA | #E8E8E8 | 8dp | 渐变扫光 |
| ColorOS | 2s | 8dp | #F5F5F5 | #E6E6E6 | 8dp | 渐变扫光 |
| OriginOS | 1.5s | 8dp | #F2F3F5 | #E8E8E8 | 8dp | 渐变扫光 |
| Flyme | 1.5s | 4dp | #F5F5F5 | #E0E0E0 | 8dp | 渐变扫光 |

## 4. 设计禁忌

1. **禁止弹窗嵌套弹窗**：弹窗上不可再弹出二级弹窗，复杂流程应改用页面或底部面板
2. **禁止Toast显示超过5秒**：Toast用于轻量提示，超过5秒将干扰用户操作，长信息应使用Snackbar或弹窗
3. **禁止进度条无明确终点**：不确定进度必须使用循环加载指示器，禁止用无限延伸的进度条
4. **禁止空状态无操作引导**：空状态必须提供明确的操作按钮或引导文案，禁止仅展示"暂无数据"
5. **禁止骨架屏与真实内容混用**：骨架屏加载完成后必须整体替换为真实内容，禁止部分替换导致布局跳动
6. **禁止弹窗无遮罩层**：模态弹窗必须配合半透明遮罩层（透明度40%-60%），非模态弹窗需明确区分
7. **禁止同一时刻多个Toast堆叠**：同一时间只允许一个Toast存在，新Toast必须替换旧Toast
8. **禁止进度条高度超过8dp**：过粗的进度条将显得笨重，标准高度为4dp
9. **禁止Snackbar操作按钮过长**：Snackbar的操作按钮文本不得超过2个汉字或4个英文字母，过长应改用弹窗
10. **禁止骨架屏圆角与真实内容不一致**：骨架屏的圆角、间距必须与真实内容完全匹配，避免切换时的视觉跳动
