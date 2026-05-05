# modern-agile-delivery（Cursor Agent Skill）

面向 Cursor 的 **Agent Skill**：在单次主会话中按阶段 0～5 推进现代敏捷交付，带产品 / BA / 架构师 / PM / 开发 / QA（及可选 UI）视角与协同输出格式。

## 仓库

- **GitHub（改名后的规范地址）**：https://github.com/pogy/modern-agile-delivery-cursor-skill  
- **SSH clone**：`git clone git@github.com:pogy/modern-agile-delivery-cursor-skill.git`

在 GitHub 仓库 **Settings → General → Repository name** 中，将 `skill_share` 改为 `modern-agile-delivery-cursor-skill` 后，上述链接与 Remote rule 地址即可对外使用。改名后在本机执行：

`git remote set-url origin git@github.com:pogy/modern-agile-delivery-cursor-skill.git`

## 检查结论（发布前）

- `name` 与目录名一致：`modern-agile-delivery`
- 已含 YAML：`name`、`description`、`disable-model-invocation: true`、`license`
- 安装路径符合 [Cursor Skills 文档](https://cursor.com/docs/skills) 中的 `.cursor/skills/<skill>/SKILL.md`

## 在 Cursor 里使用

### 方式 A：从 GitHub 导入（推荐）

1. 本仓库已为 **公开** GitHub 仓库（见上文「仓库」链接）。
2. Cursor：**Settings → Rules → Add rule → Remote rule (GitHub)**，填入 `https://github.com/pogy/modern-agile-delivery-cursor-skill`。  
   （说明见官方文档 *Installing skills from GitHub*。）

### 方式 B：克隆到本机 skills 目录

将本仓库中的 `.cursor/skills/modern-agile-delivery` 整个文件夹复制到：

- 全局：`~/.cursor/skills/modern-agile-delivery/`，或  
- 项目内：`<你的项目>/.cursor/skills/modern-agile-delivery/`

重启或重新打开 Cursor 后，在 Agent 对话中输入 `/` 搜索 `modern-agile-delivery` 即可手动唤起（本 skill 默认 `disable-model-invocation: true`）。

## 开放标准

本仓库布局遵循 [Agent Skills](https://agentskills.io/) 所描述的「目录 + `SKILL.md`」形态，便于在其他兼容客户端中参考使用。

## 许可证

MIT（见 `LICENSE`）。**请在发布前将 `LICENSE` 中的版权行改为你自己的姓名或组织**，避免权属不清。
