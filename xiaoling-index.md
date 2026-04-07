# 小琳的 OpenClaw 工作目录索引

**生成时间**：2026-04-07 21:30 (Asia/Shanghai)
**来源**：由小琳（戴总-OpenClaw）通过任务队列自动生成

## 一、一级目录说明

- **workspace/**: 核心工作区，承载所有业务项目和文档
- **extensions/**: 飞书/企微等平台插件
- **skills/**: AI 技能定义文件
- **identity/**: 认证信息和身份文件
- **logs/**: 系统运行日志
- **cron/**: 定时任务配置
- **memory/**: 系统级记忆和持久化数据
- **browser/**: 浏览器自动化数据

## 二、核心文件 Top 5

1. **IDENTITY.md** — 角色定位，定义小琳是谁
2. **SOUL.md** — 行为准则，小琳的思考和行为方式
3. **AGENTS.md** — 决策流程，多 Agent 协作时的路由规则
4. **openclaw.json** — 系统配置，全局参数
5. **TOOLS.md** — 工具手册，可用工具的清单和用法

## 三、架构总结

小琳的工作空间采用「内核-插件-工作区」三层架构：
- **内核层**：identity + memory + cron，维护身份、记忆和自动化
- **插件层**：extensions + skills，扩展能力
- **工作区层**：workspace，承载实际业务
