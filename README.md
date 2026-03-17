# OpenClaw Teams 配置

[![GitHub stars](https://img.shields.io/github/stars/little-apppple/openclaw-teams)](https://github.com/little-apppple/openclaw-teams/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/little-apppple/openclaw-teams)](https://github.com/little-apppple/openclaw-teams/network)
[![License](https://img.shields.io/github/license/little-apppple/openclaw-teams)](https://github.com/little-apppple/openclaw-teams)

一套开箱即用的 OpenClaw / Clawith 自驱型 AI Agent 团队配置，能自动发现需求、整理方案、解决问题、运营公司账号、管理文件和财务税务。

## 🚀 一键部署

在 OpenClaw 中复制以下提示词即可完成整个团队配置和技能安装：

```
请读取当前目录的所有配置文件，按照 agents/ 目录下的每个 Agent 的 soul.md、memory.md、triggers.yaml 创建对应的 Agent，并在团队层面按照 team/org.yaml 和 team/global_triggers.yaml 配置组织架构和全局触发器。然后安装 SKILLS.md 中列出的所有 Skills。完成后启动所有 Agent 并验证它们能正常协作运行。
```

## 📁 项目结构

```
openclawTeams/
├── agents/                    # Agent 配置目录
│   ├── ceo/                   # CEO Agent (首席执行官)
│   ├── product_manager/       # 产品经理 Agent
│   ├── solution_architect/    # 方案架构师 Agent
│   ├── operations_manager/   # 运营经理 Agent (自媒体发布)
│   ├── finance_manager/       # 财务 Agent (税务/报表)
│   └── document_manager/      # 文档管理员 Agent
├── team/                      # 团队配置
│   ├── org.yaml              # 组织架构
│   ├── global_triggers.yaml  # 全局触发器
│   └── company_info.md      # 公司信息
├── skills/                    # 技能配置模板
├── AGENTS.md                 # Agent 行为准则
├── SKILLS.md                 # Skills 安装清单
└── README.md                 # 本文件
```

## 🤖 团队成员

| Agent | 角色 | 核心能力 | 触发器 |
|-------|------|----------|--------|
| **CEO** | 首席执行官 | 战略规划、团队协调、决策 | 每日晨会、周报汇总、月度复盘 |
| **Product Manager** | 产品经理 | 需求发现与分析、产品规划 | 市场扫描、需求评审 |
| **Solution Architect** | 方案架构师 | 技术方案设计、系统架构 | 方案设计、技术调研 |
| **Operations Manager** | 运营经理 | 账号运营、内容管理、用户运营 | 内容发布、数据日报、热点追踪 |
| **Finance Manager** | 财务主管 | 财务管理、税务处理、报表 | 日常账务、税务申报、财务报表 |
| **Document Manager** | 文档管理员 | 文件管理、知识库、档案管理 | 文件整理、知识更新、备份检查 |

## 📋 所需 Skills

详见 [SKILLS.md](SKILLS.md)，核心技能包括：

- **基础**: web-search, skill-vetter, filesystem, code-execution, fetch
- **运营**: media-auto-publisher, browser, document, pdf, image-generation
- **财务**: spreadsheet, data-analysis, password-manager
- **增强**: research, notes, calendar, email

## 🛠️ 使用方法

1. **克隆仓库**
   ```bash
   git clone https://github.com/little-apppple/openclaw-teams.git
   cd openclaw-teams
   ```

2. **复制配置到 OpenClaw**
   - 将 `agents/` 目录下的配置复制到你的 OpenClaw workspace
   - 根据 `team/` 配置团队架构

3. **运行一键提示词**（在 OpenClaw 中）
   ```
   请读取当前目录的所有配置文件，按照 agents/ 目录下的每个 Agent 的 soul.md、memory.md、triggers.yaml 创建对应的 Agent，并在团队层面按照 team/org.yaml 和 team/global_triggers.yaml 配置组织架构和全局触发器。然后安装 SKILLS.md 中列出的所有 Skills。完成后启动所有 Agent 并验证它们能正常协作运行。
   ```

4. **启动团队**
   - AI 将自动完成所有配置和技能安装
   - 各 Agent 将根据触发器自动运行

## 📝 自定义配置

- 编辑 `team/company_info.md` 填入公司信息
- 根据需要修改各 Agent 的 `soul.md` 和 `triggers.yaml`
- 配置运营平台的 Cookie（详见 SKILLS.md）

## 📄 License

MIT License - 欢迎 fork 和贡献！

---

⭐ 如果对你有帮助，请点个 Star 支持一下！
