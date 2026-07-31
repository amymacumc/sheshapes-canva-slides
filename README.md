# SheShapes AI Canva Slide Generator

这是一套可分享的 Canva 幻灯片生成规范。其他人可以用两种方式使用：

## 方式一：直接复制提示词

打开 [`PROMPT_TEMPLATE.md`](PROMPT_TEMPLATE.md)，填写方括号中的内容，并把完整提示词交给支持生成 PPT/Canva 的 AI 工具。

同时附上：

- 内容文件或文本；
- 自己的照片、数据和链接；
- 如需自定义品牌，附上 Logo 与色板。

## 方式二：安装为 Codex Skill

把整个目录：

`skill/sheshapes-canva-slides`

复制到 Codex 的 skills 目录，然后在任务中使用：

```text
Use $sheshapes-canva-slides to turn my content into a Canva presentation.
```

Skill 内已经包含：

- SheShapes 白色和 Bright Purple Logo；
- 9 套 16:9 SVG 渐变背景；
- 44 个角色、图标、装饰和演示组件；
- 一份可编辑 PPTX 视觉参考；
- 内容输入规范、页面模式和 QA 工作流。

## Canva 使用

如果 Codex 已连接 Canva，请在指令中提供目标文件夹链接或文件夹 ID。生成完成后，Skill 会先验证本地 PPTX，再导入 Canva，并把可复用素材单独上传到目标文件夹。

如果没有连接 Canva，仍会生成可导入 Canva 的 PPTX 和 SVG 素材文件夹。

不要为了上传而把私人文件发布到公共临时链接。

## 文件

- `PROMPT_TEMPLATE.md`：无需安装的完整提示词。
- `CONTENT_BRIEF_TEMPLATE.md`：可重复填写的内容需求表。
- `examples/`：中文、英文和自定义品牌示例。
- `skill/sheshapes-canva-slides/`：可安装 Skill。

