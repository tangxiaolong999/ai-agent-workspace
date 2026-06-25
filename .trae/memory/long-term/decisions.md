# Decisions

## Trae Agent Architecture (2026-06-25)

**背景**：初始化Trae专属个人AI工作空间，对标OpenClaw本地驻留Agent设计

**选项**：
1. 使用复杂记忆系统（数据库、服务）
2. 保持轻量，以Git仓库文件为基础

**决策**：选择方案2，保持轻量

**理由**：
- 简单的系统更容易维护和扩展
- Git仓库天然支持版本控制和跨设备同步
- 文件作为记忆载体，跨平台兼容
- 不需要额外的数据库或服务
- 适合个人使用场景

**架构选择**：
- 使用 `.trae/` 目录存放Trae专属数据
- 记忆分层：长期永久记忆 + 每日临时日志
- 技能目录遵循Trae标准 SKILL.md 规范

**相关文件**：
- [AGENTS.md](file:///d:/program/develop/AI-Agent/AGENTS.md)