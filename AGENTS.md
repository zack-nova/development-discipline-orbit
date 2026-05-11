# Development Discipline Workflow

Development Discipline Workflow 用于在需要时选择并执行 TDD、diagnose 或 review-commit 反馈纪律。

## 按需读取

- 开发新行为、修复行为并明确需要 test-first 时，使用 `tdd` skill，并读取该 skill 指向的测试、mocking、refactoring 等材料。
- 遇到 bug、失败、性能回退或根因不明问题时，使用 `diagnose` skill。
- 完成本地变更并需要 review、记录非阻塞技术债或提交时，使用 `review-commit` skill。

## 常驻边界

- 不要把没有复现、失败信号或通过信号的工作报告成已验证。
- 报告完成结果时说明使用的反馈循环、观察到的失败信号、通过信号、commit 或技术债记录结果，以及仍缺失的证据。
