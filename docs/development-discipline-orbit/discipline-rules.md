# Discipline Rules

Development Discipline Orbit 为目标代码仓库提供三种开发反馈纪律。

## Purpose

- `diagnose`: 用于 bug、broken behavior、失败、性能回退和根因不明的问题。
- `tdd`: 用于新行为、行为变更、测试驱动开发和 red-green-refactor。
- `review-commit`: 用于审查当前 worktree 变更、修复阻塞问题、记录非阻塞技术债并创建 commit。

## Skill Choice

- 当前目标是确认真实失败模式、定位根因或提高复现率时，选择 `diagnose`。
- 当前目标是交付可观察行为变更时，选择 `tdd`。
- 当前目标是审查并提交已经完成的本地代码变更时，选择 `review-commit`。
- 同一任务同时包含失败排查和行为变更时，先选择 `diagnose`，再选择 `tdd`。
- 同一任务完成实现后需要提交时，最后选择 `review-commit`。

## Project Sources

按需发现并读取目标仓库中已经存在、且与当前任务相关的来源。下面是候选来源，不是目标仓库必须具备的目录结构：

- project memory，例如 `CONTEXT.md`、`CONTEXT-MAP.md` 指向的 context 文件，或其他仓库声明的领域语言文件。
- design decisions，例如现有 ADR 目录、架构决策文档，或其他仓库声明的决策记录。
- task context，例如已提供的 issue body、任务描述、acceptance criteria、人类补充说明或对话上下文。
- repository conventions，例如 `AGENTS.md`、`CLAUDE.md`、commit 规范、validation 命令或格式化规则。
- debt sinks，例如 issue body 中的 Debt Notes、tracker contract 声明的 section mapping，或仓库声明的技术债记录位置。

缺少任一候选来源不视为失败；继续使用可读取的代码、测试和任务上下文。

## Feedback Evidence

完成时报告：

- 使用的反馈循环。
- 失败信号如何被观察到。
- 通过信号如何被验证。
- 对 `review-commit`，说明审查的 commit scope、validation、commit hash，以及技术债记录位置；如果没有合适位置，则在完成报告列出 debt。
- 仍缺失的证据或需要人类补充的上下文。
