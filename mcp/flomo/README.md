# flomo MCP

## 说明

flomo Max 会员专属功能。

通过官方 MCP 协议，AI 可以直接读取、写入、搜索你的 flomo 笔记。

---

## 能力范围

- 创建 memo
- 读取 memo
- 搜索 memo（按标签、关键词）
- 更新 memo 状态/标签
- 删除 memo

---

## 获取 Token

1. 打开 flomo 设置
2. 进入「MCP 连接」
3. 切换到「个人 Token」标签
4. 点击「创建」，给 Token 起个名字（如 Claude、Cola）
5. 立即复制，只显示一次

---

## 配置方式（Claude Code）

### 方式一：命令行（推荐）

```bash
claude mcp add --transport http flomo https://flomoapp.com/mcp \
  --header "Authorization: Bearer YOUR_FLOMO_TOKEN"
```

### 方式二：手动编辑配置文件

编辑 `~/.claude/settings.json`，在 `mcpServers` 里添加：

```json
"flomo": {
  "type": "http",
  "url": "https://flomoapp.com/mcp",
  "headers": {
    "Authorization": "Bearer YOUR_FLOMO_TOKEN"
  }
}
```

配置后重启 Claude Code 生效。

---

## 验证

在 Claude Code 里直接说：

```
帮我看看最近 7 天的 flomo memo
```

能返回内容即表示接通。

---

## 安全边界

- Token 不保存在本仓库
- 默认只读分析
- 写入、修改、删除操作需要确认

---

## 依赖

- flomo Max 会员
- Claude Code（本地安装）

---

## 一句话

flomo MCP 让 Claude Code 可以直接读写你的笔记库，AI 辅助，你做决定。
