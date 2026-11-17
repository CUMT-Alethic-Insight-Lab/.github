# 仓库边界与迁移记录

本文件记录组织公开仓库的权威职责和结构性调整，供维护者核对链接、版本兼容与发布顺序。它不是组织开屏介绍，也不包含本机路径、私有数据或凭据。

## 当前公开仓库职责

| 仓库 | 当前职责 |
| --- | --- |
| `alethicinsight-platform` | 招新考试服务端，根 `server/` 仅承担考试；保留现有远端名称，不再作为成员产品的维护入口 |
| `alethicinsight-member-platform` | 独立成员与组织产品仓，承接原 `member-platform/` 子树：成员事务、组织 API 和同包 CLI/MCP 内部 infra；远端发布是本次导航 PR 的合入前置条件 |
| `recruitment-exam-kit` | 考生本地考试套件、会话清洗、安装器与局域网接收工具；名称保持不变 |
| `website` | 公共官网及官网专属内容与交互 |
| `open-onboarding` | 学习路径、实践顺序与协作入门 |
| `awesome-ai` | 学习资源索引 |
| `governance-public` | 正式公开制度 |

CLI 与本地 MCP 是同一**内部** infra 接口包，不拆成独立 MCP 产品仓，也不是考试套件依赖。`infra-handoff` 仅承担私有运维交接，不作为平台源码仓或公共客户端发行源。`Alethic-Insight-Frontend-Templates` 不属于本次调整范围。

## 2026-11-17：隔离已合并，成员产品独立仓发布

- 已核对隔离 [PR #6](https://github.com/CUMT-Alethic-Insight-Lab/alethicinsight-platform/pull/6) 为 MERGED，合并提交与核对时远端 `main` 为 `9dc7229cae1ee709c89a243e035b2685a11f2475`。下方“源码待纠正 PR 合入”仅是旧计划，不再描述当前状态。
- 内部成员与组织平台的独立仓名确定为 [alethicinsight-member-platform](https://github.com/CUMT-Alethic-Insight-Lab/alethicinsight-member-platform)，从原 `member-platform/` 子树提取；新仓内的路径和开发入口以新仓 README 为准，不继续将旧仓子目录列为成员产品权威入口。
- 考试仓保留 [alethicinsight-platform](https://github.com/CUMT-Alethic-Insight-Lab/alethicinsight-platform)，不再擅自重命名；[recruitment-exam-kit](https://github.com/CUMT-Alethic-Insight-Lab/recruitment-exam-kit) 名称不变。
- 新成员仓发布由产品维护者统一执行。本次核对新仓 API 返回 404，未确认其可访问；四个导航 PR 均应先标明该发布依赖，待发布确认后再合入，不把预定链接当作已完成发布的证据。
- CLI/MCP 仍为内部 infra 同一发行包；不创建独立 MCP 仓、不变成考试依赖。`infra-handoff` 仅私有运维交接，`exam-archive` 与前端模板仓不在操作范围。
- 本次仅纠正文档与导航，不进行生产部署、真实账号迁移或数据操作；源码隔离不等于跨仓兼容和运维切换验收。此前的测试记录属于对应代码工作，不是本次文档任务重跑的结果。

## 2026-11-04 追加纠正（历史计划，已由 2026-11-17 更新取代）

下方“已合入”与“已重命名”保留为历史事实，不代表运行隔离。审计确认 `origin/main=229e69c` 中组织 API 与考试共 DB、账号和启动流程，不能只改 README 冒称解耦。内部成员/组织平台不是考试增量。

第一阶段在现有同源仓通过纠正 PR 审查 `member-platform/` 独立运行内部产品，根 `server/` 仅考试。**源码待纠正 PR 合入**，当前只链接现有仓库，不生成尚不存在的 `main/member-platform` 链接。远端重命名与独立仓映射另行处理；本次文档更正不进行生产部署、真实账号迁移或真实数据操作。

## 2026-11 分仓调整

1. 组织接口和成员事务能力已合入 `alethicinsight-platform` 主分支。
2. `recruitment-exam-kit` 已从平台仓的 `exam_kit/` 子目录拆出，使用 Git subtree 保留相关历史。新仓是考生套件的权威源码。
3. 平台仓已通过独立 Pull Request 移除旧 `exam_kit/` 并更新跨仓链接，考生套件只在独立仓继续维护。
4. 招新物料另设私有仓库，仅收纳经过审查的内容；原始个人信息和本地运行数据不进入公开迁移记录。
5. `recruitment-exam-platform` 已重命名为 `alethicinsight-platform`，旧 URL 由 GitHub 保留重定向；`recruitment-exam-kit` 名称不变。

## 兼容与发布

- 考生套件与服务端 API 的兼容必须通过配对提交或发布记录确认，不能以目录拆分代替联调。
- 平台部署需要显式提供套件源码位置；不得依赖旧仓中仍然存在 `exam_kit/`。
- 仓库重命名或拆分后应更新项目 README、部署文档和组织项目导航；迁移过程本身不需要成为组织开屏内容。
- 详细本机路径、文件保全、未提交状态和回滚记录保存在受控工作区，不公开发布。

## 验证边界

仓库拆分、文档链接和自动测试分别验证。完整安装器重建、真实跨仓流程、生产部署与回滚演练需要独立记录，不能由本文件推定已完成。
