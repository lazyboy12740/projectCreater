---
name: my-rules
description: 个人规则集：每次 AI 问答时遵守的行为规范，由 AGENTS.md 自动调用加载
---

# My Rules

以下规则在每次 AI 问答时生效，所有操作必须遵守。

---

## GitHub 操作规则

任何涉及 GitHub 的操作，**在执行前必须先使用 `ask` 工具向用户确认**，得到明确同意后方可执行。

GitHub 操作包括但不限于：
- 创建/删除仓库
- 推送代码 (`git push`)
- 创建/合并 Pull Request
- 创建 Release / Tag
- 修改远程仓库配置 (`git remote`)
- 任何通过 `gh` CLI 执行的操作
- 任何通过 GitHub API 执行的操作

可以展示计划执行的操作和命令，但不能在未经确认的情况下静默执行。

---

## 工程化原则

**所有配置和工具尽量在项目内实现，不依赖项目外的环境。**

具体而言：
- 配置文件（lint、format、type-check、build 等）放在项目目录内，不依赖全局配置
- 工具依赖通过项目自身的包管理器管理（`package.json` / `pyproject.toml` / `go.mod` 等），避免要求全局安装 CLI 工具
- CI/CD 配置包含在项目内（`.github/workflows/`、`.gitlab-ci.yml` 等）
- 环境变量通过 `.env.example` 或项目内配置模板提供，不依赖外部注入
- 脚本命令（`dev`、`build`、`test`、`lint`）定义在项目配置文件中，统一入口

---

## 规则追加指南

如需添加新规则，在下方按分类追加即可：

### 示例：代码规范
<!-- 待补充 -->

### 示例：文件操作
<!-- 待补充 -->

### 示例：回答风格
<!-- 待补充 -->
