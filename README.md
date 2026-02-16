# code-tuner

A Claude Code plugin skill that analyzes server-side code for architectural violations, cross-layer duplication, abstraction opportunities, and validation issues. Outputs a comprehensive score (0-100) and actionable refactoring task list. Supports three-tier, two-tier, and DDD architectures across Java, Go, Node.js, Python, .NET, Rust, PHP, and Ruby.

## Installation

```bash
claude plugin install /path/to/code-tuner-skill
```

## Usage

```bash
# Full analysis (all phases)
/code-tuner full --lifecycle pre-launch

# Architecture compliance only
/code-tuner compliance

# Duplication detection only
/code-tuner duplication

# Abstraction analysis only
/code-tuner abstraction

# Regenerate report from existing phase outputs
/code-tuner report
```

Or use natural language:

```
please use code-tuner to analyze my project at /path/to/project. It's pre-launch.
```

## Design

See [design doc](../docs/plans/2026-02-17-code-tuner-design.md) and [implementation plan](../docs/plans/2026-02-17-code-tuner-implementation.md).

## License

MIT
