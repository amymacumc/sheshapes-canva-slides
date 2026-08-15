# SheShapes AI Slide Generator

这是一套面向 SheShapes AI 社群的可复用幻灯片设计系统和 Codex Skill，支持两种正式产出：

| 产出方式 | 适用场景 | 前置条件 |
| --- | --- | --- |
| 可编辑 `.pptx` | PowerPoint 演示、归档、交付给他人继续编辑，或手动导入 Canva | 无需 Canva Plugin |
| Canva Presentation | 在线共创、评论、复制模板、归档到 Canva 文件夹 | 在 Codex 中安装并授权 Canva Plugin |

本设计系统最初为 **SheShapes AI 2026** 建立，供组委、项目组、课程组、影响力运营组和学员制作活动、课程、项目与社群材料。未来如有新的 SheShapes AI 延续项目，也欢迎继续复用、组合和扩展这些设计元素。

## 背景：How was this design born?

工作流：
```text
需求或内容
  → 请 ChatGPT 整理成 Codex 可执行的 Markdown brief
  → Codex 读取 brief 与品牌素材
  → 生成可编辑 PPTX
  → 逐页渲染与 QA
  → 可选：通过 Canva Plugin 导入 Canva
  → 团队继续共创
```
该工作流可复用在其他场景的ppt设计。
如果一开始只有零散想法，可以先让 ChatGPT 按 [`CONTENT_BRIEF_TEMPLATE.md`](CONTENT_BRIEF_TEMPLATE.md) 生成一个 `.md` 文件，再将该文件交给 Codex。建议 brief 至少包含：目标、受众、页数、页面结构、已有内容、待补占位、品牌要求、输出格式和 Canva 目标文件夹。

## 使用方式一：直接复制提示词

打开 [`PROMPT_TEMPLATE.md`](PROMPT_TEMPLATE.md)，填写方括号中的内容，并把完整提示词交给支持生成 PPT/Canva 的 AI 工具。

同时附上：

- 内容文件或文本；
- 自己的照片、数据和链接；
- 如需自定义品牌，附上 Logo 与色板。

## 使用方式二：安装为 Codex Skill

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

## 产出 PPTX

无需安装 Canva Plugin。示例指令：

```text
Use $sheshapes-canva-slides to turn this Markdown brief into an editable 16:9 PPTX.
Render and QA every slide, then return the versioned PPTX source file.
```

PPTX 路径是默认且最稳定的交付方式。文字、卡片、线条和大部分版式元素应保持可编辑；渐变背景、插画和 Logo 可以作为 SVG/PNG 素材嵌入。

## 产出 Canva Presentation

Canva 产出需要先在 Codex 的 **Plugins** 中安装 **Canva Plugin**，登录并授权目标 Canva 账号。安装完成后，在指令中提供目标文件夹链接或文件夹 ID：

```text
Use $sheshapes-canva-slides to create an editable PPTX from this brief,
QA every page, import it as a Canva Presentation, and move it to this folder:
[Canva folder URL or folder ID]
```

Skill 会先生成并验证本地 PPTX，再通过 Canva Plugin 导入为 Canva Presentation；需要长期复用的 SVG、PNG 和 Logo 素材可以单独上传到目标文件夹。

如果 Canva Plugin 未安装、未授权或暂时不可用，Skill 应回退为交付可手动导入 Canva 的 PPTX 与素材文件夹，而不是停止整个任务。

不要为了上传而把私人文件发布到公共临时链接。

## 复用与署名

- SheShapes AI 2026 组委和学员可按项目需要自由复用、复制页面、替换内容和重新组合素材。
- 后续 SheShapes AI 活动、课程、Fellow 项目和社群延续项目欢迎继续使用。
- 建议在对外分享或二次发布时保留来源说明：`Built with the SheShapes AI Slide System`。
- 修改内容时应继续遵循包容、温暖、人本和轻科技的视觉原则，并使用正确的 Logo 版本。
- 这是一份社群复用声明，不替代正式的法律许可证；如需对外商业授权或转售素材，请先与 SheShapes AI 确认。

## 质量与限制

- 每页必须包含 SheShapes Logo：深色页面用白色 Logo，浅色页面用 `#C33EE3`。
- 输出必须版本化，例如 `v0.1`、`v0.2`，不要覆盖已经确认的文件。
- PPTX 在交付前应逐页渲染，检查溢出、裁切、对比度、页数和内容准确性。
- Canva 导入后应再次确认页数、标题、文件夹位置和关键页面。
- Canva 可能把 SVG 作为一个整体可缩放图像导入，不保证渐变节点或插画分组能够完全解组。
- 不要虚构缺失的姓名、日期、数据或引用；模板任务可以保留明确标注的占位内容。

## 文件

- `PROMPT_TEMPLATE.md`：无需安装的完整提示词。
- `CONTENT_BRIEF_TEMPLATE.md`：可重复填写的内容需求表。
- `examples/`：中文、英文和自定义品牌示例。
- `skill/sheshapes-canva-slides/`：可安装 Skill。
