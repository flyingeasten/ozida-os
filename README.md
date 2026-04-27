# ozida OS

ozida OS 是我的个人 AI 操作系统。

它用于管理我在 AI 使用中的核心能力、工具连接、执行角色和工作流，让 skills、MCP、agents、workflows 可以被持续收集、整理、复用和升级。

## 核心定位

ozida OS 不是一个普通代码仓库，也不是 prompt 收集夹。

它是我的个人 AI 能力管理中枢，用来保存：

- **Skills**：可复用能力
- **MCP**：外部工具与数据连接
- **Agents**：不同 AI 执行角色
- **Workflows**：跨工具工作流
- **Principles**：AI 使用原则与安全边界
- **Templates**：标准模板

## 核心原则

1. 先方案，后执行
2. 默认只读分析
3. 所有写入必须确认
4. 不改写原始数据
5. 不保存敏感密钥
6. 数据由我掌控，AI 只在授权范围内访问
7. 能力可复用，流程可组合

## 系统架构

```text
Human
  ↓
Agent
  ↓
Skills + MCP
  ↓
Workflow
  ↓
Data Sources
```

## 各层说明

### Agent 层

Agent 是执行角色，负责理解任务、选择 skill、调用 MCP、整理结果。

示例：

- Tag Agent：标签体检
- Todo Agent：每日待办
- Airtable Agent：业务数据查询
- Archive Agent：对话归档

### Skills 层

Skills 是可复用能力模块，解决一类固定问题。

示例：

- flomo-tag-health-check
- memo-todo-loop
- airtable-sample-audit
- conversation-archive

### MCP 层

MCP 是连接器，负责让 AI 访问外部工具和数据。

示例：

- flomo MCP
- Airtable MCP
- GitHub MCP
- Feishu MCP
- Obsidian MCP

### Workflow 层

Workflow 是流程编排，把 skills 和 MCP 组合成可执行流程。

示例：

- flomo 标签体检流程
- 每日待办流程
- Airtable 样品审计流程
- AI 对话归档流程

### Data Sources 层

数据源是真实信息所在的位置。

示例：

- flomo
- Airtable
- GitHub
- 飞书 / 飞书文档
- Obsidian
- 本地文件

## 安全边界

本仓库只保存规则、说明、模板和流程。

**不保存：**

- API Key
- Token
- Cookie
- 客户敏感信息
- flomo 原始数据
- Airtable 业务数据
- 私人隐私内容

## 当前状态

ozida OS 正在建设中。

当前优先建设：

1. README 与目录结构
2. AI 操作原则
3. flomo 标签体检 skill
4. MCP 使用边界
5. workflow 标准模板

## 一句话原则

ozida OS 是我的个人 AI 操作系统配置中枢，用来管理能力、权限、边界和流程。
