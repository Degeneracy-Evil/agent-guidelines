# agent-guidelines

一份面向 Codex 等编码 Agent 的通用行为准则，重点解决两类问题：不自然的防御性表达，以及把简单开发任务复杂化的工程习惯。

仓库目前只维护一个可直接使用的 [AGENTS.md](./AGENTS.md)，不依赖 Skills、子 Agent 或额外框架。

## 核心理念

- **第一性原理**：从真实需求和判断依据出发，而不是机械执行既定流程。
- **奥卡姆剃刀**：优先选择满足需求的最简单方案，不引入没有实际价值的复杂度。
- **非防御性写作**：直接交流，不说教、不自我辩解、不用冗余免责声明填充答案。

具体规则覆盖日常交流、代码修改、验证和交付。尤其不鼓励例行计算 Hash、无条件补写单元测试、为小改动执行全量验证，以及生成冗长的工作报告。

## 使用

在 Codex 中，将 [AGENTS.md](./AGENTS.md) 放到对应位置：

- **全局生效**：`~/.codex/AGENTS.md`。
- **仅当前项目生效**：项目根目录的 `AGENTS.md`。

也可以复制其中的规则到其他支持自定义指令的编码 Agent。

## 维护

通过实际使用中遇到的问题逐步调整规则。优先修改已有条目，避免不断堆叠近义禁令；不引入额外组件，除非它能解决明确存在的问题。

## 参考

- [Codex No-Fluff Prompt](https://github.com/aidenfausto/codex-no-fluff-prompt)
- [Karpathy Guidelines](https://github.com/nassimna/karpathy-guidelines)
- [Anthropic Code Simplifier](https://github.com/anthropics/claude-plugins-official/tree/main/plugins/code-simplifier)
