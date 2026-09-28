# Clean Coding

A standalone Codex plugin containing the `clean-development` skill for implementing features, fixing bugs, and refactoring with minimal complexity and evidence-backed verification.

## Install

```bash
codex plugin marketplace add wgtechlabs/clean-coding
codex plugin add clean-coding@clean-coding
```

Start a new chat after installation and invoke `$clean-development`.
Agents supporting the Agent Skills format can load `skills/clean-development/` directly.

## Scope

The skill covers clarification, implementation, relevant UI design and polish, verification, and maintainability review. It is self-contained and requires no other skills. Repository access and task-specific development tools are still needed.

Repository instructions and user requests remain authoritative. Installing this skill does not authorize publishing, merging, or deploying changes.

## Attribution

Extracted from [Clean Workflow](https://github.com/wgtechlabs/clean-workflow). The skill includes its source lineage and the Codelynx article that inspired the workflow.

## Contributing

Use short-lived feature branches from `dev`, squash merge feature PRs into `dev`, and promote `dev` to `main` with a regular merge commit. Follow [Clean Commit](https://github.com/wgtechlabs/clean-commit) message conventions.

## License

MIT. See [LICENSE](LICENSE).
