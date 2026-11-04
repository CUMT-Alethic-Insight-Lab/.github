<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/logo-dark.png">
  <source media="(prefers-color-scheme: light)" srcset="assets/logo-light.png">
  <img src="assets/logo-dark.png" alt="Alethic Insight — 人工智能社团" width="520">
</picture>

<p align="center">
  <strong>CUMT Alethic Insight Lab</strong>
  <br />
  Student-led AI research, engineering, and open-source practice.
  <br />
  中国矿业大学学生主导的 AI 研究工程共同体。
</p>

<p align="center">
  <a href="https://aletheion.cn">Website</a>
  ·
  <a href="https://huggingface.co/Alethic-Insight">Hugging Face</a>
  ·
  <a href="mailto:contact@alethicinsight.org">Contact</a>
  ·
  <a href="README.en.md">English</a>
  ·
  <a href="README.zh-CN.md">简体中文</a>
</p>

---

**CUMT Alethic Insight Lab** is a student-led AI society-lab and research-engineering community at China University of Mining and Technology.

**CUMT Alethic Insight Lab** 是中国矿业大学学生主导的 AI 社团实验室，面向 AI 研究训练、工程实践、开源协作与项目孵化。

> A place where hidden structures become visible, testable, and buildable.

## Two Products / 两个产品

