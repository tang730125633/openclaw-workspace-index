# 小婷的 OpenClaw 工作目录索引

**生成时间**：2026-04-07 21:35 (Asia/Shanghai)

## 一级目录说明

- **.openclaw/**: 核心配置与运行时根目录。
- **agency-agents/**: 包含 120+ 专家角色模板库，提供 P0 级别的能力支持。
- **agents/**: 存放不同角色的 Agent 实例配置与会话历史。
- **browser/**: 浏览器自动化相关的用户数据。
- **cron/**: 定时任务配置（jobs.json）及运行记录。
- **identity/**: 设备身份认证文件。
- **logs/**: 系统运行日志。
- **media/**: 存放图片、文档等媒体资源，包括生成的图片。
- **memory/**: 长期记忆、进化状态等持久化数据。
- **skills/**: 本地安装或开发的 Agent 技能文件夹。
- **workspace/**: 核心工作区，包含所有的项目代码、文档及核心人格文件（SOUL.md/USER.md）。

## 重要二/三级目录说明

- **workspace/projects/**: 存放具体的业务项目，如「AI-日报」、「财税通-员工导入」等。
- **workspace/skills/**: 工作区特定的自定义技能。
- **agents/main/**: 主 Agent（小婷）的运行时状态和 QMD 索引。
- **workspace/戴总的知识库/**: 存储电力行业专业知识，用于 RAG 检索。
- **agency-agents/.../**: 各类垂直领域专家的指令集（AGENTS.md/SOUL.md）。

## 核心文件 Top 5

1. **.openclaw/openclaw.json**: 全局系统配置文件，定义了插件、模型映射等。
2. **workspace/SOUL.md**: 小婷的人格核心，定义了思考习惯和行为准则。
3. **workspace/USER.md**: 泽龙（主人）的背景资料及项目状态，确保服务的对齐。
4. **.openclaw/cron/jobs.json**: 控制所有自动化任务（如 watchdog）的调度中心。
5. **agents/main/qmd/xdg-cache/qmd/index.sqlite**: 知识库 QMD 向量索引文件，决定了检索能力。

## 总结
我的工作空间采用了「配置与数据分离、通用专家库与特化技能并存」的架构。通过 `.openclaw` 维护底层运行，通过 `workspace` 承载业务逻辑，并利用 `agency-agents` 库快速切换和调用行业专家经验，形成了一个高效、可进化的智能助手环境。
