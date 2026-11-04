# 组织仓库变更日志

本文件只记录组织级仓库结构和公共规则变化。各项目的功能版本与发布说明仍由对应仓库维护。

## 2026-11-04 追加纠正：两个产品，不以改名代替隔离

- 组织开屏明确区分招新考试与内部成员/组织平台；内部产品不是考试增量，CLI/MCP 同包属于内部 infra，不是 `recruitment-exam-kit` 的依赖。套件名称不变，`infra-handoff` 仅私有运维。
- 审计基线 `229e69c` 的组织 API 与考试仍共 DB、账号、启动流程；前述能力已合入与改名是历史事实，不等于已解耦或已部署。
- 第一阶段通过纠正 PR 审查同仓 `member-platform/server`、`member-platform/infra/...` 独立运行，根 `server/` 仅考试。源码待纠正 PR 合入，暂不发布尚不存在的 `main/member-platform` 链接；远端重命名与独立仓映射另行处理。
- 保留下方历史记录，不以本次文档纠正宣称生产部署、真实账号迁移或跨仓验收已经完成。

## 2026-11-04

### 仓库命名

- `recruitment-exam-platform` 重命名为 `alethicinsight-platform`，以覆盖成员、组织业务与 infra 接口职责；GitHub 保留旧 URL 重定向。`recruitment-exam-kit` 名称不变。

### 文档

- 在 `.github` 主根仓增加仓库边界与迁移记录。
- 组织开屏项目导航补充 `recruitment-exam-kit`，并将平台与考生套件的职责分开描述；开屏不展示迁移过程。

## 2026-11-02

### 新增

- 发布公共仓库 `recruitment-exam-kit`，作为考生本地考试套件、会话清洗和安装器的权威源码。
- 平台仓引入组织 API、成员事务网页及 `infra/interface/alethicinsight-cli` 单发行接口包。

### 变更

- `recruitment-exam-kit` 从 `recruitment-exam-platform` 的 `exam_kit/` 子目录拆出并保留相关 Git 历史；仓库名称不变。
- 平台移除旧套件目录的工作通过独立 Pull Request 审查，不以双主方式维护两份源码。
- CLI 与本地 MCP 保持同一 infra 接口包和版本，不拆独立 MCP 仓。
- 招新物料转入受控私有仓库；公开文档不记录个人信息、私有路径或真实运行数据。
