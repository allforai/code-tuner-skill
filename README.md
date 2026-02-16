# code-tuner

A Claude Code plugin skill that analyzes server-side code for architectural violations, cross-layer duplication, abstraction opportunities, and validation issues. Outputs a comprehensive score (0-100) and actionable refactoring task list. Supports three-tier, two-tier, and DDD architectures across Java, Go, Node.js, Python, .NET, Rust, PHP, and Ruby.

## Installation

```bash
claude plugin install /path/to/code-tuner-skill
```

## Usage

```
/code-tuner full
/code-tuner compliance
/code-tuner duplication
/code-tuner abstraction
/code-tuner report
```

Or use natural language:

```
请用 code-tuner 分析我的项目。项目路径是 /path/to/project。项目状态是未上线。
please use code-tuner to analyze my project at /path/to/project. It's pre-launch.
```

Modes:
- **full** — Phase 0 → 1 → 2 → 3 → 4 (default)
- **compliance** — Architecture compliance only
- **duplication** — Duplication detection only
- **abstraction** — Abstraction analysis only
- **report** — Regenerate report from existing phase outputs

Lifecycle is asked interactively if not specified (pre-launch or maintenance).

## License

MIT
