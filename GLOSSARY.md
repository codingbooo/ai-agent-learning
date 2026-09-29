# Glossary (AI Principles, Harness & Agent)

## Core Concepts

- **Token（词元）**：大模型处理文本的基本物理单元。英文中约 1 个单词 = 1.3 个 Token，中文中通常 1 个汉字 = 1~2 个 Token。
- **Next-Token Prediction（下一词元预测）**：自回归语言模型的核心生成机制。模型不“思考”全篇，而是基于给定上文，以概率分布预测下一个最可能的 Token。
- **Context Window（上下文窗口）**：模型单次推理能“看见”的最大 Token 序列长度。相当于处理器的片上工作缓存（RAM/Cache）。
- **Temperature（采样温度）**：控制预测概率分布平滑度的超参数。温度趋近 0 时行为最确定（贪心选择最大概率），温度升高时增加多样性与发散性。
- **Harness（装具/测试台架）**：包裹在大模型外部的宿主运行时或测试框架，负责输入预处理、提示词封装、工具调用拦截与安全沙盒隔离。
- **Agent（智能体）**：由大模型驱动的自治决策状态机，具备推导（Reasoning）、工具使用（Tools/Actuators）、感知观察（Observation）和反思修正能力。
- **ReAct（Reason + Act）**：Agent 的经典循环模式：根据目标推导思考（Thought） -> 做出决策并调用工具（Action） -> 获取物理环境反馈（Observation）并循环。
