<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/logo-dark.png">
  <source media="(prefers-color-scheme: light)" srcset="assets/logo-light.png">
  <img src="assets/logo-dark.png" alt="Alethic Insight — 人工智能社团" width="420">
</picture>

# CUMT Alethic Insight Lab

**CUMT Alethic Insight Lab** is a student-led AI society-lab and research-engineering community at **China University of Mining and Technology**.

## Two Products

| Product | Current entry and boundary |
| --- | --- |
| Recruitment exam | [Current exam-server repository](https://github.com/CUMT-Alethic-Insight-Lab/alethicinsight-platform) and candidate [recruitment-exam-kit](https://github.com/CUMT-Alethic-Insight-Lab/recruitment-exam-kit); the kit name stays unchanged. |
| Internal member and organization platform | Temporarily in the [same source repository](https://github.com/CUMT-Alethic-Insight-Lab/alethicinsight-platform). Member workflows, organization API and the single CLI/MCP infra package are not exam extensions or kit dependencies. |

**Source isolation pending correction PR:** first-stage target `member-platform/server` and `member-platform/infra/...` run the internal product independently; root `server/` serves exams only. At audit baseline `229e69c`, organization and exam APIs still share a database, accounts and startup flow. Review runtime isolation first; decide remote renaming and separate-repository mapping later. This page does not claim completed isolation, a new repository or production deployment. See [boundary correction](https://github.com/CUMT-Alethic-Insight-Lab/.github/blob/main/MIGRATION.md).

We work across:

- Language & NLP;
- Vision & Multimodal Learning;
- Agents & Reinforcement Learning;
- Trustworthy / Alethic Intelligence;
- AI Infrastructure;
- Open-source Practice;
- Research-engineering training for undergraduate students.

## About Alethic Insight

The name **Alethic Insight** is derived from the philosophical root *aletheia*, associated with truth, disclosure, and unconcealment.

For this community, it means:

> A place where hidden structures become visible, testable, and buildable.

We use this name in a grounded way: our work should connect ideas with evidence, systems, experiments, and open collaboration.

## What We Build

We maintain public repositories for organization documentation, open-source practice, learning resources, project templates, and selected research-engineering projects.

Sensitive materials such as real recruitment questions, interview records, scoring rubrics, internal governance records, credentials, and unreleased project plans are not published in public repositories.

## Contributing

Unless a repository states otherwise, contributions follow the organization-level guidelines in the `.github` repository.

For non-trivial changes, please open or join an Issue first, discuss the scope, then submit a focused Pull Request.

AI-assisted contributions are welcome, but contributors must disclose, verify, test, and understand their submissions.

## Contact

- Public contact: contact@alethicinsight.org
- GitHub contact: github@alethicinsight.org
- Website: https://aletheion.cn

