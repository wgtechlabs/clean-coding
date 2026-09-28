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

## Releases

Pushes to `main` run [Release Build Flow](https://github.com/wgtechlabs/release-build-flow-action).
The workflow plans a SemVer release from Clean Commit history, updates the plugin
manifest, then commits it with the changelog before creating the tag and GitHub Release.
The initial release is `0.1.0`. No release runs on `dev`.

The workflow uses the built-in `GITHUB_TOKEN` with `contents: write`; no PAT secret
is required. Branch rules must allow its release commit. Token-generated pushes
do not trigger another release run. After a release, sync `main` back into `dev`
to retain generated version and changelog changes.

## License

MIT. See [LICENSE](LICENSE).
