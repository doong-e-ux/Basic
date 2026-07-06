# basic

## Install Claude Code

```sh
./install.sh
```

Or run the underlying command directly:

```sh
curl -fsSL https://claude.ai/install.sh | bash
```

## Agent team

This repo defines a small team of specialized subagents under `.claude/agents/`. Claude Code picks the right one automatically, or you can invoke one directly (e.g. `@code-reviewer`, `@test-writer`).

| Agent | Purpose |
| --- | --- |
| `code-reviewer` | Reviews diffs/PRs for correctness, security, and maintainability issues |
| `test-writer` | Writes and runs tests for new or changed code |
| `docs-writer` | Keeps README/docs in sync with actual code behavior |
| `debugger` | Root-causes failing tests, crashes, or unexpected behavior |
