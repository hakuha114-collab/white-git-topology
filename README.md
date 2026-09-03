# white-git-topology

Git 拉取后「影响面 + 拓扑图」一键分析 skill（v1.0.0）。

> 触发：用户说 "git 影响拓扑" / "git-impact-topology" / "拉取后影响范围" / "生成变更拓扑图" 时，
> 一键串联 变更检测 -> 影响半径 -> 受影响流程 -> 拓扑图（D3 力导向）。
> 基于已接入的 code-review-graph MCP 图谱，输出 影响面摘要 + 拓扑图 + 高危点清单。
> 不执行任何 git 命令，pull 由用户在其环境完成。

## 安装
将本仓库内容复制到技能目录：
- WorkBuddy：`~/.workbuddy/skills/white-git-topology/`
- Codex：`~/.agents/skills/white-git-topology/` 或 `~/.codex/skills/white-git-topology/`

## 红线
本 skill 不执行任何 git 命令。pull 由用户在其开发环境完成。检测基于用户提供的 pull 前基准 SHA（BASE）。

详见 [SKILL.md](SKILL.md)。
