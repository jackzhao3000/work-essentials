# 04 多智能体与技能工作流

本目录是一张短索引。多智能体框架和入门课程体积大，完整仓库留在上游；日常要用的技能正文已经放在 `01-ppt-lecture/` 和 `02-academic-writing/` 的 `SKILL.md` 里。

来源与「为什么不镜像」见 [`SOURCE.md`](SOURCE.md)。

## 先看这门课

[AI Agents for Beginners](https://github.com/microsoft/ai-agents-for-beginners)（Microsoft，MIT）：18 节入门课，从代理概念讲到工具调用和多代理协作。适合在自己拆「调研—写作—出片」流程之前，把常见模式过一遍。仓库体积约 3.6 GB，这里只保留链接。

## 技能格式

本库收录的 PPT 与写作材料都是 Agent Skill：一个目录加一份 `SKILL.md`。

- 规范说明目前写在 [agentskills.io/specification](https://agentskills.io/specification)。2026-10-19 核对时，[anthropics/skills](https://github.com/anthropics/skills) 的 `spec/agent-skills-spec.md` 已改为指向该地址。
- [anthropics/skills](https://github.com/anthropics/skills) 是示例仓库。其中不少示例为 Apache-2.0；`skills/pptx` 等文档技能是源码可见的生产实现，许可证并不单一。需要对照 PPTX 技能写法时直接打开上游，不把整库复制进来。

## 多代理框架（只作对照）

| 项目 | 许可证 | 适合用来理解的问题 |
| --- | --- | --- |
| [microsoft/autogen](https://github.com/microsoft/autogen) | CC-BY-4.0 | 多个代理如何对话、分工 |
| [langchain-ai/langgraph](https://github.com/langchain-ai/langgraph) | MIT | 把一步调研、一次改写、一次出片收成有状态的图 |
| [crewAIInc/crewAI](https://github.com/crewAIInc/crewAI) | MIT | 按角色组一个小组来完成同一项任务 |

这三份都是完整框架仓库。教学准备阶段用上面的入门课和本库已有的 `SKILL.md` 即可。
