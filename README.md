# OpenClaw Teams 配置

## 快速部署

一键配置整个 AI Agent 团队 + 安装所有 Skills：

```
请读取当前目录的所有配置文件，按照 agents/ 目录下的每个 Agent 的 soul.md、memory.md、triggers.yaml 创建对应的 Agent，并在团队层面按照 team/org.yaml 和 team/global_triggers.yaml 配置组织架构和全局触发器。然后安装 SKILLS.md 中列出的所有 Skills。完成后启动所有 Agent 并验证它们能正常协作运行。
```

## 项目结构

```
openclawTeams/
├── agents/                    # Agent 配置目录
│   ├── ceo/                   # CEO Agent
│   ├── product_manager/       # 产品经理 Agent
│   ├── solution_architect/    # 方案架构师 Agent
│   ├── operations_manager/    # 运营经理 Agent
│   ├── finance_manager/       # 财务 Agent
│   └── document_manager/      # 文档管理员 Agent
├── team/                      # 团队配置
│   ├── org.yaml              # 组织架构
│   ├── global_triggers.yaml  # 全局触发器
│   └── company_info.md       # 公司信息
├── skills/                   # 技能配置
├── AGENTS.md                 # Agent 行为准则
├── SKILLS.md                 # Skills 安装清单
└── README.md                 # 本文件
```

## 详细说明

- **每个 Agent 目录** 包含：`soul.md`（人设）、`memory.md`（记忆）、`triggers.yaml`（触发器）
- **team/** 目录包含团队协作配置
- **SKILLS.md** 列出所有需要安装的技能

## 使用方法

1. 克隆仓库到本地 OpenClaw 配置目录
2. 运行上述一键提示词
3. AI 将自动完成所有配置和技能安装
