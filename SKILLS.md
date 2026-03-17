# OpenClaw Teams 所需 Skills 完整清单

## 安装命令

在终端中运行以下命令批量安装所有技能：

```bash
# ===== 基础核心技能 (必装) =====

# 1. 网络搜索 - 实时搜索互联网信息
openclaw skills install web-search

# 2. 安全守门人 - 扫描其他技能代码，检查安全
openclaw skills install skill-vetter

# 3. 文件读写 - 基础文件操作
openclaw skills install filesystem

# 4. 代码执行 - 运行代码和脚本
openclaw skills install code-execution


# ===== 产品经理 & 方案架构师 =====

# 5. 高级搜索 - 更强大的搜索能力
openclaw skills install research

# 6. 浏览器操作 - 自动化浏览器操作
openclaw skills install browser

# 7. 阅读理解 - 提取网页/文档关键信息
openclaw skills install fetch


# ===== 运营经理 (自媒体发布) =====

# 8. 自动化发布 - 自媒体多平台发布 (需配置Cookie)
openclaw skills install media-auto-publisher

# 9. PDF处理 - 生成和读取PDF
openclaw skills install pdf

# 10. 文档处理 - Word/Excel/PPT文档
openclaw skills install document

# 11. 图片生成 - AI生成配图
openclaw skills install image-generation


# ===== 财务 & 文档管理 =====

# 12. 数据分析 - 处理和分析数据
openclaw skills install data-analysis

# 13. 表格处理 - Excel操作
openclaw skills install spreadsheet

# 14. 密码管理 - 安全存储敏感信息
openclaw skills install password-manager


# ===== 高级可选技能 =====

# 15. 邮件处理 - 收发邮件
openclaw skills install email

# 16. 日历管理 - 日程安排
openclaw skills install calendar

# 17. 任务管理 - 待办事项
openclaw skills install todo

# 18. 笔记记录 - 笔记和知识整理
openclaw skills install notes

# 19. API调用 - 第三方API集成
openclaw skills install api-caller

# 20. HTTP请求 - 网络请求
openclaw skills install http
```

## 按 Agent 分类的技能配置

### CEO Agent
| 技能 | 用途 | 优先级 |
|------|------|--------|
| web-search | 搜索行业信息 | ⭐⭐⭐ |
| fetch | 获取网页内容 | ⭐⭐⭐ |
| notes | 记录决策 | ⭐⭐ |
| todo | 任务跟踪 | ⭐⭐ |
| calendar | 日程管理 | ⭐ |

### Product Manager Agent
| 技能 | 用途 | 优先级 |
|------|------|--------|
| web-search | 市场调研 | ⭐⭐⭐ |
| research | 深度研究 | ⭐⭐⭐ |
| fetch | 竞品分析 | ⭐⭐⭐ |
| browser | 用户行为分析 | ⭐⭐ |
| data-analysis | 需求数据分析 | ⭐⭐ |

### Solution Architect Agent
| 技能 | 用途 | 优先级 |
|------|------|--------|
| web-search | 技术调研 | ⭐⭐⭐ |
| code-execution | 技术验证 | ⭐⭐⭐ |
| fetch | 文档获取 | ⭐⭐⭐ |
| filesystem | 代码操作 | ⭐⭐⭐ |
| http | API测试 | ⭐⭐ |

### Operations Manager Agent
| 技能 | 用途 | 优先级 |
|------|------|--------|
| media-auto-publisher | 自媒体发布 | ⭐⭐⭐ |
| web-search | 热点追踪 | ⭐⭐⭐ |
| fetch | 内容获取 | ⭐⭐⭐ |
| pdf | 报告生成 | ⭐⭐⭐ |
| document | 文档撰写 | ⭐⭐⭐ |
| image-generation | 配图生成 | ⭐⭐ |
| browser | 平台操作 | ⭐⭐ |

### Finance Manager Agent
| 技能 | 用途 | 优先级 |
|------|------|--------|
| spreadsheet | 财务报表 | ⭐⭐⭐ |
| data-analysis | 财务分析 | ⭐⭐⭐ |
| web-search | 税法查询 | ⭐⭐⭐ |
| pdf | 发票处理 | ⭐⭐⭐ |
| document | 文档生成 | ⭐⭐⭐ |
| password-manager | 敏感信息 | ⭐⭐ |

### Document Manager Agent
| 技能 | 用途 | 优先级 |
|------|------|--------|
| filesystem | 文件管理 | ⭐⭐⭐ |
| pdf | 文档转换 | ⭐⭐⭐ |
| document | 文档处理 | ⭐⭐⭐ |
| fetch | 内容获取 | ⭐⭐ |
| notes | 知识整理 | ⭐⭐ |

## 推荐安装顺序

```bash
# 第一批：基础核心 (先装这些)
openclaw skills install web-search
openclaw skills install skill-vetter
openclaw skills install filesystem
openclaw skills install code-execution
openclaw skills install fetch

# 第二批：运营必备
openclaw skills install media-auto-publisher
openclaw skills install browser
openclaw skills install document
openclaw skills install pdf

# 第三批：财务文档
openclaw skills install spreadsheet
openclaw skills install data-analysis

# 第四批：增强功能
openclaw skills install image-generation
openclaw skills install notes
openclaw skills install calendar
```

## 技能检查命令

安装完成后，检查技能状态：

```bash
# 查看已安装的技能
openclaw skills list

# 检查技能依赖
openclaw skills check

# 更新所有技能
openclaw skills update
```

## 常见问题

### Q: 技能安装失败
```bash
# 检查网络连接
# 更换国内镜像源
openclaw config set mirror https://pypi.tuna.tsinghua.edu.cn
```

### Q: 技能冲突
```bash
# 禁用冲突的技能
openclaw skills disable <skill-name>

# 检查依赖
openclaw skills check --fix
```

### Q: 需要重新安装
```bash
# 卸载技能
openclaw skills uninstall <skill-name>

# 重新安装
openclaw skills install <skill-name>
```
