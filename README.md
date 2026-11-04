# CUMT Alethic Insight Lab GitHub Defaults

This repository defines organization-level public profile content, contribution guidelines, community health files, Issue templates, and Pull Request templates for CUMT Alethic Insight Lab.

## Product Navigation

The [organization profile](profile/README.md#two-products--两个产品) distinguishes the recruitment exam from the internal member and organization platform, currently in the [same source repository](https://github.com/CUMT-Alethic-Insight-Lab/alethicinsight-platform). The candidate [recruitment-exam-kit](https://github.com/CUMT-Alethic-Insight-Lab/recruitment-exam-kit) retains its name; organization CLI/MCP is one internal infra package, not a kit dependency. Runtime isolation into `member-platform/server` and `member-platform/infra/...` is pending correction PR review and merge; documentation does not establish isolation or deployment. See [current boundaries and the audit baseline](MIGRATION.md).

## Languages

- [English](README.en.md)
- [简体中文](README.zh-CN.md)

## Repository Changes

- [Repository boundaries and migration](MIGRATION.md)
- [Organization repository changelog](CHANGELOG.md)

These records are for maintainers. The organization profile presents current projects rather than migration activity.

## Repository Rule Inheritance

Unless otherwise specified by a repository, all repositories under CUMT Alethic Insight Lab follow the organization-level contribution guidelines and templates defined in this `.github` repository.

If a repository has its own README, CONTRIBUTING.md, Issue templates, Pull Request templates, or workflow rules, the repository-specific rules take precedence.