| Product 产品 | Entry and boundary 入口与边界 |
| --- | --- |
| Recruitment exam 招新考试 | [Exam server source / 考试服务端当前源码仓](https://github.com/CUMT-Alethic-Insight-Lab/alethicinsight-platform) + [recruitment-exam-kit](https://github.com/CUMT-Alethic-Insight-Lab/recruitment-exam-kit) candidate kit; the kit name stays unchanged. 考生套件名称不变。 |
| Internal member and organization platform 内部成员与组织平台 | [Current shared source repository / 当前同源仓](https://github.com/CUMT-Alethic-Insight-Lab/alethicinsight-platform). Member workflows, organization API and the single CLI/MCP infra package are an internal product, not an exam extension or kit dependency. 成员事务、组织 API 与同包 CLI/MCP 属于内部产品，不是考试增量或套件依赖。 |

**Source isolation pending correction PR / 源码待纠正 PR 合入：** the reviewed first-stage target is independently runnable `member-platform/server` and `member-platform/infra/...`, with root `server/` reserved for exams. At audit baseline `229e69c`, organization and exam APIs still share a database, accounts and startup flow. 文档分栏不代表已解耦；先审查同仓运行隔离，再决定远端重命名与分仓映射。No new repository or deployment is claimed / 不宣称新仓或部署已完成。See [boundary correction](https://github.com/CUMT-Alethic-Insight-Lab/.github/blob/main/MIGRATION.md) for maintainer details.

## Directions

| Area | Focus |
| --- | --- |
| Language & NLP | LLM applications, retrieval, Chinese NLP, evaluation |
| Vision & Multimodal Learning | VLM demos, visual reasoning, remote sensing, multimodal systems |
| Agents & Reinforcement Learning | tool use, planning, local assistants, feedback loops |
| Trustworthy / Alethic Intelligence | verification, reproducibility, safety, governance |
| AI Infrastructure | deployment, experiment tracking, model service, GPU and storage workflow |
| Open-source Practice | Issues, Pull Requests, review culture, responsible AI-assisted work |

## Start Here

| Need | Link |
| --- | --- |
| Join the lab | [join-us](https://github.com/CUMT-Alethic-Insight-Lab/join-us) |
| Recruitment process | [Process](https://github.com/CUMT-Alethic-Insight-Lab/join-us/blob/main/docs/en/process.md) / [招新流程](https://github.com/CUMT-Alethic-Insight-Lab/join-us/blob/main/docs/zh-CN/process.md) |
| Preparation guide | [Preparation](https://github.com/CUMT-Alethic-Insight-Lab/join-us/blob/main/docs/en/preparation.md) / [准备建议](https://github.com/CUMT-Alethic-Insight-Lab/join-us/blob/main/docs/zh-CN/preparation.md) |
| Exam server (internal product listed separately above) | [Current exam-server repository](https://github.com/CUMT-Alethic-Insight-Lab/alethicinsight-platform) |
| Candidate exam kit, cleaning code and downloads | [recruitment-exam-kit](https://github.com/CUMT-Alethic-Insight-Lab/recruitment-exam-kit) |
| Onboarding in depth | [open-onboarding](https://github.com/CUMT-Alethic-Insight-Lab/open-onboarding) |
| Curated AI resources | [awesome-ai](https://github.com/CUMT-Alethic-Insight-Lab/awesome-ai) |
| Public governance | [governance-public](https://github.com/CUMT-Alethic-Insight-Lab/governance-public) |
| Contribution rules | [CONTRIBUTING](https://github.com/CUMT-Alethic-Insight-Lab/.github/blob/main/CONTRIBUTING.md) |
| AI assistance policy | [AI Assistance](https://github.com/CUMT-Alethic-Insight-Lab/governance-public/blob/main/docs/en/ai-assistance-policy.md) / [AI 辅助规则](https://github.com/CUMT-Alethic-Insight-Lab/governance-public/blob/main/docs/zh-CN/ai-assistance-policy.md) |
| Models, datasets, demos | [Hugging Face Organization](https://huggingface.co/Alethic-Insight) |

## Key Documents

| Document | Link |
| --- | --- |
| Organization defaults | [`.github`](https://github.com/CUMT-Alethic-Insight-Lab/.github) |
| Pull Request template | [PULL_REQUEST_TEMPLATE](https://github.com/CUMT-Alethic-Insight-Lab/.github/blob/main/PULL_REQUEST_TEMPLATE.md) |
| Issue templates | [ISSUE_TEMPLATE](https://github.com/CUMT-Alethic-Insight-Lab/.github/tree/main/ISSUE_TEMPLATE) |
| Security policy | [SECURITY](https://github.com/CUMT-Alethic-Insight-Lab/.github/blob/main/SECURITY.md) |
| Code of conduct | [CODE_OF_CONDUCT](https://github.com/CUMT-Alethic-Insight-Lab/.github/blob/main/CODE_OF_CONDUCT.md) |
| Public charter | [Charter](https://github.com/CUMT-Alethic-Insight-Lab/governance-public/blob/main/docs/en/charter.md) / [章程](https://github.com/CUMT-Alethic-Insight-Lab/governance-public/blob/main/docs/zh-CN/charter.md) |
| Membership | [Membership](https://github.com/CUMT-Alethic-Insight-Lab/governance-public/blob/main/docs/en/membership.md) / [成员规则](https://github.com/CUMT-Alethic-Insight-Lab/governance-public/blob/main/docs/zh-CN/membership.md) |
| Project governance | [Project Governance](https://github.com/CUMT-Alethic-Insight-Lab/governance-public/blob/main/docs/en/project-governance.md) / [项目治理](https://github.com/CUMT-Alethic-Insight-Lab/governance-public/blob/main/docs/zh-CN/project-governance.md) |
| Open-source policy | [Open-source Policy](https://github.com/CUMT-Alethic-Insight-Lab/governance-public/blob/main/docs/en/open-source-policy.md) / [开源政策](https://github.com/CUMT-Alethic-Insight-Lab/governance-public/blob/main/docs/zh-CN/open-source-policy.md) |
| Release policy | [Release Policy](https://github.com/CUMT-Alethic-Insight-Lab/governance-public/blob/main/docs/en/release-policy.md) / [发布规范](https://github.com/CUMT-Alethic-Insight-Lab/governance-public/blob/main/docs/zh-CN/release-policy.md) |
| Review policy | [Review Policy](https://github.com/CUMT-Alethic-Insight-Lab/governance-public/blob/main/docs/en/review-policy.md) / [Review 规则](https://github.com/CUMT-Alethic-Insight-Lab/governance-public/blob/main/docs/zh-CN/review-policy.md) |
| Core-only charter draft | [Internal charter draft](https://github.com/CUMT-Alethic-Insight-Lab/internal-governance/blob/main/docs/zh-CN/charter-draft.md) |

## Public Repositories

| Repository | Purpose |
| --- | --- |
| [website](https://github.com/CUMT-Alethic-Insight-Lab/website) | Public website source and deployment |
| [alethicinsight-platform](https://github.com/CUMT-Alethic-Insight-Lab/alethicinsight-platform) | Current shared source for two products: recruitment exam and internal member/organization platform; runtime isolation pending correction PR |
| [recruitment-exam-kit](https://github.com/CUMT-Alethic-Insight-Lab/recruitment-exam-kit) | Candidate exam kit, open session-cleaning code, and installer |
| [join-us](https://github.com/CUMT-Alethic-Insight-Lab/join-us) | Public recruitment process and preparation guide |
| [governance-public](https://github.com/CUMT-Alethic-Insight-Lab/governance-public) | Public governance documents |
| [awesome-ai](https://github.com/CUMT-Alethic-Insight-Lab/awesome-ai) | Curated AI learning and research-engineering resources |
| [project-template](https://github.com/CUMT-Alethic-Insight-Lab/project-template) | Reusable project template |
| [open-onboarding](https://github.com/CUMT-Alethic-Insight-Lab/open-onboarding) | GitHub and open-source onboarding |
| [contribution-playground](https://github.com/CUMT-Alethic-Insight-Lab/contribution-playground) | Non-sensitive contribution practice |

## Rule

AI assistance is allowed. Blind submission is not.

Every AI-assisted contribution should disclose the model/tool, assisted parts, cross-checking method, tests actually run, and the contributor's understanding of the final solution.

## Contact

- Public contact: contact@alethicinsight.org
- GitHub contact: github@alethicinsight.org
- Hugging Face contact: hf@alethicinsight.org
