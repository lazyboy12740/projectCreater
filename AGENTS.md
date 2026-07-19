# AGENTS

## 会话启动规则

在每次对话开始时，**必须先加载我的个人规则**：

```
/my-rules
```

或通过 `run_skill({ name: "my-rules" })` 调用。

如果 `my-rules` skill 不可用，请提醒我配置该 skill。

---

## 迁移说明

将此文件连同 `.reasonix/skills/my-rules/` 目录复制到新项目，即可在新项目中自动应用相同规则。
